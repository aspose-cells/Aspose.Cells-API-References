---
title: "GridCells.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà GridCells. Ottiene l'elemento GridCell all'indice di riga e colonna specificati"
type: docs
url: /it/net/aspose.cells.gridweb.data/gridcells/item/
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
GridWeb GridWeb1 = new GridWeb();
GridCells cells = GridWeb1.WorkSheets[0].Cells;
//Ottiene la cella in "A1"
GridCell cell = cells[0, 0];	

[Visual Basic]

Dim cells As Cells =  excel.WorkSheets(0).Cells
 'Gets the cell at "A1"
Dim cell As Cell =  cells(0,0) 
```

### Vedi anche

* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

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

### Esempi

```csharp
[C#]
ridWeb GridWeb1 = new GridWeb();
 GridCells cells = GridWeb1.WorkSheets[0].Cells;
 GridCell cell = cells["A1"];	//Gets the cell at "A1"

[Visual Basic]

Dim cells As Cells =  excel.Worksheets(0).Cells
Dim cell As Cell =  cells("A1")  'Gets the cell at "A1"
```

### Vedi anche

* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


