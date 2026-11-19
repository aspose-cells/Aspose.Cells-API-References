---
title: "CellErrorHandler"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente l'interface qui a pour but de gérer les événements d'erreur de cellule."
type: docs
url: /fr/java/com.aspose.gridweb/cellerrorhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface CellErrorHandler extends Serializable
```

Représente l'interface qui a pour but de gérer les événements d'erreur de cellule.
## Méthodes

| Méthode | Description |
| --- | --- |
| [handleCellEvent(Object sender, GridCellException ex, OnErrorActionQuery query)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.GridCellException-com.aspose.gridweb.OnErrorActionQuery-) | gérer l'événement Cell associé. |
### handleCellEvent(Object sender, GridCellException ex, OnErrorActionQuery query) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.GridCellException-com.aspose.gridweb.OnErrorActionQuery-}
```
public abstract void handleCellEvent(Object sender, GridCellException ex, OnErrorActionQuery query)
```


gérer l'événement Cell associé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sender | java.lang.Object | La source de l'événement. |
| ex | [GridCellException](../../com.aspose.gridweb/gridcellexception) | L'erreur d'opération de cellule. |
| query | [OnErrorActionQuery](../../com.aspose.gridweb/onerroractionquery) | peut obtenir des informations sur le type d'action onerror. |

