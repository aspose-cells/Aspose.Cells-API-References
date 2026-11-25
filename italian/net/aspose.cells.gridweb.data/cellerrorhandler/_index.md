---
title: "Delegato CellErrorHandler"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Rappresenta l'interfaccia che intende gestire gli eventi di errore della cella"
type: docs
url: /it/net/aspose.cells.gridweb.data/cellerrorhandler/
---
## CellErrorHandler delegate

Rappresenta l'interfaccia che intende gestire gli eventi di errore della cella.

void **handleCellEvent**(Object sender, GridCellException ex, OnErrorActionQuery query);

```csharp
public delegate void CellErrorHandler(object sender, WebCellException ex, 
    OnErrorActionQuery action);
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sender | Object | L'origine dell'evento. |
| ex | WebCellException | L'errore di operazione della cella. |
| azione | OnErrorActionQuery | può ottenere informazioni sul tipo di azione onerror. |

### Vedi anche

* class [WebCellException](../webcellexception/)
* class [OnErrorActionQuery](../onerroractionquery/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


