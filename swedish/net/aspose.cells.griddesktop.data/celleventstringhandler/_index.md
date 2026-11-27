---
title: "Delegat CellEventStringHandler"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Representerar metoden som är avsedd att hantera cellhändelser. samma som CellEventHandler interface men returnerar ett strängresultat"
type: docs
url: /sv/net/aspose.cells.griddesktop.data/celleventstringhandler/
---
## CellEventStringHandler delegate

Representerar metoden som är avsedd att hantera cellhändelser. samma som CellEventHandler-gränssnittet, men returnerar ett strängresultat

String **handleCellEvent**(Object sender, CellEventArgs e);

```csharp
public delegate string CellEventStringHandler(object sender, CellEventArgs e);
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sender | Object | Källrutnätet för händelsen. |
| e | CellEventArgs | Händelseargumentet. e.Cell är cellen som utlöser händelsen. e.Argument innehåller argumentet för händelsen. |

### Returvärde

string värde

### Se även

* class [CellEventArgs](../../aspose.cells.griddesktop/celleventargs/)
* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


