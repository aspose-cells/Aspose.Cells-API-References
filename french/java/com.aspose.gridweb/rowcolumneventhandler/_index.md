---
title: "RowColumnEventHandler"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente l'interface qui a pour but de gérer les événements de ligne/colonne."
type: docs
url: /fr/java/com.aspose.gridweb/rowcolumneventhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface RowColumnEventHandler extends Serializable
```

Représente l'interface qui a pour but de gérer les événements de ligne/colonne.
## Méthodes

| Méthode | Description |
| --- | --- |
| [handleCellEvent(Object sender, RowColumnEventArgs e)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.RowColumnEventArgs-) | gérer l'événement Cell associé. |
### handleCellEvent(Object sender, RowColumnEventArgs e) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.RowColumnEventArgs-}
```
public abstract void handleCellEvent(Object sender, RowColumnEventArgs e)
```


gérer l'événement Cell associé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sender | java.lang.Object | La source de l'événement. |
| e | [RowColumnEventArgs](../../com.aspose.gridweb/rowcolumneventargs) | L'argument de l'événement. Appelez e.RejectOperation() si vous souhaitez annuler l'opération de suppression dans les gestionnaires d'événements RowDeleting ou ColumnDeleting. |

