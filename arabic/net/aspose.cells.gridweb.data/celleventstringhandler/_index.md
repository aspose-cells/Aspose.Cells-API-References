---
title: "المندوب CellEventStringHandler"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "يمثل الطريقة التي تهدف إلى معالجة أحداث الخلية. نفس واجهة CellEventHandler ولكنها تُعيد نتيجة نصية"
type: docs
url: /ar/net/aspose.cells.gridweb.data/celleventstringhandler/
---
## CellEventStringHandler delegate

يمثل الطريقة التي تهدف إلى معالجة أحداث الخلية. نفس واجهة CellEventHandler، ولكنها تُعيد نتيجة نصية.

String **handleCellEvent**(Object sender, CellEventArgs e);

```csharp
public delegate string CellEventStringHandler(object sender, CellEventArgs e);
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sender | Object | شبكة المصدر للحدث. |
| e | CellEventArgs | معامل الحدث. الـ e.Cell هو الخلية التي تُطلق الحدث. الـ e.Argument يحتوي على معامل الحدث. |

### قيمة الإرجاع

قيمة string

### انظر أيضًا

* class [CellEventArgs](../../aspose.cells.gridweb/celleventargs/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


