---
title: "Worksheet.FreezePanes"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Worksheet. تُجمد الألواح عند الخلية المحددة في ورقة العمل"
type: docs
url: /ar/net/aspose.cells.griddesktop/worksheet/freezepanes/
---
## FreezePanes(string, int, int) {#freezepanes_1}

يثبت الألواح عند الخلية المحددة في ورقة العمل.

```csharp
public void FreezePanes(string cellName, int freezedRows, int freezedColumns)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| cellName | String | اسم الخلية. |
| freezedRows | Int32 | عدد الصفوف الظاهرة في اللوحة العلوية، لا يزيد عن فهرس الصف. |
| freezedColumns | Int32 | عدد الأعمدة الظاهرة في اللوحة اليسرى، لا يزيد عن فهرس العمود. |

### ملاحظات

لا يمكن أن يكون فهرس الصف وفهرس العمود كلاهما صفرًا. كما لا يمكن أن يكون عدد الصفوف وعدد الأعمدة كلاهما صفرًا.

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## FreezePanes(int, int, int, int) {#freezepanes}

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

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


