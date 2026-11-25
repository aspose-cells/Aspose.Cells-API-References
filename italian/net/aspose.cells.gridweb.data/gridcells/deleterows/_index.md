---
title: "GridCells.DeleteRows"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GridCells. Elimina diverse righe"
type: docs
url: /it/net/aspose.cells.gridweb.data/gridcells/deleterows/
---
## DeleteRows(int, int) {#deleterows}

Elimina diverse righe.

```csharp
public bool DeleteRows(int rowIndex, int totalRows)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | Int32 | L'indice della prima riga da eliminare. |
| totalRows | Int32 | Numero di righe da eliminare. |

### Osservazioni

Se l'intervallo eliminato contiene la parte superiore (non l'intera) della tabella (ListObject), l'intervallo non può essere eliminato e non verrà eseguita alcuna operazione. Funziona come MS Excel.

### Vedi anche

* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## DeleteRows(int, int, bool) {#deleterows_1}

Elimina più righe nel foglio di lavoro.

```csharp
public bool DeleteRows(int rowIndex, int totalRows, bool updateReference)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | Int32 | Indice della riga. |
| totalRows | Int32 | Numero di righe da eliminare. |
| updateReference | Booleano | Indica se aggiornare i riferimenti in altri fogli di lavoro. |

### Vedi anche

* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


