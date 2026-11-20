---
title: "PivotPageFields"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет элементы страницы сводки, если источник данных сводной таблицы — диапазоны консолидации."
type: docs
url: /ru/java/com.aspose.cells/pivotpagefields/
---

**Inheritance:**
java.lang.Object
```
public class PivotPageFields
```

Представляет элементы страницы сводки, если источник данных сводной таблицы — диапазоны консолидации. Может содержать не более 4 элементов.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [PivotPageFields()](#PivotPageFields--) | Представляет элементы поля страницы сводки. |
## Методы

| Метод | Описание |
| --- | --- |
| [addIdentify(int rangeIndex, int[] pageItemIndex)](#addIdentify-int-int---) | Устанавливает, какую метку элемента в каждом поле страницы использовать для идентификации диапазона данных. |
| [addPageField(String[] pageItems)](#addPageField-java.lang.String---) | Добавляет поле страницы. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPageFieldCount()](#getPageFieldCount--) | Получает количество полей страницы. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotPageFields() {#PivotPageFields--}
```
public PivotPageFields()
```


Представляет элементы поля страницы сводки.

### addIdentify(int rangeIndex, int[] pageItemIndex) {#addIdentify-int-int---}
```
public void addIdentify(int rangeIndex, int[] pageItemIndex)
```


Устанавливает, какую метку элемента в каждом поле страницы использовать для идентификации диапазона данных. Длина pageItemIndex должна быть равна PageFieldCount, поэтому сначала добавьте поле страницы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rangeIndex | int | Индекс диапазона данных консолидации. |
| pageItemIndex | int[] | Индекс элемента страницы в каждом поле страницы. pageItemIndex[2] = 1 означает, что второй элемент в третьем поле используется для идентификации этого диапазона. pageItemIndex[1] = -1 означает отсутствие элемента во втором поле для идентификации этого диапазона, и MS автоматически создаст элемент "blank" во втором поле для идентификации этого диапазона. |

### addPageField(String[] pageItems) {#addPageField-java.lang.String---}
```
public void addPageField(String[] pageItems)
```


Добавляет поле страницы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| pageItems | java.lang.String[] | Метка элемента поля страницы |

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
### getPageFieldCount() {#getPageFieldCount--}
```
public int getPageFieldCount()
```


Получает количество полей страницы.

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

