---
title: "Delegato CellEventHandler"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Rappresenta l'interfaccia che intende gestire gli eventi delle celle"
type: docs
url: /it/net/aspose.cells.griddesktop.data/celleventhandler/
---
## CellEventHandler delegate

Rappresenta l'interfaccia che intende gestire gli eventi delle celle.

void **handleCellEvent**(Object sender, CellEventArgs e);

```csharp
public delegate void CellEventHandler(object sender, CellEventArgs e);
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sender | Object | La griglia di origine dell'evento. |
| e | CellEventArgs | L'argomento dell'evento. e.Cell è la cella che genera l'evento. e.Argument contiene l'argomento dell'evento. |

### Vedi anche

* class [CellEventArgs](../../aspose.cells.griddesktop/celleventargs/)
* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


