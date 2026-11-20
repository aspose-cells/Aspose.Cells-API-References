---
title: "LoadDataFilterOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет параметры фильтрации данных при загрузке книги из шаблона."
type: docs
url: /ru/java/com.aspose.cells/loaddatafilteroptions/
---

**Inheritance:**
java.lang.Object
```
public final class LoadDataFilterOptions
```

Представляет параметры фильтрации данных при загрузке книги из шаблона.
## Поля

| Поле | Описание |
| --- | --- |
| [ALL](#ALL) | Загрузить всё |
| [BOOK_SETTINGS](#BOOK-SETTINGS) | Загрузить настройки книги |
| [CELL_BLANK](#CELL-BLANK) | Загрузить ячейки, значение которых пусто |
| [CELL_BOOL](#CELL-BOOL) | Загрузить ячейки, значение которых является логическим |
| [CELL_DATA](#CELL-DATA) | Загрузить данные ячеек, включая значения, формулы и форматирование |
| [CELL_ERROR](#CELL-ERROR) | Загрузить ячейки, значение которых является ошибкой |
| [CELL_NUMERIC](#CELL-NUMERIC) | Загрузить ячейки, значение которых числовое(включая дату и время) |
| [CELL_STRING](#CELL-STRING) | Загрузить ячейки, значение которых строковое |
| [CELL_VALUE](#CELL-VALUE) | Загрузить только значения ячеек (все типы значений) |
| [CHART](#CHART) | Загрузить диаграммы |
| [CONDITIONAL_FORMATTING](#CONDITIONAL-FORMATTING) | Загрузить условное форматирование |
| [DATA_VALIDATION](#DATA-VALIDATION) | Загрузить проверки данных |
| [DEFINED_NAMES](#DEFINED-NAMES) | Загрузить объекты определённых имён |
| [DOCUMENT_PROPERTIES](#DOCUMENT-PROPERTIES) | Загрузить свойства документа |
| [DRAWING](#DRAWING) | Графические объекты(включая диаграмму, изображение, OleObject и все остальные графические объекты) |
| [FORMULA](#FORMULA) | Загрузить формулы ячеек. |
| [HYPERLINKS](#HYPERLINKS) | Загрузить гиперссылки |
| [MERGED_AREA](#MERGED-AREA) | Загрузить объединённые ячейки |
| [NONE](#NONE) | Не загружать данные листа |
| [OLE_OBJECT](#OLE-OBJECT) | Загрузить OleObject |
| [PICTURE](#PICTURE) | Загрузить изображения |
| [PIVOT_TABLE](#PIVOT-TABLE) | Загрузить сводные таблицы |
| [REVISION](#REVISION) | Загрузить журналы изменений |
| [SETTINGS](#SETTINGS) | Загрузить настройки книги и листа |
| [SHAPE](#SHAPE) | Загрузить фигуры |
| [SHEET_DATA](#SHEET-DATA) | Загрузить все данные листа, такие как данные ячеек, настройки, объекты и т.д. |
| [SHEET_SETTINGS](#SHEET-SETTINGS) | Загрузить настройки листа |
| [STRUCTURE](#STRUCTURE) | Загрузить структуру книги |
| [STYLE](#STYLE) | Загрузить стили форматирования ячеек |
| [TABLE](#TABLE) | Загрузить таблицы |
| [VBA](#VBA) | Загрузить проекты VBA |
| [XML_MAP](#XML-MAP) | Загрузить XmlMap |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ALL {#ALL}
```
public static final int ALL
```


Загрузить всё

### BOOK_SETTINGS {#BOOK-SETTINGS}
```
public static final int BOOK_SETTINGS
```


Загрузить настройки книги

### CELL_BLANK {#CELL-BLANK}
```
public static final int CELL_BLANK
```


Загрузить ячейки, значение которых пусто

### CELL_BOOL {#CELL-BOOL}
```
public static final int CELL_BOOL
```


Загрузить ячейки, значение которых является логическим

### CELL_DATA {#CELL-DATA}
```
public static final int CELL_DATA
```


Загрузить данные ячеек, включая значения, формулы и форматирование

### CELL_ERROR {#CELL-ERROR}
```
public static final int CELL_ERROR
```


Загрузить ячейки, значение которых является ошибкой

### CELL_NUMERIC {#CELL-NUMERIC}
```
public static final int CELL_NUMERIC
```


Загрузить ячейки, значение которых числовое(включая дату и время)

### CELL_STRING {#CELL-STRING}
```
public static final int CELL_STRING
```


Загрузить ячейки, значение которых строковое

### CELL_VALUE {#CELL-VALUE}
```
public static final int CELL_VALUE
```


Загрузить только значения ячеек (все типы значений)

### CHART {#CHART}
```
public static final int CHART
```


Загрузить диаграммы

### CONDITIONAL_FORMATTING {#CONDITIONAL-FORMATTING}
```
public static final int CONDITIONAL_FORMATTING
```


Загрузить условное форматирование

### DATA_VALIDATION {#DATA-VALIDATION}
```
public static final int DATA_VALIDATION
```


Загрузить проверки данных

### DEFINED_NAMES {#DEFINED-NAMES}
```
public static final int DEFINED_NAMES
```


Загрузить объекты определённых имён

### DOCUMENT_PROPERTIES {#DOCUMENT-PROPERTIES}
```
public static final int DOCUMENT_PROPERTIES
```


Загрузить свойства документа

### DRAWING {#DRAWING}
```
public static final int DRAWING
```


Графические объекты(включая диаграмму, изображение, OleObject и все остальные графические объекты)

### FORMULA {#FORMULA}
```
public static final int FORMULA
```


Загрузить формулы ячеек.

**Remarks**

Обычно определённые объекты Name (DefinedNames) также необходимо загружать при загрузке формул, поскольку они могут использоваться в формулах. Поэтому параметр Formula или CellData должен работать совместно с параметром DefinedNames (Formula\\|DefinedNames или CellData\\|DefinedNames) в большинстве сценариев.

### HYPERLINKS {#HYPERLINKS}
```
public static final int HYPERLINKS
```


Загрузить гиперссылки

### MERGED_AREA {#MERGED-AREA}
```
public static final int MERGED_AREA
```


Загрузить объединённые ячейки

### NONE {#NONE}
```
public static final int NONE
```


Не загружать данные листа

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел, используйте Structure вместо него. Это свойство будет удалено через 12 месяцев, начиная с декабря 2017 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### OLE_OBJECT {#OLE-OBJECT}
```
public static final int OLE_OBJECT
```


Загрузить OleObject

### PICTURE {#PICTURE}
```
public static final int PICTURE
```


Загрузить изображения

### PIVOT_TABLE {#PIVOT-TABLE}
```
public static final int PIVOT_TABLE
```


Загрузить сводные таблицы

### REVISION {#REVISION}
```
public static final int REVISION
```


Загрузить журналы изменений

### SETTINGS {#SETTINGS}
```
public static final int SETTINGS
```


Загрузить настройки книги и листа

### SHAPE {#SHAPE}
```
public static final int SHAPE
```


Загрузить фигуры

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел, используйте Drawing вместо него. Это свойство будет удалено через 12 месяцев, начиная с ноября 2019 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### SHEET_DATA {#SHEET-DATA}
```
public static final int SHEET_DATA
```


Загрузить все данные листа, такие как данные ячеек, настройки, объекты и т.д.

### SHEET_SETTINGS {#SHEET-SETTINGS}
```
public static final int SHEET_SETTINGS
```


Загрузить настройки листа

### STRUCTURE {#STRUCTURE}
```
public static final int STRUCTURE
```


Загрузить структуру книги

### STYLE {#STYLE}
```
public static final int STYLE
```


Загрузить стили форматирования ячеек

### TABLE {#TABLE}
```
public static final int TABLE
```


Загрузить таблицы

### VBA {#VBA}
```
public static final int VBA
```


Загрузить проекты VBA

### XML_MAP {#XML-MAP}
```
public static final int XML_MAP
```


Загрузить XmlMap

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

