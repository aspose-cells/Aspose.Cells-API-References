---
title: "PivotTableFormatCollection"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет коллекцию форматов, применённых к сводной таблице."
type: docs
url: /ru/java/com.aspose.cells/pivottableformatcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotTableFormatCollection extends CollectionBase
```

Представляет коллекцию форматов, применённых к сводной таблице.
## Методы

| Метод | Описание |
| --- | --- |
| [add()](#add--) | Добавьте [PivotTableFormat](../../com.aspose.cells/pivottableformat). |
| [add(Object o)](#add-java.lang.Object-) | Добавляет элемент в экземпляр CollectionBase. |
| [clear()](#clear--) | Удаляет все объекты из экземпляра CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Возвращает, содержит ли экземпляр этот объект |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [format(CellArea ca, Style style)](#format-com.aspose.cells.CellArea-com.aspose.cells.Style-) | Форматирует выбранную область сводной таблицы. |
| [format(PivotArea pivotArea, Style style)](#format-com.aspose.cells.PivotArea-com.aspose.cells.Style-) | Форматирует выбранную область сводной таблицы. |
| [format(int row, int column, Style style)](#format-int-int-com.aspose.cells.Style-) | Форматирует ячейку в области сводной таблицы |
| [formatArea(int axisType, int fieldPosition, int subtotalType, int selectionType, boolean isGrandRow, boolean isGrandColumn, Style style)](#formatArea-int-int-int-int-boolean-boolean-com.aspose.cells.Style-) | Форматирует выбранную область. |
| [get(int index)](#get-int-) | Получает формат по индексу. |
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
### add() {#add--}
```
public int add()
```


Добавьте [PivotTableFormat](../../com.aspose.cells/pivottableformat).

**Returns:**
int - Индекс нового формата.
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
### format(CellArea ca, Style style) {#format-com.aspose.cells.CellArea-com.aspose.cells.Style-}
```
public void format(CellArea ca, Style style)
```


Форматирует выбранную область сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Диапазон ячеек. |
| style | [Style](../../com.aspose.cells/style) | Стиль |

### format(PivotArea pivotArea, Style style) {#format-com.aspose.cells.PivotArea-com.aspose.cells.Style-}
```
public void format(PivotArea pivotArea, Style style)
```


Форматирует выбранную область сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| pivotArea | [PivotArea](../../com.aspose.cells/pivotarea) | Выбранная область представления сводной таблицы. |
| style | [Style](../../com.aspose.cells/style) | Форматированная настройка. |

### format(int row, int column, Style style) {#format-int-int-com.aspose.cells.Style-}
```
public void format(int row, int column, Style style)
```


Форматирует ячейку в области сводной таблицы

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки ячейки |
| столбец | int | Индекс столбца ячейки |
| style | [Style](../../com.aspose.cells/style) | Стиль, используемый для форматирования ячейки |

### formatArea(int axisType, int fieldPosition, int subtotalType, int selectionType, boolean isGrandRow, boolean isGrandColumn, Style style) {#formatArea-int-int-int-int-boolean-boolean-com.aspose.cells.Style-}
```
public PivotTableFormat formatArea(int axisType, int fieldPosition, int subtotalType, int selectionType, boolean isGrandRow, boolean isGrandColumn, Style style)
```


Форматирует выбранную область.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Область PivotTable, к которой применяется это правило. |
| fieldPosition | int | Позиция поля по оси, к которой применяется это правило. |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). Тип фильтра подытога поля сводной таблицы. |
| selectionType | int | [PivotTableSelectionType](../../com.aspose.cells/pivottableselectiontype). Указывает, как выбирать данные. |
| isGrandRow | boolean | Указывает, выбираются ли строки с итоговыми суммами. |
| isGrandColumn | boolean | Указывает, выбираются ли столбцы с итоговыми суммами. |
| style | [Style](../../com.aspose.cells/style) | Стиль, применяемый к области сводной таблицы. |

**Returns:**
[PivotTableFormat](../../com.aspose.cells/pivottableformat) - 
### get(int index) {#get-int-}
```
public PivotTableFormat get(int index)
```


Получает формат по индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс. |

**Returns:**
[PivotTableFormat](../../com.aspose.cells/pivottableformat) - 
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

