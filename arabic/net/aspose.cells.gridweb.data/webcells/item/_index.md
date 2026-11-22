---
title: "WebCells.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebCells. يحصل على عنصر Cell عند فهرس صف الخلية والعمود المحددين"
type: docs
url: /ar/net/aspose.cells.gridweb.data/webcells/item/
---
## WebCells indexer (1 of 2)

يحصل على عنصر Cell عند فهرس صف الخلية والعمود المحددين.

```csharp
public WebCell this[int row, int column] { get; }
```

| معامل | الوصف |
| --- | --- |
| صف | فهرس الصف. |
| عمود | فهرس العمود. |

### قيمة الإرجاع

كائن Cell.

### أمثلة

```csharp
[C#]

Cells cells = excel.Worksheets[0].Cells;
Cell cell = cells[0, 0];	//Gets the cell at "A1"

[Visual Basic]

Dim cells As Cells =  excel.WorkSheets(0).Cells
Dim cell As Cell =  cells(0,0)  'Gets the cell at "A1"
```

### انظر أيضًا

* class [WebCell](../../webcell/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## WebCells indexer (2 of 2)

يحصل على عنصر Cell عند اسم الخلية المحدد.

```csharp
public WebCell this[string cellName] { get; }
```

| معامل | الوصف |
| --- | --- |
| cellName | اسم الخلية، بما في ذلك حرف العمود ورقم الصف، على سبيل المثال A5. |

### قيمة الإرجاع

كائن Cell

### أمثلة

```csharp
[C#]

Cells cells = excel.Worksheets[0].Cells;
Cell cell = cells["A1"];	//Gets the cell at "A1"

[Visual Basic]

Dim cells As Cells =  excel.Worksheets(0).Cells
Dim cell As Cell =  cells("A1")  'Gets the cell at "A1"
```

### انظر أيضًا

* class [WebCell](../../webcell/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


