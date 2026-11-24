---
title: "Delegate CellErrorHandler"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Stellt die Schnittstelle dar, die dazu gedacht ist, Zellfehlerereignisse zu behandeln"
type: docs
url: /de/net/aspose.cells.gridweb.data/cellerrorhandler/
---
## CellErrorHandler delegate

Stellt die Schnittstelle dar, die dazu bestimmt ist, Zellfehlerereignisse zu behandeln.

void **handleCellEvent**(Object sender, GridCellException ex, OnErrorActionQuery query);

```csharp
public delegate void CellErrorHandler(object sender, WebCellException ex, 
    OnErrorActionQuery action);
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sender | Object | Die Quelle des Ereignisses. |
| ex | WebCellException | Der Zellvorgangsfehler. |
| Aktion | OnErrorActionQuery | Kann Informationen zum OnError-Aktionstyp abrufen. |

### Siehe auch

* class [WebCellException](../webcellexception/)
* class [OnErrorActionQuery](../onerroractionquery/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


