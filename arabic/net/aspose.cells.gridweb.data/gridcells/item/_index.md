---
title: "GridCells.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية GridCells. تحصل على عنصر GridCell في فهرس الصف والعمود المحددين للخلية"
type: docs
url: /ar/net/aspose.cells.gridweb.data/gridcells/item/
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
GridWeb GridWeb1 = new GridWeb();
GridCells cells = GridWeb1.WorkSheets[0].Cells;
//يحصل على الخلية في "A1"
GridCell cell = cells[0, 0];	

[Visual Basic]

Dim cells As Cells =  excel.WorkSheets(0).Cells
 'Gets the cell at "A1"
Dim cell As Cell =  cells(0,0) 
```

### انظر أيضًا

* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

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

### أمثلة

```csharp
[C#]
ridWeb GridWeb1 = new GridWeb();
 GridCells cells = GridWeb1.WorkSheets[0].Cells;
 GridCell cell = cells["A1"];	//Gets the cell at "A1"

[Visual Basic]

Dim cells As Cells =  excel.Worksheets(0).Cells
Dim cell As Cell =  cells("A1")  'Gets the cell at "A1"
```

### انظر أيضًا

* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


