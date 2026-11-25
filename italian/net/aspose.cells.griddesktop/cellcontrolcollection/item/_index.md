---
title: "CellControlCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CellControlCollection. Ottiene il controllo cella all'indice di riga e colonna specificato"
type: docs
url: /it/net/aspose.cells.griddesktop/cellcontrolcollection/item/
---
## CellControlCollection indexer (1 of 2)

Ottiene il controllo cella all'indice di riga e colonna specificato.

```csharp
public CellControl this[int row, int col] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| riga | indice della riga. |
| col | indice colonna. |

### Osservazioni

Se non esiste un oggetto CellControl all'indice di riga e colonna specificato, questo controllerà l'oggetto CellControl della colonna.

### Vedi anche

* class [CellControl](../../cellcontrol/)
* class [CellControlCollection](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## CellControlCollection indexer (2 of 2)

Ottiene il controllo cella per il nome cella specificato.

```csharp
public CellControl this[string cellName] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| cellName | nome cella (nel formato nome di Excel, come 'A1', 'F22') |

### Osservazioni

Se non esiste un oggetto CellControl all'indice di riga e colonna specificato, questo controllerà l'oggetto CellControl della colonna.

### Vedi anche

* class [CellControl](../../cellcontrol/)
* class [CellControlCollection](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


