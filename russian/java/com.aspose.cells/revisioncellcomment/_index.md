---
title: "RevisionCellComment"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет запись ревизии изменения комментария ячейки."
type: docs
url: /ru/java/com.aspose.cells/revisioncellcomment/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionCellComment extends Revision
```

Представляет запись ревизии изменения комментария ячейки.
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActionType()](#getActionType--) | Получает тип действия ревизии. |
| [getCellName()](#getCellName--) | Получает имя ячейки. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Получает индекс столбца, который содержит комментарий. |
| [getId()](#getId--) | Получает номер этой ревизии. |
| [getNewLength()](#getNewLength--) | Получает длину комментария до внесения этой правки. |
| [getOldLength()](#getOldLength--) | Получает длину текста комментария, добавленного в этой правке. |
| [getRow()](#getRow--) | Получает индекс строки, который содержит комментарий. |
| [getType()](#getType--) | Получает тип ревизии. |
| [getWorksheet()](#getWorksheet--) | Получает рабочий лист. |
| [hashCode()](#hashCode--) |  |
| [isOldComment()](#isOldComment--) | Указывает, является ли комментарий старым. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCellName(String value)](#setCellName-java.lang.String-) | Получает имя ячейки. |
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
### getActionType() {#getActionType--}
```
public int getActionType()
```


Получает тип действия ревизии.

Смотрите [RevisionActionType](../../com.aspose.cells/revisionactiontype).

**Returns:**
int
### getCellName() {#getCellName--}
```
public String getCellName()
```


Получает имя ячейки.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```


Получает индекс столбца, который содержит комментарий.

**Returns:**
int
### getId() {#getId--}
```
public int getId()
```


Получает номер этой ревизии.

**Remarks**

Ноль означает, что эта ревизия не содержит идентификатор.

**Returns:**
int
### getNewLength() {#getNewLength--}
```
public int getNewLength()
```


Получает длину комментария до внесения этой правки.

**Returns:**
int
### getOldLength() {#getOldLength--}
```
public int getOldLength()
```


Получает длину текста комментария, добавленного в этой правке.

**Returns:**
int
### getRow() {#getRow--}
```
public int getRow()
```


Получает индекс строки, который содержит комментарий.

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Получает тип ревизии.

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
### isOldComment() {#isOldComment--}
```
public boolean isOldComment()
```


Указывает, является ли комментарий старым.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setCellName(String value) {#setCellName-java.lang.String-}
```
public void setCellName(String value)
```


Получает имя ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

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

