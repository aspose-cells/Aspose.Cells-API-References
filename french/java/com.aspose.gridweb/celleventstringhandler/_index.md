---
title: "CellEventStringHandler"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente l'interface qui a pour but de gérer les événements de cellule."
type: docs
url: /fr/java/com.aspose.gridweb/celleventstringhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface CellEventStringHandler extends Serializable
```

Représente l'interface qui a pour but de gérer les événements de cellule.
## Méthodes

| Méthode | Description |
| --- | --- |
| [handleCellEvent(Object sender, CellEventArgs e)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-) | gérer l'événement Cell associé. |
### handleCellEvent(Object sender, CellEventArgs e) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-}
```
public abstract String handleCellEvent(Object sender, CellEventArgs e)
```


gérer l'événement Cell associé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sender | java.lang.Object | La grille source de l'événement. |
| e | [CellEventArgs](../../com.aspose.gridweb/celleventargs) | L'argument de l'événement. e.Cell est la cellule qui déclenche l'événement. e.Argument contient l'argument de l'événement. |

**Returns:**
java.lang.String - valeur de chaîne
