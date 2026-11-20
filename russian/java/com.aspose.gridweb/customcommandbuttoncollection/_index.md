---
title: "CustomCommandButtonCollection"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет коллекцию CustomCommandButton."
type: docs
url: /ru/java/com.aspose.gridweb/customcommandbuttoncollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.CollectionBase](../../com.aspose.gridweb/collectionbase)
```
public class CustomCommandButtonCollection extends CollectionBase
```

Представляет коллекцию CustomCommandButton.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         CustomCommandButton button = new CustomCommandButton();
         button.setCommand("MyCommand");
         button.setImageUrl("images/button1.gif");
         GridWeb1.getCustomCommandButtons().add(button);
```
## Методы

| Метод | Описание |
| --- | --- |
| [add(Object value)](#add-java.lang.Object-) | Добавьте объект пользовательской кнопки команды в коллекцию. |
| [clear()](#clear--) | Очищает коллекцию. |
| [contains(Object value)](#contains-java.lang.Object-) | Указывает, находится ли объект пользовательской кнопки команды в коллекции. |
| [copyTo(Object[] array, int index)](#copyTo-java.lang.Object---int-) | Копирует коллекцию в массив. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Получает объект пользовательской кнопки команды по индексу. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Получает количество элементов в коллекции. |
| [getSyncRoot()](#getSyncRoot--) | Используется только внутри. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object value)](#indexOf-java.lang.Object-) | Получает индекс кнопки. |
| [insert(int index, Object value)](#insert-int-java.lang.Object-) | Вставляет кнопку по индексу. |
| [isFixedSize()](#isFixedSize--) | Используется только внутри. |
| [isReadOnly()](#isReadOnly--) | Используется только внутри. |
| [isSynchronized()](#isSynchronized--) | Используется только внутри. |
| [iterator()](#iterator--) | Получает объект IEnumerator из коллекции. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Object value)](#remove-java.lang.Object-) | Удаляет объект пользовательской кнопки команды. |
| [removeAt(int index)](#removeAt-int-) | Удаляет по индексу. |
| [set(int index, CustomCommandButton value)](#set-int-com.aspose.gridweb.CustomCommandButton-) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object value) {#add-java.lang.Object-}
```
public int add(Object value)
```


Добавьте объект пользовательской кнопки команды в коллекцию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.Object | Объект пользовательской кнопки команды. |

**Returns:**
int — индекс.
### clear() {#clear--}
```
public void clear()
```


Очищает коллекцию.

### contains(Object value) {#contains-java.lang.Object-}
```
public boolean contains(Object value)
```


Указывает, находится ли объект пользовательской кнопки команды в коллекции.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.Object | Указывает, находится ли объект пользовательской кнопки команды в коллекции. |

**Returns:**
boolean — Истина или ложь.
### copyTo(Object[] array, int index) {#copyTo-java.lang.Object---int-}
```
public void copyTo(Object[] array, int index)
```


Копирует коллекцию в массив.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| массив | java.lang.Object[] | Массив. |
| индекс | int | Начальный индекс массива. |

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
public CustomCommandButton get(int index)
```


Получает объект пользовательской кнопки команды по индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int |  |

**Returns:**
[CustomCommandButton](../../com.aspose.gridweb/customcommandbutton)
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


Получает количество элементов в коллекции.

**Returns:**
int
### getSyncRoot() {#getSyncRoot--}
```
public Object getSyncRoot()
```


Используется только внутри.

**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object value) {#indexOf-java.lang.Object-}
```
public int indexOf(Object value)
```


Получает индекс кнопки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.Object | Объект кнопки. |

**Returns:**
int — индекс.
### insert(int index, Object value) {#insert-int-java.lang.Object-}
```
public void insert(int index, Object value)
```


Вставляет кнопку по индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс. |
| значение | java.lang.Object | Объект CustomCommandButton. |

### isFixedSize() {#isFixedSize--}
```
public boolean isFixedSize()
```


Используется только внутри.

**Returns:**
boolean
### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Используется только внутри.

**Returns:**
boolean
### isSynchronized() {#isSynchronized--}
```
public boolean isSynchronized()
```


Используется только внутри.

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


Получает объект IEnumerator из коллекции.

**Returns:**
java.util.Iterator — объект IEnumerator.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### remove(Object value) {#remove-java.lang.Object-}
```
public void remove(Object value)
```


Удаляет объект пользовательской кнопки команды.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.Object | Объект пользовательской кнопки команды. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Удаляет по индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс. |

### set(int index, CustomCommandButton value) {#set-int-com.aspose.gridweb.CustomCommandButton-}
```
public void set(int index, CustomCommandButton value)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int |  |
| value | [CustomCommandButton](../../com.aspose.gridweb/customcommandbutton) |  |

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

