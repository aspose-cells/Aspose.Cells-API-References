---
title: "المندوب CellEventHandler"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "يمثل الواجهة التي تهدف إلى معالجة أحداث الخلية"
type: docs
url: /ar/net/aspose.cells.griddesktop.data/celleventhandler/
---
## CellEventHandler delegate

يمثل الواجهة التي تهدف إلى معالجة أحداث الخلية.

void **handleCellEvent**(Object sender, CellEventArgs e);

```csharp
public delegate void CellEventHandler(object sender, CellEventArgs e);
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sender | Object | شبكة المصدر للحدث. |
| e | CellEventArgs | معامل الحدث. الـ e.Cell هو الخلية التي تُطلق الحدث. الـ e.Argument يحتوي على معامل الحدث. |

### انظر أيضًا

* class [CellEventArgs](../../aspose.cells.griddesktop/celleventargs/)
* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


