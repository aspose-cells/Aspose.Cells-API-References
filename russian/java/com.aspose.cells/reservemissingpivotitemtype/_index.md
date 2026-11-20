---
title: "ReserveMissingPivotItemType"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет, как сохранять отсутствующие элементы сводной таблицы."
type: docs
url: /ru/java/com.aspose.cells/reservemissingpivotitemtype/
---

**Inheritance:**
java.lang.Object
```
public final class ReserveMissingPivotItemType
```

Представляет, как сохранять отсутствующие элементы сводной таблицы.
## Поля

| Поле | Описание |
| --- | --- |
| [ALL](#ALL) | Резервирует все отсутствующие элементы. |
| [DEFAULT](#DEFAULT) | Удаляет старые отсутствующие элементы сводки и резервирует удалённые элементы нового источника данных как отсутствующие. |
| [NONE](#NONE) | Удаляет все отсутствующие элементы сводки. |
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


Резервирует все отсутствующие элементы.

**Remarks**

В Excel, пока приложение не закрыто, отсутствующие элементы, сгенерированные при первом обновлении сводной таблицы, сохраняются, даже при многократных обновлениях.

### DEFAULT {#DEFAULT}
```
public static final int DEFAULT
```


Удаляет старые отсутствующие элементы сводки и резервирует удалённые элементы нового источника данных как отсутствующие.

### NONE {#NONE}
```
public static final int NONE
```


Удаляет все отсутствующие элементы сводки.

**Remarks**

Порядок старых отсутствующих элементов сводной таблицы будет игнорироваться.

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

