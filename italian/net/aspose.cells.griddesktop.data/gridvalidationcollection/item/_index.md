---
title: "GridValidationCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà GridValidationCollection. Ottiene l'elemento Hyperlink all'indice specificato."
type: docs
url: /it/net/aspose.cells.griddesktop.data/gridvalidationcollection/item/
---
## GridValidationCollection indexer (1 of 2)

Restituisce l'elemento Hyperlink all'indice specificato.

```csharp
public GridValidation this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice a base zero dell'elemento. |

### Valore di ritorno

L'elemento all'indice specificato.

### Vedi anche

* class [GridValidation](../../gridvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## GridValidationCollection indexer (2 of 2)

Ottiene l'elemento [`GridValidation`](../../gridvalidation/) nella cella specificata. Se non c'è alcuna convalida, restituisce null.

```csharp
public GridValidation this[int row, int column] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| riga | La riga della cella. |
| colonna | La colonna della cella. |

### Valore di ritorno

L'elemento all'indice specificato.

### Osservazioni

Se non esiste un oggetto di convalida all'indice di riga e colonna specificato, questo controllerà l'oggetto di convalida della colonna.

### Vedi anche

* class [GridValidation](../../gridvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


