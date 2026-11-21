---
title: "CellEventStringHandler"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar gränssnittet som är avsett att hantera cellhändelser."
type: docs
url: /sv/java/com.aspose.gridweb/celleventstringhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface CellEventStringHandler extends Serializable
```

Representerar gränssnittet som är avsett att hantera cellhändelser.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [handleCellEvent(Object sender, CellEventArgs e)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-) | hantera den relaterade Cell-händelsen. |
### handleCellEvent(Object sender, CellEventArgs e) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-}
```
public abstract String handleCellEvent(Object sender, CellEventArgs e)
```


hantera den relaterade Cell-händelsen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| avsändare | java.lang.Object | Källrutnätet för händelsen. |
| e | [CellEventArgs](../../com.aspose.gridweb/celleventargs) | Händelseargumentet. e.Cell är cellen som utlöser händelsen. e.Argument innehåller argumentet för händelsen. |

**Returns:**
java.lang.String - strängvärde
