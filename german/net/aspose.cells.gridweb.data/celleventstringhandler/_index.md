---
title: "Delegat CellEventStringHandler"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Stellt die Methode dar, die dazu bestimmt ist, Zellenereignisse zu behandeln. Gleich wie die CellEventHandler‑Schnittstelle, gibt jedoch einen Zeichenketten‑Ergebnis zurück."
type: docs
url: /de/net/aspose.cells.gridweb.data/celleventstringhandler/
---
## CellEventStringHandler delegate

Stellt die Methode dar, die dazu bestimmt ist, Zellereignisse zu verarbeiten. gleich wie die CellEventHandler-Schnittstelle, gibt jedoch einen Zeichenkettenwert zurück.

String **handleCellEvent**(Object sender, CellEventArgs e);

```csharp
public delegate string CellEventStringHandler(object sender, CellEventArgs e);
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sender | Object | Das Quell‑Raster des Ereignisses. |
| e | CellEventArgs | Das Ereignisargument. Das e.Cell ist die Zelle, die das Ereignis auslöst. Das e.Argument enthält das Argument des Ereignisses. |

### Rückgabewert

string-Wert

### Siehe auch

* class [CellEventArgs](../../aspose.cells.gridweb/celleventargs/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


