---
title: "GridCells.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية GridCells. تحصل على عنصر GridCell في فهرس الصف والعمود المحددين للخلية"
type: docs
url: /ar/net/aspose.cells.griddesktop.data/gridcells/item/
---
## GridCells indexer (1 of 2)

يحصل على عنصر [`GridCell`](../../gridcell/) في فهرس الصف والعمود المحددين للخلية.

```csharp
public GridCell this[int row, int column] { get; }
```

| معامل | الوصف |
| --- | --- |
| صف | فهرس الصف. |
| عمود | فهرس العمود. |

### قيمة الإرجاع

كائن [`GridCell`](../../gridcell/).

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

* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## GridCells indexer (2 of 2)

يحصل على عنصر [`GridCell`](../../gridcell/) بالاسم المحدد للخلية.

```csharp
public GridCell this[string cellName] { get; }
```

| معامل | الوصف |
| --- | --- |
| cellName | اسم الخلية، بما في ذلك حرف العمود ورقم الصف، على سبيل المثال A5. |

### قيمة الإرجاع

كائن [`GridCell`](../../gridcell/)

### انظر أيضًا

* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


