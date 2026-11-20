---
title: "TableStyleElementCollection"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет все элементы стиля таблицы."
type: docs
url: /ru/java/com.aspose.cells/tablestyleelementcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class TableStyleElementCollection extends CollectionBase
```

Представляет все элементы стиля таблицы.
## Методы

| Метод | Описание |
| --- | --- |
| [add(int type)](#add-int-) | Добавляет элемент. |
| [add(Object o)](#add-java.lang.Object-) | Добавляет элемент в экземпляр CollectionBase. |
| [clear()](#clear--) | Удаляет все объекты из экземпляра CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Возвращает, содержит ли экземпляр этот объект |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Получает элемент стиля таблицы по индексу. |
| [getByTableStyleElementType(int type)](#getByTableStyleElementType-int-) | Получает элемент стиля таблицы по типу элемента. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Получает количество элементов, содержащихся в экземпляре CollectionBase. |
| [getTableStyleElementWithIndex(int index)](#getTableStyleElementWithIndex-int-) | Получает элемент стиля таблицы по индексу. |
| [getTableStyleElementWithType(int type)](#getTableStyleElementWithType-int-) | Получает элемент стиля таблицы по типу элемента. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Определяет индекс конкретного элемента в экземпляре CollectionBase. |
| [iterator()](#iterator--) | Возвращает перечислитель, который проходит по экземпляру CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Удаляет элемент по указанному индексу. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int type) {#add-int-}
```
public int add(int type)
```


Добавляет элемент.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [TableStyleElementType](../../com.aspose.cells/tablestyleelementtype). Тип элемента |

**Returns:**
int — Возвращает индекс элемента в списке.
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
public TableStyleElement get(int index)
```


Получает элемент стиля таблицы по индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс. |

**Returns:**
[TableStyleElement](../../com.aspose.cells/tablestyleelement) - Returns [TableStyleElement](../../com.aspose.cells/tablestyleelement) object
### getByTableStyleElementType(int type) {#getByTableStyleElementType-int-}
```
public TableStyleElement getByTableStyleElementType(int type)
```


Получает элемент стиля таблицы по типу элемента.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [TableStyleElementType](../../com.aspose.cells/tablestyleelementtype). Тип элемента. |

**Returns:**
[TableStyleElement](../../com.aspose.cells/tablestyleelement) - Returns [TableStyleElement](../../com.aspose.cells/tablestyleelement) object
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
### getTableStyleElementWithIndex(int index) {#getTableStyleElementWithIndex-int-}
```
public TableStyleElement getTableStyleElementWithIndex(int index)
```


Получает элемент стиля таблицы по индексу.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство Aspose.Cells.Tables.TableStyleElementCollection.this[int index]. Это свойство будет удалено через 12 месяцев, начиная с ЯНВАРЯ 2012 года. Aspose приносит извинения за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int |  |

**Returns:**
[TableStyleElement](../../com.aspose.cells/tablestyleelement)
### getTableStyleElementWithType(int type) {#getTableStyleElementWithType-int-}
```
public TableStyleElement getTableStyleElementWithType(int type)
```


Получает элемент стиля таблицы по типу элемента.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство Aspose.Cells.Tables.TableStyleElementCollection.this[TableStyleElementType type]. Это свойство будет удалено через 12 месяцев, начиная с ЯНВАРЯ 2012 года. Aspose приносит извинения за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| тип | int |  |

**Returns:**
[TableStyleElement](../../com.aspose.cells/tablestyleelement)
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


Удаляет элемент по указанному индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Нулевой индекс элемента, который нужно удалить. |

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

