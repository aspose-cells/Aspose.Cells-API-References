---
title: "MultipleFilterCollection"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет коллекцию множественных фильтров."
type: docs
url: /ru/java/com.aspose.cells/multiplefiltercollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class MultipleFilterCollection implements Iterable
```

Представляет коллекцию множественных фильтров.

**Remarks**

ПРИМЕЧАНИЕ: Этот класс теперь устарел. Вместо него, пожалуйста, используйте [FilterValueCollection](../../com.aspose.cells/filtervaluecollection). Это свойство будет удалено через 12 месяцев, начиная с июня 2026 года. Aspose приносит извинения за любые причинённые неудобства.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [MultipleFilterCollection()](#MultipleFilterCollection--) | Создаёт один новый экземпляр. |
## Методы

| Метод | Описание |
| --- | --- |
| [add(int type, int year, int month, int day)](#add-int-int-int-int-) | Добавляет значение критерия фильтра даты. |
| [add(int type, int year, int month, int day, int hour, int minute, int second)](#add-int-int-int-int-int-int-int-) | Добавляет значение критерия фильтра даты и времени. |
| [add(String filter)](#add-java.lang.String-) | Добавляет критерий фильтра метки. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Получает [DateTimeGroupItem](../../com.aspose.cells/datetimegroupitem) или строковое значение. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Получает количество значений фильтра. |
| [getMatchBlank()](#getMatchBlank--) | Указывает, следует ли фильтровать пустые значения. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Получить перечислитель для значения фильтра, |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setMatchBlank(boolean value)](#setMatchBlank-boolean-) | Указывает, следует ли фильтровать пустые значения. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### MultipleFilterCollection() {#MultipleFilterCollection--}
```
public MultipleFilterCollection()
```


Создаёт один новый экземпляр.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, установите FilterColumn.FilterType как FilterType.MultipleFilters, затем получите FilterColumn.MultipleFilters. Это свойство будет удалено через 12 месяцев, начиная с июня 2026 года. Aspose приносит извинения за любые причинённые неудобства.

### add(int type, int year, int month, int day) {#add-int-int-int-int-}
```
public void add(int type, int year, int month, int day)
```


Добавляет значение критерия фильтра даты.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). Тип фильтра даты. |
| год | int | Год. |
| месяц | int | Месяц. |
| день | int | День. |

### add(int type, int year, int month, int day, int hour, int minute, int second) {#add-int-int-int-int-int-int-int-}
```
public void add(int type, int year, int month, int day, int hour, int minute, int second)
```


Добавляет значение критерия фильтра даты и времени.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). Тип фильтра даты. |
| год | int | Год. |
| месяц | int | Месяц. |
| день | int | День. |
| час | int | Час. |
| минута | int | Минута. |
| секунда | int | Секунда. |

### add(String filter) {#add-java.lang.String-}
```
public void add(String filter)
```


Добавляет критерий фильтра метки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| фильтр | java.lang.String | Данные фильтра. |

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
### get(int index) {#get-int-}
```
public Object get(int index)
```


Получает [DateTimeGroupItem](../../com.aspose.cells/datetimegroupitem) или строковое значение.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int |  |

**Returns:**
java.lang.Object - 
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Получает количество значений фильтра.

**Returns:**
int
### getMatchBlank() {#getMatchBlank--}
```
public boolean getMatchBlank()
```


Указывает, следует ли фильтровать пустые значения.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### iterator() {#iterator--}
```
public Iterator iterator()
```


Получить перечислитель для значения фильтра,

**Returns:**
java.util.Iterator -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setMatchBlank(boolean value) {#setMatchBlank-boolean-}
```
public void setMatchBlank(boolean value)
```


Указывает, следует ли фильтровать пустые значения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

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

