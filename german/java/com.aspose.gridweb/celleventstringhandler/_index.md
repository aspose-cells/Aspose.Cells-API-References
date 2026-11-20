---
title: "CellEventStringHandler"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Schnittstelle dar, die dazu gedacht ist, Zelleereignisse zu behandeln."
type: docs
url: /de/java/com.aspose.gridweb/celleventstringhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface CellEventStringHandler extends Serializable
```

Stellt die Schnittstelle dar, die dazu gedacht ist, Zelleereignisse zu behandeln.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [handleCellEvent(Object sender, CellEventArgs e)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-) | Verarbeiten Sie das zugehörige Zellenereignis. |
### handleCellEvent(Object sender, CellEventArgs e) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-}
```
public abstract String handleCellEvent(Object sender, CellEventArgs e)
```


Verarbeiten Sie das zugehörige Zellenereignis.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sender | java.lang.Object | Das Quellraster des Ereignisses. |
| e | [CellEventArgs](../../com.aspose.gridweb/celleventargs) | Das Ereignisargument. e.Cell ist die Zelle, die das Ereignis auslöst. e.Argument enthält das Argument des Ereignisses. |

**Returns:**
java.lang.String - Zeichenkettenwert
