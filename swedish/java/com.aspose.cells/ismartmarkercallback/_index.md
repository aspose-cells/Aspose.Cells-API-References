---
title: "ISmartMarkerCallBack"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar återuppringningsgränssnittet för bearbetning av smartmarker."
type: docs
url: /sv/java/com.aspose.cells/ismartmarkercallback/
---
```
public interface ISmartMarkerCallBack
```

Representerar återuppringningsgränssnittet för bearbetning av smartmarker.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [process(int sheetIndex, int rowIndex, int colIndex, String tableName, String columnName)](#process-int-int-int-java.lang.String-java.lang.String-) | Återanrop för bearbetning av en smart markör. |
### process(int sheetIndex, int rowIndex, int colIndex, String tableName, String columnName) {#process-int-int-int-java.lang.String-java.lang.String-}
```
public abstract void process(int sheetIndex, int rowIndex, int colIndex, String tableName, String columnName)
```


Återanrop för bearbetning av en smart markör.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetIndex | int | Bladets index. |
| rowIndex | int | Radindexet. |
| colIndex | int | Kolumnindexet. |
| tableName | java.lang.String | Tabellnamnet för smartmarkören. |
| columnName | java.lang.String | Tabellnamnet för smartmarkören. |

