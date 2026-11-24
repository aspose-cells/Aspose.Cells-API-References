---
title: "GridCells.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridCells-Eigenschaft. Gibt das GridCell-Element am angegebenen Zeilen‑ und Spaltenindex zurück."
type: docs
url: /de/net/aspose.cells.gridweb.data/gridcells/item/
---
## GridCells indexer (1 of 2)

Gibt das [`GridCell`](../../gridcell/)‑Element am angegebenen Zeilen‑ und Spaltenindex zurück.

```csharp
public GridCell this[int row, int column] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| row | Zeilenindex. |
| column | Spaltenindex. |

### Rückgabewert

Das [`GridCell`](../../gridcell/)‑Objekt.

### Beispiele

```csharp
[C#]
GridWeb GridWeb1 = new GridWeb();
GridCells cells = GridWeb1.WorkSheets[0].Cells;
//Gibt die Zelle bei "A1" zurück
GridCell cell = cells[0, 0];	

[Visual Basic]

Dim cells As Cells =  excel.WorkSheets(0).Cells
 'Gets the cell at "A1"
Dim cell As Cell =  cells(0,0) 
```

### Siehe auch

* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## GridCells indexer (2 of 2)

Gibt das [`GridCell`](../../gridcell/)‑Element am angegebenen Zellenamen zurück.

```csharp
public GridCell this[string cellName] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| cellName | Zellenname, einschließlich seines Spaltenbuchstabens und seiner Zeilennummer, zum Beispiel A5. |

### Rückgabewert

Ein [`GridCell`](../../gridcell/)‑Objekt

### Beispiele

```csharp
[C#]
ridWeb GridWeb1 = new GridWeb();
 GridCells cells = GridWeb1.WorkSheets[0].Cells;
 GridCell cell = cells["A1"];	//Gets the cell at "A1"

[Visual Basic]

Dim cells As Cells =  excel.Worksheets(0).Cells
Dim cell As Cell =  cells("A1")  'Gets the cell at "A1"
```

### Siehe auch

* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


