---
title: '方法: イメージ要素を使用する'
ms.date: 03/30/2017
dev_langs:
- csharp
- vb
helpviewer_keywords:
- controls [WPF], Image
- Image control [WPF]
- rendering images [WPF]
ms.assetid: 5b92e74b-1b56-4756-ac64-d5e9e08d9854
ms.openlocfilehash: 164eee7c10d9e388c6e6ee695af479ca2d6974b3
ms.sourcegitcommit: 68653db98c5ea7744fd438710248935f70020dfb
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "69958325"
---
# <a name="how-to-use-the-image-element"></a>方法: イメージ要素を使用する
この例では、 <xref:System.Windows.Controls.Image>要素を使用してアプリケーションにイメージを含める方法を示します。  
  
## <a name="example"></a>例  
 次の例では、幅 200 ピクセルのイメージをレンダリングする方法を示します。 この[!INCLUDE[TLA#tla_xaml](../../../../includes/tlasharptla-xaml-md.md)]例では、イメージの定義に属性の構文とプロパティ タグ構文の両方を使用します。 属性構文とプロパティ構文の詳細については、「[依存関係プロパティの概要](../advanced/dependency-properties-overview.md)」を参照してください。 は<xref:System.Windows.Media.Imaging.BitmapImage> 、イメージのソースデータを定義するために使用され、プロパティタグ構文の例に対して明示的に定義されます。 また<xref:System.Windows.Media.Imaging.BitmapImage.DecodePixelWidth%2A> <xref:System.Windows.FrameworkElement.Width%2A> 、の<xref:System.Windows.Controls.Image>は、のと同じ幅に設定されます。<xref:System.Windows.Media.Imaging.BitmapImage> これは、イメージのレンダリングに使用するメモリ量が最小になるように実行されます。  
  
> [!NOTE]
> 一般に、レンダリングされるイメージのサイズを指定する場合は、 <xref:System.Windows.FrameworkElement.Width%2A>またはの<xref:System.Windows.FrameworkElement.Height%2A>両方を指定します。 いずれかのみを指定する場合、イメージの縦横比が保持されます。 それ以外の場合、イメージの拡大表示やゆがみ表示が予期せず発生する可能性があります。 イメージの伸縮動作を制御するには、 <xref:System.Windows.Controls.Image.Stretch%2A>プロパティ<xref:System.Windows.Controls.Image.StretchDirection%2A>とプロパティを使用します。  
  
> [!NOTE]
> <xref:System.Windows.FrameworkElement.Width%2A>または<xref:System.Windows.FrameworkElement.Height%2A>のいずれかを使用してイメージのサイズを指定する場合<xref:System.Windows.Media.Imaging.BitmapImage.DecodePixelWidth%2A>は、 <xref:System.Windows.Media.Imaging.BitmapImage.DecodePixelHeight%2A>同じサイズにまたはを設定する必要があります。  
  
 プロパティ<xref:System.Windows.Controls.Image.Stretch%2A>は、イメージ要素を塗りつぶすためにイメージソースをどのように拡大するかを決定します。 詳細については、<xref:System.Windows.Media.Stretch> 列挙型のページをご覧ください。  
  
 [!code-xaml[ImageElementExample_snip#ImageSimpleExampleInlineMarkup](~/samples/snippets/csharp/VS_Snippets_Wpf/ImageElementExample_snip/CSharp/ImageSimpleExample.xaml#imagesimpleexampleinlinemarkup)]  
  
## <a name="example"></a>例  
 次の例は、コードを使用して幅 200 ピクセルのイメージをレンダリングする方法を示しています。  
  
> [!NOTE]
> 設定<xref:System.Windows.Media.Imaging.BitmapImage>プロパティは、 <xref:System.Windows.Media.Imaging.BitmapImage.BeginInit%2A>および<xref:System.Windows.Media.Imaging.BitmapImage.EndInit%2A>ブロック内で実行する必要があります。  
  
 [!code-csharp[ImageElementExample_snip#ImageSimpleExampleInlineCode1](~/samples/snippets/csharp/VS_Snippets_Wpf/ImageElementExample_snip/CSharp/ImageSimpleExample.xaml.cs#imagesimpleexampleinlinecode1)]
 [!code-vb[ImageElementExample_snip#ImageSimpleExampleInlineCode1](~/samples/snippets/visualbasic/VS_Snippets_Wpf/ImageElementExample_snip/VB/ImageSimpleExample.xaml.vb#imagesimpleexampleinlinecode1)]  
  
## <a name="see-also"></a>関連項目

- [イメージングの概要](../graphics-multimedia/imaging-overview.md)
