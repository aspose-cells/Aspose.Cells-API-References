---
title: "المندوب CellErrorHandler"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "يمثل الواجهة التي تهدف إلى معالجة أحداث خطأ الخلية"
type: docs
url: /ar/net/aspose.cells.gridweb.data/cellerrorhandler/
---
## CellErrorHandler delegate

يمثل الواجهة التي تهدف إلى معالجة أحداث أخطاء الخلية.

void **handleCellEvent**(Object sender, GridCellException ex, OnErrorActionQuery query);

```csharp
public delegate void CellErrorHandler(object sender, WebCellException ex, 
    OnErrorActionQuery action);
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sender | Object | مصدر الحدث. |
| ex | WebCellException | خطأ عملية الخلية. |
| action | OnErrorActionQuery | يمكن الحصول على معلومات نوع إجراء onerror. |

### انظر أيضًا

* class [WebCellException](../webcellexception/)
* class [OnErrorActionQuery](../onerroractionquery/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


