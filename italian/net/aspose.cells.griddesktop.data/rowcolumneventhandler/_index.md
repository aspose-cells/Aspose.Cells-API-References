---
title: "Delegate RowColumnEventHandler"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Rappresenta l'interfaccia che intende gestire gli eventi di riga/colonna"
type: docs
url: /it/net/aspose.cells.griddesktop.data/rowcolumneventhandler/
---
## RowColumnEventHandler delegate

Rappresenta l'interfaccia che intende gestire gli eventi di riga/colonna.

void **handleCellEvent**(Object sender, RowColumnEventArgs e);

```csharp
public delegate void RowColumnEventHandler(object sender, RowColumnEventArgs e);
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sender | Object | L'origine dell'evento. |
| e | RowColumnEventArgs | L'argomento dell'evento. Chiama e.RejectOperation() se vuoi annullare l'operazione di eliminazione nei gestori di eventi RowDeleting o ColumnDeleting. |

### Vedi anche

* class [RowColumnEventArgs](../../aspose.cells.griddesktop/rowcolumneventargs/)
* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


