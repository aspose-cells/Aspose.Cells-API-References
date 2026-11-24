---
title: "GridCells.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridCells-Eigenschaft. Gibt das GridCell-Element am angegebenen Zeilen‑ und Spaltenindex zurück."
type: docs
url: /de/net/aspose.cells.griddesktop.data/gridcells/item/
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

Cells cells = excel.Worksheets[0].Cells;
Cell cell = cells[0, 0];	//Gets the cell at "A1"

[Visual Basic]

Dim cells As Cells =  excel.WorkSheets(0).Cells
Dim cell As Cell =  cells(0,0)  'Gets the cell at "A1"
```

### Siehe auch

* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

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

### Siehe auch

* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


