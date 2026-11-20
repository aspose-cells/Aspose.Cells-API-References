---
title: "PivotFilterCollection"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет коллекцию всех PivotFilters."
type: docs
url: /ru/java/com.aspose.cells/pivotfiltercollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotFilterCollection extends CollectionBase
```

Представляет коллекцию всех PivotFilters.
## Методы

| Метод | Описание |
| --- | --- |
| [add(int fieldIndex, int type)](#add-int-int-) | Добавляет объект PivotFilter к определенному типу |
| [add(Object o)](#add-java.lang.Object-) | Добавляет элемент в экземпляр CollectionBase. |
| [addDateFilter(int baseFieldIndex, int type, DateTime dateTime1, DateTime dateTime2)](#addDateFilter-int-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-) | Фильтрует по настройке даты строки или столбца сводного поля. |
| [addLabelFilter(int baseFieldIndex, int type, String label1, String label2)](#addLabelFilter-int-int-java.lang.String-java.lang.String-) | Фильтрует по подписьям строки или столбца сводного поля. |
| [addTop10Filter(int baseFieldIndex, int valueFieldIndex, int type, boolean isTop, int itemCount)](#addTop10Filter-int-int-int-boolean-int-) | Фильтрует по значениям данных сводного поля. |
| [addValueFilter(int baseFieldIndex, int valueFieldIndex, int type, double value1, double value2)](#addValueFilter-int-int-int-double-double-) | Фильтрует по значениям данных сводного поля. |
| [clear()](#clear--) | Удаляет все объекты из экземпляра CollectionBase. |
| [clearFilter(int fieldIndex)](#clearFilter-int-) | Очистить PivotFilter из конкретного PivotField |
| [contains(Object o)](#contains-java.lang.Object-) | Возвращает, содержит ли экземпляр этот объект |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Получает объект pivotfilter по конкретному индексу. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Получает количество элементов, содержащихся в экземпляре CollectionBase. |
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
### add(int fieldIndex, int type) {#add-int-int-}
```
public int add(int fieldIndex, int type)
```


Добавляет объект PivotFilter к определенному типу

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте методы PivotFilterCollection.AddValueFilter(), AddTop10Filter(), AddLabelFilter() и AddDateFilter(). Этот метод будет удалён через 12 месяцев, начиная с ноября 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | int | индекс PivotField |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). тип PivotFilter |

**Returns:**
int - индекс объекта PivotFilter в этой PivotFilterCollection.
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
### addDateFilter(int baseFieldIndex, int type, DateTime dateTime1, DateTime dateTime2) {#addDateFilter-int-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-}
```
public PivotFilter addDateFilter(int baseFieldIndex, int type, DateTime dateTime1, DateTime dateTime2)
```


Фильтрует по настройке даты строки или столбца сводного поля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| baseFieldIndex | int | Индекс поля в источнике. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Тип фильтрации данных. |
| dateTime1 | [DateTime](../../com.aspose.cells/datetime) | Дата метки условия фильтра |
| dateTime2 | [DateTime](../../com.aspose.cells/datetime) | Верхняя граница даты метки условия фильтра между |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### addLabelFilter(int baseFieldIndex, int type, String label1, String label2) {#addLabelFilter-int-int-java.lang.String-java.lang.String-}
```
public PivotFilter addLabelFilter(int baseFieldIndex, int type, String label1, String label2)
```


Фильтрует по подписьям строки или столбца сводного поля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| baseFieldIndex | int | Индекс поля в источнике. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Тип фильтрации данных. |
| label1 | java.lang.String | Метка условия фильтра |
| label2 | java.lang.String | Верхняя граница метки условия фильтра между |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### addTop10Filter(int baseFieldIndex, int valueFieldIndex, int type, boolean isTop, int itemCount) {#addTop10Filter-int-int-int-boolean-int-}
```
public PivotFilter addTop10Filter(int baseFieldIndex, int valueFieldIndex, int type, boolean isTop, int itemCount)
```


Фильтрует по значениям данных сводного поля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| baseFieldIndex | int | Индекс поля в источнике. |
| valueFieldIndex | int | Индекс поля данных в области данных. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Тип фильтрации данных. Может быть только Count, Sum и Percent. |
| isTop | boolean | Указывает, применяется ли фильтр сверху или снизу |
| itemCount | int | Количество элементов |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### addValueFilter(int baseFieldIndex, int valueFieldIndex, int type, double value1, double value2) {#addValueFilter-int-int-int-double-double-}
```
public PivotFilter addValueFilter(int baseFieldIndex, int valueFieldIndex, int type, double value1, double value2)
```


Фильтрует по значениям данных сводного поля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| baseFieldIndex | int | Индекс поля в источнике. |
| valueFieldIndex | int | Индекс поля значения в области значений. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Тип фильтрации данных. |
| value1 | double | Значение условия фильтра |
| value2 | double | Верхнее значение условия фильтра между |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### clear() {#clear--}
```
public void clear()
```


Удаляет все объекты из экземпляра CollectionBase.

### clearFilter(int fieldIndex) {#clearFilter-int-}
```
public void clearFilter(int fieldIndex)
```


Очистить PivotFilter из конкретного PivotField

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | int | индекс PivotField |

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
public PivotFilter get(int index)
```


Получает объект pivotfilter по конкретному индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int |  |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
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

