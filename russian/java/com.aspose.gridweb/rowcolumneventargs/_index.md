---
title: "RowColumnEventArgs"
second_title: "Справочник API Aspose.Cells for Java"
description: "Предоставляет данные для событий строки/столбца."
type: docs
url: /ru/java/com.aspose.gridweb/rowcolumneventargs/
---

**Inheritance:**
java.lang.Object
```
public class RowColumnEventArgs
```

Предоставляет данные для событий строки/столбца.
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgument()](#getArgument--) | Аргумент события. |
| [getClass()](#getClass--) |  |
| [getNum()](#getNum--) | Номер строки или столбца, начинается с нуля. |
| [getType()](#getType--) | Тип строки или столбца. |
| [hashCode()](#hashCode--) |  |
| [isCancel()](#isCancel--) | Отменим операцию. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [rejectOperation()](#rejectOperation--) | Вызовите этот метод в обработчиках событий RowDeleting/ColumnDeleting, чтобы отменить операции удаления. |
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
### getArgument() {#getArgument--}
```
public Object getArgument()
```


Аргумент события.

**Returns:**
java.lang.Object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getNum() {#getNum--}
```
public int getNum()
```


Номер строки или столбца, начинается с нуля.

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Тип строки или столбца.

Смотрите [RowColumnType](../../com.aspose.gridweb/rowcolumntype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCancel() {#isCancel--}
```
public boolean isCancel()
```


Отменим операцию.

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




### rejectOperation() {#rejectOperation--}
```
public void rejectOperation()
```


Вызовите этот метод в обработчиках событий RowDeleting/ColumnDeleting, чтобы отменить операции удаления.

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

