---
title: "WebCells.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "WebCells property. Ottiene l'elemento Cell all'indice di riga e indice di colonna specificati"
type: docs
url: /it/net/aspose.cells.gridweb.data/webcells/item/
---
## WebCells indexer (1 of 2)

Ottiene l'elemento Cell all'indice di riga e indice di colonna specificati.

```csharp
public WebCell this[int row, int column] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| riga | Indice della riga. |
| colonna | Indice colonna. |

### Valore di ritorno

L'oggetto Cell.

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

* class [WebCell](../../webcell/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## WebCells indexer (2 of 2)

Ottiene l'elemento Cell al nome di cella specificato.

```csharp
public WebCell this[string cellName] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| cellName | Nome della cella, includendo la lettera della colonna e il numero della riga, ad esempio A5. |

### Valore di ritorno

Un oggetto Cell

### Esempi

```csharp
[C#]

Cells cells = excel.Worksheets[0].Cells;
Cell cell = cells["A1"];	//Gets the cell at "A1"

[Visual Basic]

Dim cells As Cells =  excel.Worksheets(0).Cells
Dim cell As Cell =  cells("A1")  'Gets the cell at "A1"
```

### Vedi anche

* class [WebCell](../../webcell/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


