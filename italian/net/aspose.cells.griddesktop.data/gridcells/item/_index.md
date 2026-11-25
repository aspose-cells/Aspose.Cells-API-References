---
title: "GridCells.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà GridCells. Ottiene l'elemento GridCell all'indice di riga e colonna specificati"
type: docs
url: /it/net/aspose.cells.griddesktop.data/gridcells/item/
---
## GridCells indexer (1 of 2)

Ottiene l'elemento [`GridCell`](../../gridcell/) all'indice di riga e colonna della cella specificati.

```csharp
public GridCell this[int row, int column] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| riga | Indice della riga. |
| colonna | Indice colonna. |

### Valore di ritorno

L'oggetto [`GridCell`](../../gridcell/).

### Esempi

```csharp
[C#]

Cells cells = excel.Worksheets[0].Cells;
Cell cell = cells[0, 0];	//Gets the cell at "A1"

[Visual Basic]

Dim cells As Cells =  excel.WorkSheets(0).Cells
Dim cell As Cell =  cells(0,0)  'Gets the cell at "A1"
```

### Vedi anche

* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## GridCells indexer (2 of 2)

Ottiene l'elemento [`GridCell`](../../gridcell/) al nome della cella specificato.

```csharp
public GridCell this[string cellName] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| cellName | Nome della cella, includendo la lettera della colonna e il numero della riga, ad esempio A5. |

### Valore di ritorno

Un oggetto [`GridCell`](../../gridcell/)

### Vedi anche

* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


