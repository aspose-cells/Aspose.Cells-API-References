---
title: "RowColumnEventHandler"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Schnittstelle dar, die dazu gedacht ist, Zeilen-/Spaltenereignisse zu behandeln."
type: docs
url: /de/java/com.aspose.gridweb/rowcolumneventhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface RowColumnEventHandler extends Serializable
```

Stellt die Schnittstelle dar, die dazu gedacht ist, Zeilen-/Spaltenereignisse zu behandeln.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [handleCellEvent(Object sender, RowColumnEventArgs e)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.RowColumnEventArgs-) | Verarbeiten Sie das zugehörige Zellenereignis. |
### handleCellEvent(Object sender, RowColumnEventArgs e) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.RowColumnEventArgs-}
```
public abstract void handleCellEvent(Object sender, RowColumnEventArgs e)
```


Verarbeiten Sie das zugehörige Zellenereignis.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sender | java.lang.Object | Die Quelle des Ereignisses. |
| e | [RowColumnEventArgs](../../com.aspose.gridweb/rowcolumneventargs) | Das Ereignisargument. Rufen Sie e.RejectOperation() auf, wenn Sie den Löschvorgang in den RowDeleting- oder ColumnDeleting-Ereignishandlern abbrechen möchten. |

