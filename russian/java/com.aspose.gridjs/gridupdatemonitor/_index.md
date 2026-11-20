---
title: "GridUpdateMonitor"
second_title: "Справочник API Aspose.Cells for Java"
description: "Монитор для пользователя, отслеживающий изменения операции обновления."
type: docs
url: /ru/java/com.aspose.gridjs/gridupdatemonitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class GridUpdateMonitor
```

Монитор для пользователя, отслеживающий изменения операции обновления.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [GridUpdateMonitor()](#GridUpdateMonitor--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [afterUpdate(String op, String uid, ArrayList cells)](#afterUpdate-java.lang.String-java.lang.String-java.util.ArrayList-) | после операции обновления |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridUpdateMonitor() {#GridUpdateMonitor--}
```
public GridUpdateMonitor()
```


### afterUpdate(String op, String uid, ArrayList cells) {#afterUpdate-java.lang.String-java.lang.String-java.util.ArrayList-}
```
public abstract void afterUpdate(String op, String uid, ArrayList cells)
```


после операции обновления

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| op | java.lang.String | JSON-строка для операции обновления |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |
| cells | java.util.ArrayList | Обновлённый список ячеек, включающий ячейки, у которых изменён стиль, значение или формула |

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

