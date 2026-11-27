---
title: "Delegate RowColumnEventHandler"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Representerar gränssnittet som är avsett att hantera rad-/kolumnhändelser"
type: docs
url: /sv/net/aspose.cells.gridweb.data/rowcolumneventhandler/
---
## RowColumnEventHandler delegate

Representerar gränssnittet som avser att hantera rad-/kolumnhändelser.

void **handleCellEvent**(Object sender, RowColumnEventArgs e);

```csharp
public delegate void RowColumnEventHandler(object sender, RowColumnEventArgs e);
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sender | Object | Källan till händelsen. |
| e | RowColumnEventArgs | Argumentet för händelsen. Anropa e.RejectOperation() om du vill avbryta raderingsoperationen i händelsehanterarna RowDeleting eller ColumnDeleting. |

### Se även

* class [RowColumnEventArgs](../../aspose.cells.gridweb/rowcolumneventargs/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


