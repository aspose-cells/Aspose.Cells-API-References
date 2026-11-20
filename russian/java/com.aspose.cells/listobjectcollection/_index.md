---
title: "ListObjectCollection"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет коллекцию объектов в листе."
type: docs
url: /ru/java/com.aspose.cells/listobjectcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ListObjectCollection extends CollectionBase
```

Представляет коллекцию объектов [ListObject](../../com.aspose.cells/listobject) в листе.
## Методы

| Метод | Описание |
| --- | --- |
| [add(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders)](#add-int-int-int-int-boolean-) | Добавляет ListObject в лист. |
| [add(Object o)](#add-java.lang.Object-) | Добавляет элемент в экземпляр CollectionBase. |
| [add(String startCell, String endCell, boolean hasHeaders)](#add-java.lang.String-java.lang.String-boolean-) | Добавляет ListObject в лист. |
| [clear()](#clear--) | Удаляет все объекты из экземпляра CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Возвращает, содержит ли экземпляр этот объект |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Получает ListObject по индексу. |
| [get(String tableName)](#get-java.lang.String-) | Получает ListObject по указанному имени. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Получает количество элементов, содержащихся в экземпляре CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Определяет индекс конкретного элемента в экземпляре CollectionBase. |
| [iterator()](#iterator--) | Возвращает перечислитель, который проходит по экземпляру CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Удалить [ListObject](../../com.aspose.cells/listobject) по индексу. |
| [toString()](#toString--) |  |
| [updateColumnName()](#updateColumnName--) | Обновить все имена столбцов таблиц. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders) {#add-int-int-int-int-boolean-}
```
public int add(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders)
```


Добавляет ListObject в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | int | Начальная строка диапазона списка. |
| startColumn | int | Начальная строка диапазона списка. |
| endRow | int | Начальная строка диапазона списка. |
| endColumn | int | Начальная строка диапазона списка. |
| hasHeaders | boolean | Указывает, имеет ли диапазон заголовки. |

**Returns:**
int - Индекс нового ListObject
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Добавляет элемент в экземпляр CollectionBase.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| o | java.lang.Object | Объект, который нужно добавить в экземпляр CollectionBase. |

**Returns:**
int — позиция, в которую был вставлен новый элемент.
### add(String startCell, String endCell, boolean hasHeaders) {#add-java.lang.String-java.lang.String-boolean-}
```
public int add(String startCell, String endCell, boolean hasHeaders)
```


Добавляет ListObject в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startCell | java.lang.String | Начальная ячейка диапазона списка. |
| endCell | java.lang.String | Конечная ячейка диапазона списка. |
| hasHeaders | boolean | Указывает, имеет ли диапазон заголовки. |

**Returns:**
int - Индекс нового ListObject
### clear() {#clear--}
```
public void clear()
```


Удаляет все объекты из экземпляра CollectionBase.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Возвращает, содержит ли экземпляр этот объект

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| o | java.lang.Object | тестовый объект |

**Returns:**
boolean — содержит ли экземпляр этот объект
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
public ListObject get(int index)
```


Получает ListObject по индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс. |

**Returns:**
[ListObject](../../com.aspose.cells/listobject) - The ListObject
### get(String tableName) {#get-java.lang.String-}
```
public ListObject get(String tableName)
```


Получает ListObject по указанному имени.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| tableName | java.lang.String | Имя ListObject. |

**Returns:**
[ListObject](../../com.aspose.cells/listobject) - The ListObject
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


Получает количество элементов, содержащихся в экземпляре CollectionBase.

**Returns:**
int — количество элементов, содержащихся в экземпляре CollectionBase.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


Определяет индекс конкретного элемента в экземпляре CollectionBase.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| o | java.lang.Object | Определяет индекс конкретного элемента в экземпляре CollectionBase. |

**Returns:**
int — индекс значения, если оно найдено в списке; иначе -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Возвращает перечислитель, который проходит по экземпляру CollectionBase.

**Returns:**
java.util.Iterator — итератор для экземпляра CollectionBase.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Удалить [ListObject](../../com.aspose.cells/listobject) по индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс. |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### updateColumnName() {#updateColumnName--}
```
public void updateColumnName()
```


Обновить все имена столбцов таблиц.

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

