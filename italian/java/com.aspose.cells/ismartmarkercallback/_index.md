---
title: "ISmartMarkerCallBack"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta l'interfaccia di callback dell'elaborazione di smartmarker."
type: docs
url: /it/java/com.aspose.cells/ismartmarkercallback/
---
```
public interface ISmartMarkerCallBack
```

Rappresenta l'interfaccia di callback dell'elaborazione di smartmarker.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [process(int sheetIndex, int rowIndex, int colIndex, String tableName, String columnName)](#process-int-int-int-java.lang.String-java.lang.String-) | Callback per l'elaborazione di uno smart marker. |
### process(int sheetIndex, int rowIndex, int colIndex, String tableName, String columnName) {#process-int-int-int-java.lang.String-java.lang.String-}
```
public abstract void process(int sheetIndex, int rowIndex, int colIndex, String tableName, String columnName)
```


Callback per l'elaborazione di uno smart marker.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetIndex | int | L'indice del foglio. |
| rowIndex | int | L'indice della riga. |
| colIndex | int | L'indice della colonna. |
| tableName | java.lang.String | Il nome della tabella dello smartmarker. |
| columnName | java.lang.String | Il nome della tabella dello smartmarker. |

