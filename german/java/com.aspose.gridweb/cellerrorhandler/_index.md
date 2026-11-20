---
title: "CellErrorHandler"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Schnittstelle dar, die dazu gedacht ist, Zellfehlerereignisse zu behandeln."
type: docs
url: /de/java/com.aspose.gridweb/cellerrorhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface CellErrorHandler extends Serializable
```

Stellt die Schnittstelle dar, die dazu gedacht ist, Zellfehlerereignisse zu behandeln.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [handleCellEvent(Object sender, GridCellException ex, OnErrorActionQuery query)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.GridCellException-com.aspose.gridweb.OnErrorActionQuery-) | Verarbeiten Sie das zugehörige Zellenereignis. |
### handleCellEvent(Object sender, GridCellException ex, OnErrorActionQuery query) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.GridCellException-com.aspose.gridweb.OnErrorActionQuery-}
```
public abstract void handleCellEvent(Object sender, GridCellException ex, OnErrorActionQuery query)
```


Verarbeiten Sie das zugehörige Zellenereignis.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sender | java.lang.Object | Die Quelle des Ereignisses. |
| ex | [GridCellException](../../com.aspose.gridweb/gridcellexception) | Der Zelloperationsfehler. |
| query | [OnErrorActionQuery](../../com.aspose.gridweb/onerroractionquery) | Kann Informationen zum onerror-Aktionstyp abrufen. |

