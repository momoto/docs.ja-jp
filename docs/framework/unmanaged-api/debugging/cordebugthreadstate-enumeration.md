---
title: CorDebugThreadState 列挙型
ms.date: 03/30/2017
api_name:
- CorDebugThreadState
api_location:
- mscordbi.dll
api_type:
- COM
f1_keywords:
- CorDebugThreadState
helpviewer_keywords:
- CorDebugThreadState enumeration [.NET Framework debugging]
ms.assetid: a3ccdf18-4ec6-494d-9024-48e5c8c724f5
topic_type:
- apiref
ms.openlocfilehash: 1ff36e8ef6b7c02eea5b02bc22587bc3889df093
ms.sourcegitcommit: 559fcfbe4871636494870a8b716bf7325df34ac5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/30/2019
ms.locfileid: "73133690"
---
# <a name="cordebugthreadstate-enumeration"></a>CorDebugThreadState 列挙型
デバッグのスレッドの状態を指定します。  
  
## <a name="syntax"></a>構文  
  
```cpp  
typedef enum CorDebugThreadState {  
    THREAD_RUN,  
    THREAD_SUSPEND  
} CorDebugThreadState;  
```  
  
## <a name="members"></a>メンバー  
  
|メンバー|説明|  
|------------|-----------------|  
|`THREAD_RUN`|デバッグイベントが発生しない限り、スレッドは自由に実行できます。|  
|`THREAD_SUSPEND`|スレッドを実行できません。|  
  
## <a name="remarks"></a>Remarks  
 デバッガーは、`CorDebugThreadState` 列挙体を使用して、スレッドの実行を制御します。 スレッドの状態を設定するには、次のように指定する必要があります: [: SetDebugState](../../../../docs/framework/unmanaged-api/debugging/icordebugthread-setdebugstate-method.md)または、モジュール[:: SetAllThreadsDebugState](../../../../docs/framework/unmanaged-api/debugging/icordebugcontroller-setallthreadsdebugstate-method.md)メソッド。  
  
 [ホスティング API](../../../../docs/framework/unmanaged-api/hosting/index.md)に提供されるコールバックによってメッセージポンプが可能になるため、中断された状態は必要ありません。  
  
## <a name="requirements"></a>［要件］  
 **:** 「[システム要件](../../../../docs/framework/get-started/system-requirements.md)」を参照してください。  
  
 **ヘッダー:** CorDebug.idl、CorDebug.h  
  
 **ライブラリ:** CorGuids.lib  
  
 **.NET Framework のバージョン:** [!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]  
  
## <a name="see-also"></a>関連項目

- [列挙型のデバッグ](../../../../docs/framework/unmanaged-api/debugging/debugging-enumerations.md)
