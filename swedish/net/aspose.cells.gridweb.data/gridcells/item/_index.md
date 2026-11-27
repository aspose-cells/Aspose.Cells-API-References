---
title: "GridCells.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridCells-egenskap. Hämtar GridCell-elementet på det angivna cellradindexet och kolumnindexet"
type: docs
url: /sv/net/aspose.cells.gridweb.data/gridcells/item/
---
## GridCells indexer (1 of 2)

Hämtar [`GridCell`](../../gridcell/) elementet på det angivna cellradindexet och kolumnindexet.

```csharp
public GridCell this[int row, int column] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| row | Radindex. |
| column | Kolumnindex. |

### Returvärde

Det [`GridCell`](../../gridcell/) objektet.

### Exempel

```csharp
[C#]
GridWeb GridWeb1 = new GridWeb();
GridCells cells = GridWeb1.WorkSheets[0].Cells;
//Hämtar cellen på "A1"
GridCell cell = cells[0, 0];	

[Visual Basic]

Dim cells As Cells =  excel.WorkSheets(0).Cells
 'Gets the cell at "A1"
Dim cell As Cell =  cells(0,0) 
```

### Se även

* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## GridCells indexer (2 of 2)

Hämtar [`GridCell`](../../gridcell/) elementet på det angivna cellnamnet.

```csharp
public GridCell this[string cellName] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| cellName | Cellnamn, inklusive dess kolumnbokstav och radnummer, till exempel A5. |

### Returvärde

Ett [`GridCell`](../../gridcell/) objekt

### Exempel

```csharp
[C#]
ridWeb GridWeb1 = new GridWeb();
 GridCells cells = GridWeb1.WorkSheets[0].Cells;
 GridCell cell = cells["A1"];	//Gets the cell at "A1"

[Visual Basic]

Dim cells As Cells =  excel.Worksheets(0).Cells
Dim cell As Cell =  cells("A1")  'Gets the cell at "A1"
```

### Se även

* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


