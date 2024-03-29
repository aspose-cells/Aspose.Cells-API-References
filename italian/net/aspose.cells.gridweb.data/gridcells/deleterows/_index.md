---
title: DeleteRows
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Elimina diverse righe.
type: docs
weight: 360
url: /it/net/aspose.cells.gridweb.data/gridcells/deleterows/
---
## DeleteRows(int, int) {#deleterows}

Elimina diverse righe.

```csharp
public bool DeleteRows(int rowIndex, int totalRows)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | Int32 | Il primo indice di riga da eliminare. |
| totalRows | Int32 | Numero di righe da eliminare. |

### Osservazioni

Se l'intervallo eliminato contiene la parte superiore (non intera) della tabella (ListObject), l'intervallo non può essere eliminato e non verrà eseguito nulla. Funziona come MS Excel.

### Guarda anche

* class [GridCells](../../gridcells)
* spazio dei nomi [Aspose.Cells.GridWeb.Data](../../gridcells)
* assemblea [Aspose.Cells.GridWeb](../../../)

---

## DeleteRows(int, int, bool) {#deleterows_1}

Elimina più righe nel foglio di lavoro.

```csharp
public bool DeleteRows(int rowIndex, int totalRows, bool updateReference)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | Int32 | Indice di riga. |
| totalRows | Int32 | Numero di righe da eliminare. |
| updateReference | Boolean | Indica se aggiornare i riferimenti in altri fogli di lavoro. |

### Guarda anche

* class [GridCells](../../gridcells)
* spazio dei nomi [Aspose.Cells.GridWeb.Data](../../gridcells)
* assemblea [Aspose.Cells.GridWeb](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
