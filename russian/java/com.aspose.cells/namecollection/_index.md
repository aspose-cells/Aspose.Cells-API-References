---
title: "NameCollection"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет коллекцию всех объектов в электронной таблице."
type: docs
url: /ru/java/com.aspose.cells/namecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class NameCollection extends CollectionBase
```

Представляет коллекцию всех объектов [Name](../../com.aspose.cells/name) в электронной таблице.
## Методы

| Метод | Описание |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Добавляет элемент в экземпляр CollectionBase. |
| [add(String text)](#add-java.lang.String-) | Определяет новое имя. |
| [clear()](#clear--) | Удалить все определённые имена, которые не используются в формулах и источнике данных. |
| [contains(Object o)](#contains-java.lang.Object-) | Возвращает, содержит ли экземпляр этот объект |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter(int type, int sheetIndex)](#filter-int-int-) | Получает все определённые имена по области. |
| [get(int index)](#get-int-) | Получает элемент [Name](../../com.aspose.cells/name) по указанному индексу. |
| [get(String text)](#get-java.lang.String-) | Получает элемент [Name](../../com.aspose.cells/name) с указанным именем. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Получает количество элементов, содержащихся в экземпляре CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Определяет индекс конкретного элемента в экземпляре CollectionBase. |
| [iterator()](#iterator--) | Возвращает перечислитель, который проходит по экземпляру CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String text)](#remove-java.lang.String-) | Удалить имя. |
| [remove(String[] names)](#remove-java.lang.String---) | Удалить массив имён. |
| [removeAt(int index)](#removeAt-int-) | Удалить имя по конкретному индексу. |
| [removeDuplicateNames()](#removeDuplicateNames--) | Удалить дублирующие определённые имена |
| [sort()](#sort--) | Сортирует определённые имена. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### add(String text) {#add-java.lang.String-}
```
public int add(String text)
```


Определяет новое имя.

**Remarks**

Имя не может содержать пробелы и не может выглядеть как ссылки на ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| текст | java.lang.String | Текст, используемый в качестве имени. |

**Returns:**
int — индекс объекта [Name](../../com.aspose.cells/name).
### clear() {#clear--}
```
public void clear()
```


Удалить все определённые имена, которые не используются в формулах и источнике данных. Если определённое имя используется, мы просто устанавливаем Name.ReferTo в null и скрываем его.

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
### filter(int type, int sheetIndex) {#filter-int-int-}
```
public Name[] filter(int type, int sheetIndex)
```


Получает все определённые имена по области.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [NameScopeType](../../com.aspose.cells/namescopetype). Тип области. |
| sheetIndex | int | Индекс листа. Действует только когда тип области — [NameScopeType.WORKSHEET](../../com.aspose.cells/namescopetype\#WORKSHEET). |

**Returns:**
com.aspose.cells.Name[] -
### get(int index) {#get-int-}
```
public Name get(int index)
```


Получает элемент [Name](../../com.aspose.cells/name) по указанному индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Нулевой индекс элемента. |

**Returns:**
[Name](../../com.aspose.cells/name) - The element at the specified index.
### get(String text) {#get-java.lang.String-}
```
public Name get(String text)
```


Получает элемент [Name](../../com.aspose.cells/name) с указанным именем.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| текст | java.lang.String | Текст имени. |

**Returns:**
[Name](../../com.aspose.cells/name) - The element with the specified name.
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




### remove(String text) {#remove-java.lang.String-}
```
public void remove(String text)
```


Удалить имя.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| текст | java.lang.String | Текст имени. |

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

Пожалуйста, убедитесь, что имя не используется другими формулами перед вызовом метода. И если имя используется, лучше установить Name.RefersTo в null.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс имени, которое нужно удалить. |

### removeDuplicateNames() {#removeDuplicateNames--}
```
public void removeDuplicateNames()
```


Удалить дублирующие определённые имена

### sort() {#sort--}
```
public void sort()
```


Сортирует определённые имена.

**Remarks**

Если вы создаёте большое количество именованных диапазонов в файле Excel, пожалуйста, вызовите этот метод после создания всех именованных диапазонов и перед сохранением.

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

