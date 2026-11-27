---
title: "Delegate CellErrorHandler"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Representerar gränssnittet som är avsett att hantera cellfelshändelser"
type: docs
url: /sv/net/aspose.cells.gridweb.data/cellerrorhandler/
---
## CellErrorHandler delegate

Representerar gränssnittet som är avsett att hantera cellfelshändelser.

void **handleCellEvent**(Object avsändare, GridCellException ex, OnErrorActionQuery query);

```csharp
public delegate void CellErrorHandler(object sender, WebCellException ex, 
    OnErrorActionQuery action);
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sender | Object | Källan till händelsen. |
| ex | WebCellException | Cellens operationsfel. |
| åtgärd | OnErrorActionQuery | kan hämta information om onerror‑åtgärdstyp. |

### Se även

* class [WebCellException](../webcellexception/)
* class [OnErrorActionQuery](../onerroractionquery/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


