---
title: "RevisionCustomView"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет запись ревизии добавления или удаления пользовательского представления в книгу"
type: docs
url: /ru/java/com.aspose.cells/revisioncustomview/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionCustomView extends Revision
```

Представляет запись ревизии добавления или удаления пользовательского представления в книгу
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActionType()](#getActionType--) | Получает тип действия. |
| [getClass()](#getClass--) |  |
| [getGuid()](#getGuid--) | Получает глобальный уникальный идентификатор пользовательского представления. |
| [getId()](#getId--) | Получает номер этой ревизии. |
| [getType()](#getType--) | Получает тип ревизии. |
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
### getActionType() {#getActionType--}
```
public int getActionType()
```


Получает тип действия.

Смотрите [RevisionActionType](../../com.aspose.cells/revisionactiontype).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getGuid() {#getGuid--}
```
public UUID getGuid()
```


Получает глобальный уникальный идентификатор пользовательского представления.

**Returns:**
java.util.UUID
### getId() {#getId--}
```
public int getId()
```


Получает номер этой ревизии.

**Remarks**

Ноль означает, что эта ревизия не содержит идентификатор.

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

