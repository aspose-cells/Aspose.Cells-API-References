---
title: "DataSorterKey"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет ключ сортировщика данных."
type: docs
url: /ru/java/com.aspose.cells/datasorterkey/
---

**Inheritance:**
java.lang.Object
```
public class DataSorterKey
```

Представляет ключ сортировщика данных.
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Получает отсортированный цвет. |
| [getIconId()](#getIconId--) | Представляет идентификатор типа набора иконок. |
| [getIconSetType()](#getIconSetType--) | Представляет тип набора иконок. |
| [getIndex()](#getIndex--) | Получает индекс отсортированного столбца (абсолютная позиция, столбец A — 0, B — 1, ...). |
| [getOrder()](#getOrder--) | Указывает порядок сортировки. |
| [getType()](#getType--) | Представляет тип сортировки. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getColor() {#getColor--}
```
public Color getColor()
```


Получает отсортированный цвет.

**Remarks**

Действует только когда [getType()](../../com.aspose.cells/datasorterkey\#getType--) является [SortOnType.CELL\_COLOR](../../com.aspose.cells/sortontype\#CELL-COLOR) или [SortOnType.FONT\_COLOR](../../com.aspose.cells/sortontype\#FONT-COLOR).

**Returns:**
[Color](../../com.aspose.cells/color)
### getIconId() {#getIconId--}
```
public int getIconId()
```


Представляет идентификатор типа набора иконок.

**Remarks**

Действует только когда [getType()](../../com.aspose.cells/datasorterkey\#getType--) является [SortOnType.ICON](../../com.aspose.cells/sortontype\#ICON).

**Returns:**
int
### getIconSetType() {#getIconSetType--}
```
public int getIconSetType()
```


Представляет тип набора иконок.

Смотрите [IconSetType](../../com.aspose.cells/iconsettype).

**Remarks**

Действует только когда [getType()](../../com.aspose.cells/datasorterkey\#getType--) является [SortOnType.ICON](../../com.aspose.cells/sortontype\#ICON).

**Returns:**
int
### getIndex() {#getIndex--}
```
public int getIndex()
```


Получает индекс отсортированного столбца (абсолютная позиция, столбец A — 0, B — 1, ...).

**Returns:**
int
### getOrder() {#getOrder--}
```
public int getOrder()
```


Указывает порядок сортировки.

См. [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Представляет тип сортировки.

Смотрите [SortOnType](../../com.aspose.cells/sortontype).

**Returns:**
int
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

