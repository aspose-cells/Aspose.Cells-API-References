---
title: "WebWorksheet.FreezePanes"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة WebWorksheet. تجمّد الألواح عند الخلية المحددة في ورقة العمل"
type: docs
url: /ar/net/aspose.cells.gridweb.data/webworksheet/freezepanes/
---
## WebWorksheet.FreezePanes method

يثبت الألواح عند الخلية المحددة في ورقة العمل.

```csharp
public void FreezePanes(int row, int column, int freezedRows, int freezedColumns)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف. |
| عمود | Int32 | فهرس العمود. |
| freezedRows | Int32 | عدد الصفوف الظاهرة في اللوحة العلوية، لا يزيد عن فهرس الصف. |
| freezedColumns | Int32 | عدد الأعمدة الظاهرة في اللوحة اليسرى، لا يزيد عن فهرس العمود. |

### ملاحظات

لا يمكن أن يكون فهرس الصف وفهرس العمود كلاهما صفرًا. كما لا يمكن أن يكون عدد الصفوف وعدد الأعمدة كلاهما صفرًا.

المعاملان الأولان يحددان موقع التجمد، والمعاملان الأخيران يحددان المنطقة المجمدة في اللوحة العلوية اليسرى.

### انظر أيضًا

* class [WebWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


