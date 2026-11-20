---
title: "GridPivotTableCollection"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует коллекцию объектов."
type: docs
url: /ru/java/com.aspose.gridweb/gridpivottablecollection/
---

**Inheritance:**
java.lang.Object
```
public class GridPivotTableCollection
```

Инкапсулирует коллекцию объектов [GridPivotTable](../../com.aspose.gridweb/gridpivottable).
## Методы

| Метод | Описание |
| --- | --- |
| [add(GridWorksheet sourceSheet, GridCellArea sourceArea, String destCellName, String tableName)](#add-com.aspose.gridweb.GridWorksheet-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-) | Добавляет новый кэш PivotTable в коллекцию PivotCaches. |
| [add(String worksheetname, GridCellArea sourceArea, int destRow, int destCol, String tableName)](#add-java.lang.String-com.aspose.gridweb.GridCellArea-int-int-java.lang.String-) | Добавляет новый кэш PivotTable в коллекцию PivotCaches. |
| [add(String worksheetname, GridCellArea sourceArea, String destCellName, String tableName)](#add-java.lang.String-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-) | Добавляет новый кэш PivotTable в коллекцию PivotCaches. |
| [add(String sourceData, String destCellName, String tableName)](#add-java.lang.String-java.lang.String-java.lang.String-) | Добавляет новый кэш PivotTable в коллекцию PivotCaches. |
| [clear()](#clear--) | Очищает все PivotTable. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Получает элемент [GridPivotTable](../../com.aspose.gridweb/gridpivottable) по указанному индексу. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Получает размер перечислителя |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Удаляет PivotTable по указанному индексу. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(GridWorksheet sourceSheet, GridCellArea sourceArea, String destCellName, String tableName) {#add-com.aspose.gridweb.GridWorksheet-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-}
```
public int add(GridWorksheet sourceSheet, GridCellArea sourceArea, String destCellName, String tableName)
```


Добавляет новый кэш PivotTable в коллекцию PivotCaches.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceSheet | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) | Исходный лист. |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Область в исходном листе. |
| destCellName | java.lang.String | Ячейка в левом верхнем углу диапазона назначения отчета сводной таблицы. |
| tableName | java.lang.String | Имя нового отчета сводной таблицы. |

**Returns:**
int — Индекс только что добавленного кэша.
### add(String worksheetname, GridCellArea sourceArea, int destRow, int destCol, String tableName) {#add-java.lang.String-com.aspose.gridweb.GridCellArea-int-int-java.lang.String-}
```
public int add(String worksheetname, GridCellArea sourceArea, int destRow, int destCol, String tableName)
```


Добавляет новый кэш PivotTable в коллекцию PivotCaches.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| worksheetname | java.lang.String | Имя исходного листа. |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Область в исходном листе. |
| destRow | int | Номер строки ячейки в левом верхнем углу диапазона назначения отчёта PivotTable. |
| destCol | int | Номер столбца ячейки в левом верхнем углу диапазона назначения отчёта PivotTable. |
| tableName | java.lang.String | Имя нового отчета сводной таблицы. |

**Returns:**
int — Индекс только что добавленного кэша.
### add(String worksheetname, GridCellArea sourceArea, String destCellName, String tableName) {#add-java.lang.String-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-}
```
public int add(String worksheetname, GridCellArea sourceArea, String destCellName, String tableName)
```


Добавляет новый кэш PivotTable в коллекцию PivotCaches.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| worksheetname | java.lang.String | Имя исходного листа. |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Область в исходном листе. |
| destCellName | java.lang.String | Ячейка в левом верхнем углу диапазона назначения отчета сводной таблицы. |
| tableName | java.lang.String | Имя нового отчета сводной таблицы. |

**Returns:**
int — Индекс только что добавленного кэша.
### add(String sourceData, String destCellName, String tableName) {#add-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String sourceData, String destCellName, String tableName)
```


Добавляет новый кэш PivotTable в коллекцию PivotCaches.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceData | java.lang.String | Диапазон ячеек данных для новой сводной таблицы. Пример: Sheet1!A1:C8 |
| destCellName | java.lang.String | Ячейка в левом верхнем углу диапазона назначения отчета сводной таблицы. |
| tableName | java.lang.String | Имя нового отчета сводной таблицы. |

**Returns:**
int — Индекс только что добавленного кэша.
### clear() {#clear--}
```
public void clear()
```


Очищает все PivotTable.

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
public GridPivotTable get(int index)
```


Получает элемент [GridPivotTable](../../com.aspose.gridweb/gridpivottable) по указанному индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Нулевой индекс элемента. |

**Returns:**
[GridPivotTable](../../com.aspose.gridweb/gridpivottable) - The element at the specified index.
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


Удаляет PivotTable по указанному индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Нулевой индекс элемента. |

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

