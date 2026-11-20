---
title: "CellValueFormatStrategy"
second_title: "Справочник API Aspose.Cells for Java"
description: "Определяет, как применять стиль к значению ячейки."
type: docs
url: /ru/java/com.aspose.cells/cellvalueformatstrategy/
---

**Inheritance:**
java.lang.Object
```
public final class CellValueFormatStrategy
```

Определяет, как применять стиль к значению ячейки.
## Поля

| Поле | Описание |
| --- | --- |
| [CELL_STYLE](#CELL-STYLE) | Только отформатировано с оригинальным стилем ячейки. |
| [DISPLAY_STRING](#DISPLAY-STRING) | Получает отображаемую строку, показываемую в MS Excel. |
| [DISPLAY_STYLE](#DISPLAY-STYLE) | Отформатировано с отображаемым стилем ячейки. |
| [NONE](#NONE) | Не отформатировано. |
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
### CELL_STYLE {#CELL-STYLE}
```
public static final int CELL_STYLE
```


Только отформатировано с оригинальным стилем ячейки.

### DISPLAY_STRING {#DISPLAY-STRING}
```
public static final int DISPLAY_STRING
```


Получает отображаемую строку, показываемую в MS Excel. Основное отличие от [DISPLAY\_STYLE](../../com.aspose.cells/cellvalueformatstrategy\#DISPLAY-STYLE) заключается в том, что эта опция также учитывает влияние ширины столбца. Если ширина столбца слишком мала, чтобы полностью показать отформатированную строку, может отображаться "\#", как в MS Excel.

### DISPLAY_STYLE {#DISPLAY-STYLE}
```
public static final int DISPLAY_STYLE
```


Отформатировано с отображаемым стилем ячейки.

### NONE {#NONE}
```
public static final int NONE
```


Не отформатировано.

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

