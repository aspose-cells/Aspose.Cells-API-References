---
title: "Delegat CellEventHandler"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Stellt die Schnittstelle dar, die Zellenereignisse behandeln soll."
type: docs
url: /de/net/aspose.cells.gridweb.data/celleventhandler/
---
## CellEventHandler delegate

Stellt die Schnittstelle dar, die dazu bestimmt ist, Zellereignisse zu verarbeiten.

void **handleCellEvent**(Object sender, CellEventArgs e);

```csharp
public delegate void CellEventHandler(object sender, CellEventArgs e);
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sender | Object | Das Quell‑Raster des Ereignisses. |
| e | CellEventArgs | Das Ereignisargument. Das e.Cell ist die Zelle, die das Ereignis auslöst. Das e.Argument enthält das Argument des Ereignisses. |

### Siehe auch

* class [CellEventArgs](../../aspose.cells.gridweb/celleventargs/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


