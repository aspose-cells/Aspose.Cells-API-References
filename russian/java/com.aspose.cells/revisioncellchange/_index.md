---
title: "RevisionCellChange"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет ревизию, изменяющую ячейки."
type: docs
url: /ru/java/com.aspose.cells/revisioncellchange/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionCellChange extends Revision
```

Представляет ревизию, изменяющую ячейки.
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellName()](#getCellName--) | Получает имя ячейки. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Получает индекс столбца ячейки. |
| [getId()](#getId--) | Получает номер этой ревизии. |
| [getNewFormula()](#getNewFormula--) | Получает старую формулу. |
| [getNewStyle()](#getNewStyle--) | Получает новый стиль ячейки. |
| [getNewValue()](#getNewValue--) | Получает новое значение ячейки. |
| [getOldFormula()](#getOldFormula--) | Получает старую формулу. |
| [getOldStyle()](#getOldStyle--) | Получает старый стиль ячейки. |
| [getOldValue()](#getOldValue--) | Получает старое значение ячейки. |
| [getRow()](#getRow--) | Получает индекс строки ячейки. |
| [getType()](#getType--) | Представляет тип ревизии. |
| [getWorksheet()](#getWorksheet--) | Получает рабочий лист. |
| [hashCode()](#hashCode--) |  |
| [isNewFormatted()](#isNewFormatted--) | Указывает, отформатирована ли эта ячейка как новая. |
| [isOldFormatted()](#isOldFormatted--) | Указывает, отформатирована ли эта ячейка как старая. |
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


Получает индекс столбца ячейки.

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
### getNewFormula() {#getNewFormula--}
```
public String getNewFormula()
```


Получает старую формулу.

**Returns:**
java.lang.String
### getNewStyle() {#getNewStyle--}
```
public Style getNewStyle()
```


Получает новый стиль ячейки.

**Returns:**
[Style](../../com.aspose.cells/style)
### getNewValue() {#getNewValue--}
```
public Object getNewValue()
```


Получает новое значение ячейки.

**Returns:**
java.lang.Object
### getOldFormula() {#getOldFormula--}
```
public String getOldFormula()
```


Получает старую формулу.

**Returns:**
java.lang.String
### getOldStyle() {#getOldStyle--}
```
public Style getOldStyle()
```


Получает старый стиль ячейки.

**Returns:**
[Style](../../com.aspose.cells/style)
### getOldValue() {#getOldValue--}
```
public Object getOldValue()
```


Получает старое значение ячейки.

**Returns:**
java.lang.Object
### getRow() {#getRow--}
```
public int getRow()
```


Получает индекс строки ячейки.

**Returns:**
int
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
### isNewFormatted() {#isNewFormatted--}
```
public boolean isNewFormatted()
```


Указывает, отформатирована ли эта ячейка как новая.

**Returns:**
boolean
### isOldFormatted() {#isOldFormatted--}
```
public boolean isOldFormatted()
```


Указывает, отформатирована ли эта ячейка как старая.

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

