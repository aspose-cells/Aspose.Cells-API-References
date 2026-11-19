---
title: "GridCustomServerValidation"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "l'interface que vous devez implémenter lors de l'utilisation de la validation côté serveur."
type: docs
url: /fr/java/com.aspose.gridweb/gridcustomservervalidation/
---
```
public interface GridCustomServerValidation
```

l'interface que vous devez implémenter lors de l'utilisation de la validation côté serveur. CustomServerFunction.
## Méthodes

| Méthode | Description |
| --- | --- |
| [validate(GridWorksheet sheet, int row, int col, String value)](#validate-com.aspose.gridweb.GridWorksheet-int-int-java.lang.String-) | **Remarques** |
### validate(GridWorksheet sheet, int row, int col, String value) {#validate-com.aspose.gridweb.GridWorksheet-int-int-java.lang.String-}
```
public abstract String validate(GridWorksheet sheet, int row, int col, String value)
```


**Remarks**

si vous renvoyez string.empty, la validation est réussie, sinon vous pouvez retourner tout message lié qui peut être traité dans la fonction ClientCallback

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheet | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) | le GridWorksheet |
| ligne | int | l'indice de ligne de la cellule |
| col | int | l'indice de colonne de la cellule |
| valeur | java.lang.String | la valeur à valider |

**Returns:**
java.lang.String - valeur de résultat basée sur une chaîne
