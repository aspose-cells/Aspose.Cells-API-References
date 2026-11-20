---
title: "SlicerCollection"
second_title: "Справочник API Aspose.Cells for Java"
description: "Указывает коллекцию всех объектов Slicer на указанном листе."
type: docs
url: /ru/java/com.aspose.cells/slicercollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class SlicerCollection extends CollectionBase
```

Указывает коллекцию всех объектов Slicer на указанном листе.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         pivot.calculateData();
 
         SlicerCollection slicers = sheet.getSlicers();
         int slicerIndex = slicers.add(pivot, "E12", "fruit");
         Slicer slicer = slicers.get(slicerIndex);
 
         //do your business
 
         book.save("out.xlsx");
```
## Методы

| Метод | Описание |
| --- | --- |
| [add(ListObject table, ListColumn listColumn, int row, int column)](#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-int-int-) | Добавьте новый Slicer, используя ListObjet в качестве источника данных |
| [add(ListObject table, ListColumn listColumn, String destCellName)](#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-java.lang.String-) | Добавьте новый Slicer, используя ListObjet в качестве источника данных |
| [add(ListObject table, int index, String destCellName)](#add-com.aspose.cells.ListObject-int-java.lang.String-) | Добавьте новый Slicer, используя ListObjet в качестве источника данных |
| [add(PivotTable pivot, int row, int column, PivotField baseField)](#add-com.aspose.cells.PivotTable-int-int-com.aspose.cells.PivotField-) | Добавьте новый Slicer, используя PivotTable в качестве источника данных |
| [add(PivotTable pivot, int row, int column, int baseFieldIndex)](#add-com.aspose.cells.PivotTable-int-int-int-) | Добавьте новый Slicer, используя PivotTable в качестве источника данных |
| [add(PivotTable pivot, int row, int column, String baseFieldName)](#add-com.aspose.cells.PivotTable-int-int-java.lang.String-) | Добавьте новый Slicer, используя PivotTable в качестве источника данных |
| [add(PivotTable pivot, String destCellName, PivotField baseField)](#add-com.aspose.cells.PivotTable-java.lang.String-com.aspose.cells.PivotField-) | Добавьте новый Slicer, используя PivotTable в качестве источника данных |
| [add(PivotTable pivot, String destCellName, int baseFieldIndex)](#add-com.aspose.cells.PivotTable-java.lang.String-int-) | Добавьте новый Slicer, используя PivotTable в качестве источника данных |
| [add(PivotTable pivot, String destCellName, String baseFieldName)](#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-) | Добавьте новый Slicer, используя PivotTable в качестве источника данных |
| [add(Object o)](#add-java.lang.Object-) | Добавляет элемент в экземпляр CollectionBase. |
| [clear()](#clear--) | Очистить все Slicers. |
| [contains(Object o)](#contains-java.lang.Object-) | Возвращает, содержит ли экземпляр этот объект |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Получает Slicer по индексу. |
| [get(String name)](#get-java.lang.String-) | Получает Slicer по имени среза. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Получает количество элементов, содержащихся в экземпляре CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Определяет индекс конкретного элемента в экземпляре CollectionBase. |
| [iterator()](#iterator--) | Возвращает перечислитель, который проходит по экземпляру CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Slicer slicer)](#remove-com.aspose.cells.Slicer-) | Удалить указанный Slicer |
| [removeAt(int index)](#removeAt-int-) | Удаляет Slicer по указанному индексу |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(ListObject table, ListColumn listColumn, int row, int column) {#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-int-int-}
```
public int add(ListObject table, ListColumn listColumn, int row, int column)
```


Добавьте новый Slicer, используя ListObjet в качестве источника данных

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| table | [ListObject](../../com.aspose.cells/listobject) | ListObject object |
| listColumn | [ListColumn](../../com.aspose.cells/listcolumn) | Колонка ListColumn в ListObject.ListColumns |
| строка | int | Индекс строки ячейки в левом верхнем углу диапазона Slicer. |
| столбец | int | Индекс столбца ячейки в левом верхнем углу диапазона Slicer. |

**Returns:**
int — индекс нового добавляемого Slicer
### add(ListObject table, ListColumn listColumn, String destCellName) {#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-java.lang.String-}
```
public int add(ListObject table, ListColumn listColumn, String destCellName)
```


Добавьте новый Slicer, используя ListObjet в качестве источника данных

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| table | [ListObject](../../com.aspose.cells/listobject) | ListObject object |
| listColumn | [ListColumn](../../com.aspose.cells/listcolumn) | Колонка ListColumn в ListObject.ListColumns |
| destCellName | java.lang.String | Ячейка в левом верхнем углу диапазона Slicer. |

**Returns:**
int — индекс нового добавляемого Slicer
### add(ListObject table, int index, String destCellName) {#add-com.aspose.cells.ListObject-int-java.lang.String-}
```
public int add(ListObject table, int index, String destCellName)
```


Добавьте новый Slicer, используя ListObjet в качестве источника данных

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| table | [ListObject](../../com.aspose.cells/listobject) | ListObject object |
| индекс | int | Индекс ListColumn в ListObject.ListColumns |
| destCellName | java.lang.String | Ячейка в левом верхнем углу диапазона Slicer. |

**Returns:**
int — индекс нового добавляемого Slicer
### add(PivotTable pivot, int row, int column, PivotField baseField) {#add-com.aspose.cells.PivotTable-int-int-com.aspose.cells.PivotField-}
```
public int add(PivotTable pivot, int row, int column, PivotField baseField)
```


Добавьте новый Slicer, используя PivotTable в качестве источника данных

**Example**

```
         slicers.add(pivot, 3, 12, pivot.getBaseFields().get(0));
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | Объект PivotTable |
| строка | int | Индекс строки ячейки в левом верхнем углу диапазона Slicer. |
| столбец | int | Индекс столбца ячейки в левом верхнем углу диапазона Slicer. |
| baseField | [PivotField](../../com.aspose.cells/pivotfield) | Поле PivotField в PivotTable.BaseFields |

**Returns:**
int — индекс нового добавляемого Slicer
### add(PivotTable pivot, int row, int column, int baseFieldIndex) {#add-com.aspose.cells.PivotTable-int-int-int-}
```
public int add(PivotTable pivot, int row, int column, int baseFieldIndex)
```


Добавьте новый Slicer, используя PivotTable в качестве источника данных

**Example**

```
         slicers.add(pivot, 20, 8, 0);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | Объект PivotTable |
| строка | int | Индекс строки ячейки в левом верхнем углу диапазона Slicer. |
| столбец | int | Индекс столбца ячейки в левом верхнем углу диапазона Slicer. |
| baseFieldIndex | int | Индекс PivotField в PivotTable.BaseFields |

**Returns:**
int — индекс нового добавляемого Slicer
### add(PivotTable pivot, int row, int column, String baseFieldName) {#add-com.aspose.cells.PivotTable-int-int-java.lang.String-}
```
public int add(PivotTable pivot, int row, int column, String baseFieldName)
```


Добавьте новый Slicer, используя PivotTable в качестве источника данных

**Example**

```
         slicers.add(pivot, 20, 12, "fruit");
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | Объект PivotTable |
| строка | int | Индекс строки ячейки в левом верхнем углу диапазона Slicer. |
| столбец | int | Индекс столбца ячейки в левом верхнем углу диапазона Slicer. |
| baseFieldName | java.lang.String | Имя PivotField в PivotTable.BaseFields |

**Returns:**
int — индекс нового добавляемого Slicer
### add(PivotTable pivot, String destCellName, PivotField baseField) {#add-com.aspose.cells.PivotTable-java.lang.String-com.aspose.cells.PivotField-}
```
public int add(PivotTable pivot, String destCellName, PivotField baseField)
```


Добавьте новый Slicer, используя PivotTable в качестве источника данных

**Example**

```
         slicers.add(pivot, "I3", pivot.getBaseFields().get(0));
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | Объект PivotTable |
| destCellName | java.lang.String | Ячейка в левом верхнем углу диапазона Slicer. |
| baseField | [PivotField](../../com.aspose.cells/pivotfield) | Поле PivotField в PivotTable.BaseFields |

**Returns:**
int — индекс нового добавляемого Slicer
### add(PivotTable pivot, String destCellName, int baseFieldIndex) {#add-com.aspose.cells.PivotTable-java.lang.String-int-}
```
public int add(PivotTable pivot, String destCellName, int baseFieldIndex)
```


Добавьте новый Slicer, используя PivotTable в качестве источника данных

**Example**

```
         slicers.add(pivot, "E20", 0);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | Объект PivotTable |
| destCellName | java.lang.String | Ячейка в левом верхнем углу диапазона Slicer. |
| baseFieldIndex | int | Индекс PivotField в PivotTable.BaseFields |

**Returns:**
int — индекс нового добавляемого Slicer
### add(PivotTable pivot, String destCellName, String baseFieldName) {#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-}
```
public int add(PivotTable pivot, String destCellName, String baseFieldName)
```


Добавьте новый Slicer, используя PivotTable в качестве источника данных

**Example**

```
         slicers.add(pivot, "E3", "fruit");
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | Объект PivotTable |
| destCellName | java.lang.String | Ячейка в левом верхнем углу диапазона Slicer. |
| baseFieldName | java.lang.String | Имя PivotField в PivotTable.BaseFields |

**Returns:**
int — индекс нового добавляемого Slicer
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


Очистить все Slicers.

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
public Slicer get(int index)
```


Получает Slicer по индексу.

**Example**

```
         Slicer slicerByIndex = slicers.get(0);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int |  |

**Returns:**
[Slicer](../../com.aspose.cells/slicer)
### get(String name) {#get-java.lang.String-}
```
public Slicer get(String name)
```


Получает Slicer по имени среза.

**Example**

```
         Slicer slicerByName = slicers.get("fruit");
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[Slicer](../../com.aspose.cells/slicer)
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




### remove(Slicer slicer) {#remove-com.aspose.cells.Slicer-}
```
public void remove(Slicer slicer)
```


Удалить указанный Slicer

**Example**

```
         Slicer delSlicer = slicers.get(0);
         slicers.remove(delSlicer);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| slicer | [Slicer](../../com.aspose.cells/slicer) | Объект Slicer |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Удаляет Slicer по указанному индексу

**Example**

```
         slicers.removeAt(1);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс позиции в коллекции Slicer |

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

