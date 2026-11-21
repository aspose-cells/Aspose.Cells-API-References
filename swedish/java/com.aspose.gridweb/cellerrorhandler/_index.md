---
title: "CellErrorHandler"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar gränssnittet som är avsett att hantera cellfelshändelser."
type: docs
url: /sv/java/com.aspose.gridweb/cellerrorhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface CellErrorHandler extends Serializable
```

Representerar gränssnittet som är avsett att hantera cellfelshändelser.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [handleCellEvent(Object sender, GridCellException ex, OnErrorActionQuery query)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.GridCellException-com.aspose.gridweb.OnErrorActionQuery-) | hantera den relaterade Cell-händelsen. |
### handleCellEvent(Object sender, GridCellException ex, OnErrorActionQuery query) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.GridCellException-com.aspose.gridweb.OnErrorActionQuery-}
```
public abstract void handleCellEvent(Object sender, GridCellException ex, OnErrorActionQuery query)
```


hantera den relaterade Cell-händelsen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| avsändare | java.lang.Object | Källan till händelsen. |
| ex | [GridCellException](../../com.aspose.gridweb/gridcellexception) | Cellens operationsfel. |
| query | [OnErrorActionQuery](../../com.aspose.gridweb/onerroractionquery) | kan hämta information om onerror‑åtgärdstyp. |

