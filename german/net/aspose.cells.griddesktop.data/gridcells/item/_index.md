---
title: Item
second_title: Aspose.Cells für .NET-API-Referenz
description: erhältCell Element im Arbeitsblatt
type: docs
weight: 40
url: /de/net/aspose.cells.griddesktop.data/gridcells/item/
---
## GridCells indexer (1 of 3)

erhältCell Element im Arbeitsblatt

```csharp
public GridCell this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| index | Der nullbasierte Index des Elements. |

### Eigentumswert

Das Element am angegebenen Index.

### Bemerkungen

Dies ist der Indexer für die Cells-Klasse. Ruft das Zellenelement am angegebenen Index ab.

### Siehe auch

* class [GridCell](../../gridcell)
* class [GridCells](../../gridcells)
* namensraum [Aspose.Cells.GridDesktop.Data](../../gridcells)
* Montage [Aspose.Cells.GridDesktop](../../../)

---

## GridCells indexer (2 of 3)

Ruft die abCell Element am angegebenen Zellenzeilenindex und Spaltenindex.

```csharp
public GridCell this[int row, int column] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| row | Zeilenindex. |
| column | Spaltenindex. |

### Rückgabewert

DasCell Objekt.

### Beispiele

```csharp
[C#]

Cells cells = excel.Worksheets[0].Cells;
Cell cell = cells[0, 0];	// Ruft die Zelle bei "A1" ab

[Visual Basic]

Dim cells As Cells =  excel.WorkSheets(0).Cells
Dim cell As Cell =  cells(0,0)  'Gets the cell at "A1"
```

### Siehe auch

* class [GridCell](../../gridcell)
* class [GridCells](../../gridcells)
* namensraum [Aspose.Cells.GridDesktop.Data](../../gridcells)
* Montage [Aspose.Cells.GridDesktop](../../../)

---

## GridCells indexer (3 of 3)

Ruft die abCell Element am angegebenen Zellennamen.

```csharp
public GridCell this[string cellName] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| cellName | Zellenname, einschließlich Spaltenbuchstabe und Zeilennummer, z. B. A5. |

### Rückgabewert

EINCell Objekt

### Beispiele

```csharp
[C#]

Cells cells = excel.Worksheets[0].Cells;
Cell cell = cells["A1"];	// Ruft die Zelle bei "A1" ab

[Visual Basic]

Dim cells As Cells =  excel.Worksheets(0).Cells
Dim cell As Cell =  cells("A1")  'Gets the cell at "A1"
```

### Siehe auch

* class [GridCell](../../gridcell)
* class [GridCells](../../gridcells)
* namensraum [Aspose.Cells.GridDesktop.Data](../../gridcells)
* Montage [Aspose.Cells.GridDesktop](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->