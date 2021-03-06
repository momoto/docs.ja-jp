---
title: Windows フォーム コントロールの属性
ms.date: 03/30/2017
helpviewer_keywords:
- attributes [Windows Forms]
- attributes [Windows Forms], data binding properties
- attributes [Windows Forms], control properties
- attributes [Windows Forms], classes
ms.assetid: 2c5640e9-6c6c-49d7-a5e4-a768f6be7853
ms.openlocfilehash: 9dd4c2aabe1517b66d8e499de3cf2671bb94e0d6
ms.sourcegitcommit: 9b552addadfb57fab0b9e7852ed4f1f1b8a42f8e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2019
ms.locfileid: "61954376"
---
# <a name="attributes-in-windows-forms-controls"></a>Windows フォーム コントロールの属性
.NET Framework には、カスタム コントロールおよびカスタム コンポーネントのメンバーに適用できるさまざまな属性が用意されています。 これらの属性には、クラスの実行時の動作に影響を及ぼすものもあれば、デザイン時の動作に影響を及ぼすものもあります。  
  
## <a name="attributes-for-control-and-component-properties"></a>コントロールおよびコンポーネントのプロパティの属性  
 次の表には、カスタム コントロールおよびカスタム コンポーネントのプロパティや他のメンバーに適用できる属性が示されています。 これらの属性の多くを使用する例を参照してください[方法。Windows フォーム コントロールに属性を適用](how-to-apply-attributes-in-windows-forms-controls.md)します。  
  
|属性|説明|  
|---------------|-----------------|  
|<xref:System.ComponentModel.AmbientValueAttribute>|プロパティに渡す値を指定し、そのプロパティが別のソースから値を取得するようにします。 これは "*アンビエンス*" と呼ばれています。|  
|<xref:System.ComponentModel.BrowsableAttribute>|プロパティまたはイベントが **[プロパティ]** ウィンドウに表示されるかどうかを指定します。|  
|<xref:System.ComponentModel.CategoryAttribute>|プロパティまたはイベントに表示するときにグループ化するためのカテゴリの名前を指定します、<xref:System.Windows.Forms.PropertyGrid>コントロールに対して設定<xref:System.Windows.Forms.PropertySort.Categorized>モード。|  
|<xref:System.ComponentModel.DefaultValueAttribute>|プロパティの既定値を指定します。|  
|<xref:System.ComponentModel.DescriptionAttribute>|プロパティまたはイベントの説明文を指定します。|  
|<xref:System.ComponentModel.DisplayNameAttribute>|引数を受け取らないプロパティ、イベント、または `public void` メソッドの表示名を指定します。|  
|<xref:System.ComponentModel.EditorAttribute>|プロパティの変更に使用するエディターを指定します。|  
|<xref:System.ComponentModel.EditorBrowsableAttribute>|プロパティまたはメソッドをエディターで表示できるかどうかを指定します。|  
|<xref:System.ComponentModel.Design.HelpKeywordAttribute>|クラスまたはメンバーのコンテキスト キーワードを指定します。|  
|<xref:System.ComponentModel.LocalizableAttribute>|プロパティをローカライズする必要があるかどうかを指定します。|  
|<xref:System.ComponentModel.PasswordPropertyTextAttribute>|アスタリスクなどの文字で、オブジェクトのテキスト表記を隠すように指示します。|  
|<xref:System.ComponentModel.ReadOnlyAttribute>|デザイン時に、この属性がバインドされるプロパティが読み取り専用か読み取り/書き込み可能かを指定します。|  
|<xref:System.ComponentModel.RefreshPropertiesAttribute>|関連付けられているプロパティ値が変更されたときに、プロパティ グリッドが更新されるように指定します。|  
|<xref:System.ComponentModel.TypeConverterAttribute>|この属性が関連付けられているオブジェクトのコンバーターとして使用する型を指定します。|  
  
## <a name="attributes-for-data-binding-properties"></a>データ バインディング プロパティの属性  
 次の表には、カスタム コントロールおよびカスタム コンポーネントがデータ バインディングと相互作用する方法を指定するために適用できる属性が示されています。  
  
|属性|説明|  
|---------------|-----------------|  
|<xref:System.ComponentModel.BindableAttribute>|バインディングにプロパティが通常、使用されるかどうかを指定します。|  
|<xref:System.ComponentModel.ComplexBindingPropertiesAttribute>|コンポーネントのデータ ソースおよびデータ メンバーのプロパティを指定します。|  
|<xref:System.ComponentModel.DefaultBindingPropertyAttribute>|コンポーネントの既定のバインディング プロパティを指定します。|  
|<xref:System.ComponentModel.LookupBindingPropertiesAttribute>|コンポーネントのデータ ソースおよびデータ メンバーのプロパティを指定します。|  
|<xref:System.ComponentModel.AttributeProviderAttribute>|属性のリダイレクトを有効にします。|  
  
## <a name="attributes-for-classes"></a>クラスの属性  
 次の表には、デザイン時にカスタム コントロールおよびカスタム コンポーネントの動作を指定するために適用できる属性が示されています。  
  
|属性|説明|  
|---------------|-----------------|  
|<xref:System.ComponentModel.DefaultEventAttribute>|コンポーネントの既定のイベントを指定します。|  
|<xref:System.ComponentModel.DefaultPropertyAttribute>|コンポーネントの既定のプロパティを指定します。|  
|<xref:System.ComponentModel.DesignerAttribute>|コンポーネントのデザイン時サービスを実装するために使用されるクラスを指定します。|  
|<xref:System.ComponentModel.DesignerCategoryAttribute>|クラスのデザイナーが特定のカテゴリに属することを指定します。|  
|<xref:System.ComponentModel.ToolboxItemAttribute>|ツールボックス項目の属性を表します。|  
|<xref:System.ComponentModel.ToolboxItemFilterAttribute>|ツールボックス項目に使用するフィルター文字列とフィルターの種類を指定します。|  
  
## <a name="see-also"></a>関連項目

- <xref:System.Attribute>
- [方法: Windows フォーム コントロールに属性を適用します。](how-to-apply-attributes-in-windows-forms-controls.md)
- [デザイン時サポートの拡張](https://docs.microsoft.com/previous-versions/visualstudio/visual-studio-2013/37899azc(v=vs.120))
- [.NET Framework を使用したカスタム Windows フォーム コントロールの開発](developing-custom-windows-forms-controls.md)
