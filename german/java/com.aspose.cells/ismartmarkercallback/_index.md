---
title: "ISmartMarkerCallBack"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Callback‑Schnittstelle für die Verarbeitung von Smartmarker dar."
type: docs
url: /de/java/com.aspose.cells/ismartmarkercallback/
---
```
public interface ISmartMarkerCallBack
```

Stellt die Callback‑Schnittstelle für die Verarbeitung von Smartmarker dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [process(int sheetIndex, int rowIndex, int colIndex, String tableName, String columnName)](#process-int-int-int-java.lang.String-java.lang.String-) | Rückruf zur Verarbeitung eines Smart‑Markers. |
### process(int sheetIndex, int rowIndex, int colIndex, String tableName, String columnName) {#process-int-int-int-java.lang.String-java.lang.String-}
```
public abstract void process(int sheetIndex, int rowIndex, int colIndex, String tableName, String columnName)
```


Rückruf zur Verarbeitung eines Smart‑Markers.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetIndex | int | Der Blattindex. |
| rowIndex | int | Der Zeilenindex. |
| colIndex | int | Der Spaltenindex. |
| tableName | java.lang.String | Der Tabellenname des Smart‑Markers. |
| columnName | java.lang.String | Der Tabellenname des Smart‑Markers. |

