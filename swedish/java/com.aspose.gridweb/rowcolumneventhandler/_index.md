---
title: "RowColumnEventHandler"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar gränssnittet som är avsett att hantera rad-/kolumnhändelser."
type: docs
url: /sv/java/com.aspose.gridweb/rowcolumneventhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface RowColumnEventHandler extends Serializable
```

Representerar gränssnittet som är avsett att hantera rad-/kolumnhändelser.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [handleCellEvent(Object sender, RowColumnEventArgs e)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.RowColumnEventArgs-) | hantera den relaterade Cell-händelsen. |
### handleCellEvent(Object sender, RowColumnEventArgs e) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.RowColumnEventArgs-}
```
public abstract void handleCellEvent(Object sender, RowColumnEventArgs e)
```


hantera den relaterade Cell-händelsen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| avsändare | java.lang.Object | Källan till händelsen. |
| e | [RowColumnEventArgs](../../com.aspose.gridweb/rowcolumneventargs) | Eventargumentet. Anropa e.RejectOperation() om du vill avbryta raderingsoperationen i RowDeleting- eller ColumnDeleting‑händelsehanterare. |

