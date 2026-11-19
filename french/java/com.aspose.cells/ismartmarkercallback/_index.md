---
title: "ISmartMarkerCallBack"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente l'interface de rappel du traitement de smartmarker."
type: docs
url: /fr/java/com.aspose.cells/ismartmarkercallback/
---
```
public interface ISmartMarkerCallBack
```

Représente l'interface de rappel du traitement de smartmarker.
## Méthodes

| Méthode | Description |
| --- | --- |
| [process(int sheetIndex, int rowIndex, int colIndex, String tableName, String columnName)](#process-int-int-int-java.lang.String-java.lang.String-) | Rappel pour le traitement d’un smart marker. |
### process(int sheetIndex, int rowIndex, int colIndex, String tableName, String columnName) {#process-int-int-int-java.lang.String-java.lang.String-}
```
public abstract void process(int sheetIndex, int rowIndex, int colIndex, String tableName, String columnName)
```


Rappel pour le traitement d’un smart marker.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheetIndex | int | L’indice de la feuille. |
| rowIndex | int | L'index de ligne. |
| colIndex | int | L'index de colonne. |
| tableName | java.lang.String | Le nom de la table du smartmarker. |
| columnName | java.lang.String | Le nom de la table du smartmarker. |

