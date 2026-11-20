---
title: "GridNameCollection"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует коллекцию объектов."
type: docs
url: /ru/java/com.aspose.gridweb/gridnamecollection/
---

**Inheritance:**
java.lang.Object
```
public class GridNameCollection
```

Инкапсулирует коллекцию объектов [GridName](../../com.aspose.gridweb/gridname).
## Методы

| Метод | Описание |
| --- | --- |
| [add(int sheetIndex, String text, String refersTo)](#add-int-java.lang.String-java.lang.String-) | Определяет новое имя на указанном листе. |
| [add(String text, String refersTo)](#add-java.lang.String-java.lang.String-) | Определяет новое глобальное имя. |
| [clear()](#clear--) | Удаляет все имена; |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Получает элемент [GridName](../../com.aspose.gridweb/gridname) по указанному индексу. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Получает размер перечислителя |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Получает перечислитель строк |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String[] names)](#remove-java.lang.String---) | Удалить массив имён. |
| [removeAt(int index)](#removeAt-int-) | Удалить имя по конкретному индексу. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int sheetIndex, String text, String refersTo) {#add-int-java.lang.String-java.lang.String-}
```
public int add(int sheetIndex, String text, String refersTo)
```


Определяет новое имя на указанном листе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetIndex | int | Индекс листа, в котором применяется имя. |
| текст | java.lang.String | Текст имени. Не может содержать имя листа. |
| refersTo | java.lang.String | Формула, к которой привязывается имя. Должна содержать имя листа, например, 'sheet hello!'A1:B2. |

**Returns:**
int — индекс объекта Name.
### add(String text, String refersTo) {#add-java.lang.String-java.lang.String-}
```
public int add(String text, String refersTo)
```


Определяет новое глобальное имя.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| текст | java.lang.String | Текст имени. Может содержать имя листа. |
| refersTo | java.lang.String | Формула, к которой привязывается имя. Должна содержать имя листа, например, 'sheet hello!'A1:B2. |

**Returns:**
int — индекс объекта Name.
### clear() {#clear--}
```
public void clear()
```


Удаляет все имена;

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
public GridName get(int index)
```


Получает элемент [GridName](../../com.aspose.gridweb/gridname) по указанному индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Нулевой индекс элемента. |

**Returns:**
[GridName](../../com.aspose.gridweb/gridname) - The element at the specified index.
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


Получает размер перечислителя

**Returns:**
int
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


Получает перечислитель строк

**Returns:**
java.util.Iterator — перечислитель строк
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### remove(String[] names) {#remove-java.lang.String---}
```
public void remove(String[] names)
```


Удалить массив имён.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имена | java.lang.String[] | Текст имен. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Удалить имя по конкретному индексу.

**Remarks**

Пожалуйста, убедитесь, что имя не используется другими формулами перед вызовом метода. И если имя используется, установите Name.RefersTo в null только.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int |  |

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

