---
title: "IFilePathProvider"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente le fournisseur de chemin de fichier exporté."
type: docs
url: /fr/java/com.aspose.cells/ifilepathprovider/
---
```
public interface IFilePathProvider
```

Représente le fournisseur de chemin de fichier exporté.
## Méthodes

| Méthode | Description |
| --- | --- |
| [getFullName(String sheetName)](#getFullName-java.lang.String-) | Obtient le chemin complet du fichier par nom de feuille de calcul lors de l'exportation séparée de la feuille de calcul en HTML. |
### getFullName(String sheetName) {#getFullName-java.lang.String-}
```
public abstract String getFullName(String sheetName)
```


Obtient le chemin complet du fichier par nom de feuille de calcul lors de l'exportation séparée de la feuille de calcul en HTML. Ainsi, les références entre les feuilles de calcul peuvent être exportées correctement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheetName | java.lang.String | Nom de la feuille de calcul |

**Returns:**
java.lang.String - le chemin complet du fichier
