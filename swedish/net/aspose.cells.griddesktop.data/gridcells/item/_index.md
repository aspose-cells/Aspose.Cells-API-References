---
title: "GridCells.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridCells-egenskap. Hämtar GridCell-elementet på det angivna cellradindexet och kolumnindexet"
type: docs
url: /sv/net/aspose.cells.griddesktop.data/gridcells/item/
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

Cells cells = excel.Worksheets[0].Cells;
Cell cell = cells[0, 0];	//Gets the cell at "A1"

[Visual Basic]

Dim cells As Cells =  excel.WorkSheets(0).Cells
Dim cell As Cell =  cells(0,0)  'Gets the cell at "A1"
```

### Se även

* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

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

### Se även

* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


