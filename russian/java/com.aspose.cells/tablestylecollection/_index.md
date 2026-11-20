---
title: "TableStyleCollection"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет все пользовательские стили таблицы."
type: docs
url: /ru/java/com.aspose.cells/tablestylecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class TableStyleCollection extends CollectionBase
```

Представляет все пользовательские стили таблицы.
## Методы

| Метод | Описание |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Добавляет элемент в экземпляр CollectionBase. |
| [addPivotTableStyle(String name)](#addPivotTableStyle-java.lang.String-) | Добавляет пользовательский стиль сводной таблицы. |
| [addTableStyle(String name)](#addTableStyle-java.lang.String-) | Добавляет пользовательский стиль таблицы. |
| [clear()](#clear--) | Удаляет все объекты из экземпляра CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Возвращает, содержит ли экземпляр этот объект |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Получает стиль таблицы по индексу. |
| [get(String name)](#get-java.lang.String-) | Получает стиль таблицы по имени. |
| [getBuiltinTableStyle(int type)](#getBuiltinTableStyle-int-) | Получает встроенный стиль таблицы |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Получает количество элементов, содержащихся в экземпляре CollectionBase. |
| [getDefaultPivotStyleName()](#getDefaultPivotStyleName--) | Получает имя стиля по умолчанию сводной таблицы. |
| [getDefaultTableStyleName()](#getDefaultTableStyleName--) | Получает имя стиля по умолчанию таблицы. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Определяет индекс конкретного элемента в экземпляре CollectionBase. |
| [iterator()](#iterator--) | Возвращает перечислитель, который проходит по экземпляру CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Удаляет элемент по указанному индексу. |
| [setDefaultPivotStyleName(String value)](#setDefaultPivotStyleName-java.lang.String-) | Устанавливает имя стиля по умолчанию сводной таблицы. |
| [setDefaultTableStyleName(String value)](#setDefaultTableStyleName-java.lang.String-) | Устанавливает имя стиля по умолчанию таблицы. |
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
### addPivotTableStyle(String name) {#addPivotTableStyle-java.lang.String-}
```
public int addPivotTableStyle(String name)
```


Добавляет пользовательский стиль сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| name | java.lang.String | Имя стиля сводной таблицы. |

**Returns:**
int — индекс стиля сводной таблицы.
### addTableStyle(String name) {#addTableStyle-java.lang.String-}
```
public int addTableStyle(String name)
```


Добавляет пользовательский стиль таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| name | java.lang.String | Имя стиля таблицы. |

**Returns:**
int — индекс стиля таблицы.
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
public TableStyle get(int index)
```


Получает стиль таблицы по индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Позиция стиля таблицы в списке. |

**Returns:**
[TableStyle](../../com.aspose.cells/tablestyle) - The table style object.
### get(String name) {#get-java.lang.String-}
```
public TableStyle get(String name)
```


Получает стиль таблицы по имени.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| name | java.lang.String | Имя стиля таблицы. |

**Returns:**
[TableStyle](../../com.aspose.cells/tablestyle) - The table style object.
### getBuiltinTableStyle(int type) {#getBuiltinTableStyle-int-}
```
public TableStyle getBuiltinTableStyle(int type)
```


Получает встроенный стиль таблицы

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [TableStyleType](../../com.aspose.cells/tablestyletype). Встроенный тип стиля таблицы. |

**Returns:**
[TableStyle](../../com.aspose.cells/tablestyle) - 
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
### getDefaultPivotStyleName() {#getDefaultPivotStyleName--}
```
public String getDefaultPivotStyleName()
```


Получает имя стиля по умолчанию сводной таблицы.

**Returns:**
java.lang.String
### getDefaultTableStyleName() {#getDefaultTableStyleName--}
```
public String getDefaultTableStyleName()
```


Получает имя стиля по умолчанию таблицы.

**Returns:**
java.lang.String
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

### setDefaultPivotStyleName(String value) {#setDefaultPivotStyleName-java.lang.String-}
```
public void setDefaultPivotStyleName(String value)
```


Устанавливает имя стиля по умолчанию сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setDefaultTableStyleName(String value) {#setDefaultTableStyleName-java.lang.String-}
```
public void setDefaultTableStyleName(String value)
```


Устанавливает имя стиля по умолчанию таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

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

