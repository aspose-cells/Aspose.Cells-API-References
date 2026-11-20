---
title: "RevisionCellMove"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет запись ревизии для ячеек, которые были перемещены."
type: docs
url: /ru/java/com.aspose.cells/revisioncellmove/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionCellMove extends Revision
```

Представляет запись ревизии перемещения ячейки(й).
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDestinationArea()](#getDestinationArea--) | Получает целевую область. |
| [getId()](#getId--) | Получает номер этой ревизии. |
| [getSourceArea()](#getSourceArea--) | Получает исходную область. |
| [getSourceWorksheet()](#getSourceWorksheet--) | Получает исходный лист. |
| [getType()](#getType--) | Представляет тип ревизии. |
| [getWorksheet()](#getWorksheet--) | Получает рабочий лист. |
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
### getDestinationArea() {#getDestinationArea--}
```
public CellArea getDestinationArea()
```


Получает целевую область.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getId() {#getId--}
```
public int getId()
```


Получает номер этой ревизии.

**Remarks**

Ноль означает, что эта ревизия не содержит идентификатор.

**Returns:**
int
### getSourceArea() {#getSourceArea--}
```
public CellArea getSourceArea()
```


Получает исходную область.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getSourceWorksheet() {#getSourceWorksheet--}
```
public Worksheet getSourceWorksheet()
```


Получает исходный лист.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### getType() {#getType--}
```
public int getType()
```


Представляет тип ревизии.

Смотрите [RevisionType](../../com.aspose.cells/revisiontype).

**Returns:**
int
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Получает рабочий лист.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
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

