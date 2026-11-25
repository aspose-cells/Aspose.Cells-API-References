---
title: "Delegato CellEventStringHandler"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Rappresenta il metodo che intende gestire gli eventi di cella. stesso dell'interfaccia CellEventHandler ma restituisce un risultato stringa"
type: docs
url: /it/net/aspose.cells.gridweb.data/celleventstringhandler/
---
## CellEventStringHandler delegate

Rappresenta il metodo che intende gestire gli eventi delle celle. stesso dell'interfaccia CellEventHandler, ma restituisce un risultato stringa

String **handleCellEvent**(Object sender, CellEventArgs e);

```csharp
public delegate string CellEventStringHandler(object sender, CellEventArgs e);
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sender | Object | La griglia di origine dell'evento. |
| e | CellEventArgs | L'argomento dell'evento. e.Cell è la cella che genera l'evento. e.Argument contiene l'argomento dell'evento. |

### Valore di ritorno

valore stringa

### Vedi anche

* class [CellEventArgs](../../aspose.cells.gridweb/celleventargs/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


