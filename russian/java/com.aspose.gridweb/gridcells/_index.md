---
title: "GridCells"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует коллекцию объектов."
type: docs
url: /ru/java/com.aspose.gridweb/gridcells/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class GridCells implements Iterable
```

Инкапсулирует коллекцию объектов [GridCell](../../com.aspose.gridweb/gridcell).
## Методы

| Метод | Описание |
| --- | --- |
| [cellIndexToName(int row, int column)](#cellIndexToName-int-int-) | Получает имя ячейки по её индексам строки и столбца. |
| [cellNameToIndex(String cellName, int row, int column)](#cellNameToIndex-java.lang.String-int-int-) | Получает индексы строки и столбца ячейки по её имени. |
| [checkCell(int row, int column)](#checkCell-int-int-) | Получает элемент [GridCell](../../com.aspose.gridweb/gridcell) или null по указанным индексам строки и столбца ячейки. |
| [checkColumn(int col)](#checkColumn-int-) | Получает элемент [GridColumn](../../com.aspose.gridweb/gridcolumn) или null по указанному индексу столбца. |
| [checkRow(int i)](#checkRow-int-) | Получает элемент [GridRow](../../com.aspose.gridweb/gridrow) или null по указанному индексу строки ячейки. |
| [clear()](#clear--) | Очистить все ячейки в коллекции. |
| [clearContents(GridCellArea range)](#clearContents-com.aspose.gridweb.GridCellArea-) | Очищает содержимое диапазона. |
| [clearContents(int startRow, int startColumn, int endRow, int endColumn)](#clearContents-int-int-int-int-) | Очищает содержимое диапазона. |
| [clearFormats(GridCellArea range)](#clearFormats-com.aspose.gridweb.GridCellArea-) | Очищает форматирование диапазона. |
| [clearFormats(int startRow, int startColumn, int endRow, int endColumn)](#clearFormats-int-int-int-int-) | Очищает форматирование диапазона. |
| [clearRange(GridCellArea range)](#clearRange-com.aspose.gridweb.GridCellArea-) | Очищает содержимое и форматирование диапазона. |
| [clearRange(int startRow, int startColumn, int endRow, int endColumn)](#clearRange-int-int-int-int-) | Очищает содержимое и форматирование диапазона. |
| [columnIndexToName(int column)](#columnIndexToName-int-) | Получает имя столбца по индексу столбца. |
| [columnNameToIndex(String columnName)](#columnNameToIndex-java.lang.String-) | Получает индекс столбца по имени столбца. |
| [copyColumn(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex)](#copyColumn-com.aspose.gridweb.GridCells-int-int-) | Копирует данные и форматирование целого столбца. |
| [copyColumns(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)](#copyColumns-com.aspose.gridweb.GridCells-int-int-int-) | Копирует данные и форматирование целого столбца. |
| [copyRow(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex)](#copyRow-com.aspose.gridweb.GridCells-int-int-) | Копирует данные и форматирование целой строки. |
| [copyRows(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)](#copyRows-com.aspose.gridweb.GridCells-int-int-int-) | Копирует данные и форматирование нескольких целых строк. |
| [deleteBlankColumns()](#deleteBlankColumns--) | Удалить все пустые столбцы, которые не содержат никаких данных. |
| [deleteBlankRows()](#deleteBlankRows--) | Удалить все пустые строки, которые не содержат данных. |
| [deleteColumn(int columnIndex)](#deleteColumn-int-) | Удаляет столбец. |
| [deleteColumn(int columnIndex, boolean updateReference)](#deleteColumn-int-boolean-) | Удаляет столбец. |
| [deleteColumns(int columnIndex, int totalColumns, boolean updateReference)](#deleteColumns-int-int-boolean-) | Удаляет несколько столбцов. |
| [deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)](#deleteRange-int-int-int-int-int-) | Удаляет диапазон ячеек и сдвигает ячейки в соответствии с параметром сдвига. |
| [deleteRow(int rowIndex)](#deleteRow-int-) | Удаляет строку. |
| [deleteRows(int rowIndex, int totalRows)](#deleteRows-int-int-) | Удаляет несколько строк. |
| [deleteRows(int rowIndex, int totalRows, boolean updateReference)](#deleteRows-int-int-boolean-) | Удаляет несколько строк в листе. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)](#exportArray-int-int-int-int-) | Экспортирует данные из коллекции [GridCells](../../com.aspose.gridweb/gridcells) в двумерный массив. |
| [get(int row, int column)](#get-int-int-) | Получает элемент [GridCell](../../com.aspose.gridweb/gridcell) по указанным индексам строки и столбца ячейки. |
| [get(String cellName)](#get-java.lang.String-) | Получает элемент [GridCell](../../com.aspose.gridweb/gridcell) по указанному имени ячейки. |
| [getCell(int row, int column)](#getCell-int-int-) | Получает элемент [GridCell](../../com.aspose.gridweb/gridcell) по указанным индексам строки и столбца ячейки. |
| [getClass()](#getClass--) |  |
| [getColumnWidth(int column)](#getColumnWidth-int-) | Получает ширину указанного столбца. |
| [getColumnWidthInch(int column)](#getColumnWidthInch-int-) | Получает ширину указанного столбца в дюймах. |
| [getColumnWidthPixel(int column)](#getColumnWidthPixel-int-) | Получает ширину указанного столбца в пикселях. |
| [getColumns()](#getColumns--) | Получает коллекцию объектов [GridColumn](../../com.aspose.gridweb/gridcolumn), представляющих отдельные столбцы в этом листе. |
| [getCount()](#getCount--) | Получает количество ячеек. |
| [getFirstCell()](#getFirstCell--) | Получает первую ячейку в этом листе. |
| [getLastCell()](#getLastCell--) | Получает последнюю ячейку в этом листе. |
| [getMaxColumn()](#getMaxColumn--) | Максимальный индекс столбца ячейки, содержащей данные или стиль. |
| [getMaxDataColumn()](#getMaxDataColumn--) | Максимальный индекс столбца ячейки, содержащей данные. |
| [getMaxDataRow()](#getMaxDataRow--) | Максимальный индекс строки ячейки, содержащей данные. |
| [getMaxRow()](#getMaxRow--) | Максимальный индекс строки ячейки, содержащей данные или стиль. |
| [getMergedCells()](#getMergedCells--) | Получает коллекцию объединённых ячеек. |
| [getMinColumn()](#getMinColumn--) | Минимальный индекс столбца тех ячеек, которые были созданы в коллекции (не включает столбец, в котором стиль определён для всего столбца, но ни одна ячейка не была создана в нём). |
| [getMinDataColumn()](#getMinDataColumn--) | Минимальный индекс столбца ячейки, содержащей данные. |
| [getMinDataRow()](#getMinDataRow--) | Минимальный индекс строки ячейки, содержащей данные. |
| [getMinRow()](#getMinRow--) | Минимальный индекс строки ячейки, содержащей данные или стиль. |
| [getRow(int i)](#getRow-int-) | Получает элемент [GridRow](../../com.aspose.gridweb/gridrow) по указанному индексу строки ячейки. |
| [getRowEnumerator()](#getRowEnumerator--) | Получает перечислитель строк |
| [getRowHeight(int row)](#getRowHeight-int-) | Получает высоту указанной строки. |
| [getRowHeightInch(int row)](#getRowHeightInch-int-) | Получает высоту указанной строки в единицах дюймов. |
| [getRowHeightPixel(int row)](#getRowHeightPixel-int-) | Получает высоту указанной строки в единицах пикселей. |
| [getRowOutlineLevel(int rowIndex)](#getRowOutlineLevel-int-) | Получает уровень структуры строки. |
| [getRows()](#getRows--) | Получает коллекцию объектов [GridRow](../../com.aspose.gridweb/gridrow), представляющих отдельные строки в этом листе. |
| [getStandardHeight()](#getStandardHeight--) | Получает высоту строки по умолчанию в этом листе, в пунктах. |
| [getStandardHeightPixels()](#getStandardHeightPixels--) | Получает высоту строки по умолчанию в этом листе, в пикселях. |
| [getStandardWidth()](#getStandardWidth--) | Получает ширину столбца по умолчанию в листе, в единицах символов. |
| [getStandardWidthInch()](#getStandardWidthInch--) | Получает ширину столбца по умолчанию в листе в единицах дюймов. |
| [getStandardWidthPixels()](#getStandardWidthPixels--) | Получает ширину столбца по умолчанию в листе в единицах пикселей. |
| [getViewColumnWidthPixel(int column)](#getViewColumnWidthPixel-int-) | Получить ширину в разных типах представления. |
| [groupColumns(int firstIndex, int lastIndex)](#groupColumns-int-int-) | Группирует столбцы. |
| [groupColumns(int firstIndex, int lastIndex, boolean isHidden)](#groupColumns-int-int-boolean-) | Группирует столбцы. |
| [groupRows(int firstIndex, int lastIndex)](#groupRows-int-int-) | Группирует строки. |
| [hashCode()](#hashCode--) |  |
| [hideColumn(int column)](#hideColumn-int-) | Скрывает столбец. |
| [hideRow(int row)](#hideRow-int-) | Скрывает строку. |
| [insertColumn(int columnIndex)](#insertColumn-int-) | Вставляет новый столбец в лист. |
| [insertColumn(int columnIndex, boolean updateReference)](#insertColumn-int-boolean-) | Вставляет новый столбец в лист. |
| [insertColumns(int columnIndex, int totalColumns)](#insertColumns-int-int-) | Вставляет несколько столбцов в лист. |
| [insertColumns(int columnIndex, int totalColumns, boolean updateReference)](#insertColumns-int-int-boolean-) | Вставляет несколько столбцов в лист. |
| [insertRange(GridCellArea area, int shiftType)](#insertRange-com.aspose.gridweb.GridCellArea-int-) | Вставляет диапазон ячеек и сдвигает ячейки в соответствии с параметром сдвига. |
| [insertRange(GridCellArea area, int shiftNumber, int shiftType, boolean updateReference)](#insertRange-com.aspose.gridweb.GridCellArea-int-int-boolean-) | Вставляет диапазон ячеек и сдвигает ячейки в соответствии с параметром сдвига. |
| [insertRow(int rowIndex)](#insertRow-int-) | Вставляет новую строку в лист. |
| [insertRows(int rowIndex, int totalRows)](#insertRows-int-int-) | Вставляет несколько строк в лист. |
| [insertRows(int rowIndex, int totalRows, boolean updateReference)](#insertRows-int-int-boolean-) | Вставляет несколько строк в лист. |
| [isBlankColumn(int columnIndex)](#isBlankColumn-int-) | Проверяет, является ли указанная колонка пустой (не содержит данных). |
| [isColumnHidden(int columnIndex)](#isColumnHidden-int-) | Проверяет, скрыта ли колонка с указанным индексом. |
| [isRowHidden(int rowIndex)](#isRowHidden-int-) | Проверяет, скрыта ли строка с указанным индексом. |
| [iterator()](#iterator--) | Получает перечислитель строк |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#merge-int-int-int-int-) | Объединяет указанный диапазон ячеек в одну ячейку. |
| [moveRange(GridCellArea sourceArea, int destRow, int destColumn)](#moveRange-com.aspose.gridweb.GridCellArea-int-int-) | Перемещает диапазон. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)](#removeDuplicates-int-int-int-int-) | Удалить дублирующие значения в диапазоне. |
| [removeFormulas()](#removeFormulas--) | Удаляет все формулы и заменяет их значением формулы. |
| [setBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, int position, WebBorderStyle borderStyle)](#setBorders-int-int-int-int-int-com.aspose.gridweb.WebBorderStyle-) | Устанавливает границы для диапазона ячеек. |
| [setColumnWidth(int column, double width)](#setColumnWidth-int-double-) | Устанавливает ширину указанного столбца. |
| [setColumnWidthInch(int column, double inches)](#setColumnWidthInch-int-double-) | Устанавливает ширину столбца в дюймах. |
| [setColumnWidthPixel(int column, int pixel)](#setColumnWidthPixel-int-int-) | Устанавливает ширину столбца в пикселях. |
| [setRowHeight(int row, double height)](#setRowHeight-int-double-) | Устанавливает высоту указанной строки. |
| [setRowHeightInch(int row, double inches)](#setRowHeightInch-int-double-) | Устанавливает высоту строки в дюймах. |
| [setRowHeightPixel(int row, int pixels)](#setRowHeightPixel-int-int-) | Устанавливает высоту строки в пикселях. |
| [setRowOutlineLevel(int rowIndex, int outlineLevel)](#setRowOutlineLevel-int-int-) | Устанавливает уровень структуры строки. |
| [setStandardHeight(double value)](#setStandardHeight-double-) | Устанавливает высоту строки по умолчанию в этом листе, в единицах точек. |
| [setStandardHeightPixels(int value)](#setStandardHeightPixels-int-) | Устанавливает высоту строки по умолчанию в этом листе, в единицах пикселей. |
| [setStandardWidth(double value)](#setStandardWidth-double-) | Устанавливает ширину столбца по умолчанию в листе, в единицах символов. |
| [setStandardWidthInch(double value)](#setStandardWidthInch-double-) | Устанавливает ширину столбца по умолчанию в листе, в дюймах. |
| [setStandardWidthPixels(int value)](#setStandardWidthPixels-int-) | Устанавливает ширину столбца по умолчанию в листе, в пикселях. |
| [setStyle(int firstRow, int firstColumn, int rowNumber, int columnNumber, GridTableItemStyle style)](#setStyle-int-int-int-int-com.aspose.gridweb.GridTableItemStyle-) | Устанавливает стиль для указанного диапазона ячеек. |
| [setStyle(String cellRange, GridTableItemStyle style)](#setStyle-java.lang.String-com.aspose.gridweb.GridTableItemStyle-) | Устанавливает стиль для указанного диапазона ячеек. |
| [sort(int startRow, int startColumn, int rows, int columns, int index, boolean isAsending, boolean isCaseSensitive, boolean islefttoright)](#sort-int-int-int-int-int-boolean-boolean-boolean-) | Сортирует данные по возрастанию/убыванию сверху вниз в диапазоне листа по указанному индексу столбца. |
| [sort(int startRow, int startColumn, int rows, int columns, int[] indexes, int[] orders, int orientation, boolean isCaseSensitive)](#sort-int-int-int-int-int---int---int-boolean-) | Сортирует данные по возрастанию/убыванию сверху вниз в диапазоне листа по указанному индексу столбца. |
| [toString()](#toString--) |  |
| [unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#unMerge-int-int-int-int-) | Разъединяет указанный диапазон объединённых ячеек. |
| [ungroupColumns(int firstIndex, int lastIndex)](#ungroupColumns-int-int-) | Разгруппирует столбцы. |
| [ungroupRows(int firstIndex, int lastIndex)](#ungroupRows-int-int-) | Разгруппирует строки. |
| [unhideColumn(int column, double width)](#unhideColumn-int-double-) | Отображает скрытый столбец |
| [unhideRow(int row)](#unhideRow-int-) | Отображает скрытую строку. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### cellIndexToName(int row, int column) {#cellIndexToName-int-int-}
```
public static String cellIndexToName(int row, int column)
```


Получает имя ячейки по её индексам строки и столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |
| столбец | int | Индекс столбца. |

**Returns:**
java.lang.String - Имя ячейки.
### cellNameToIndex(String cellName, int row, int column) {#cellNameToIndex-java.lang.String-int-int-}
```
public static void cellNameToIndex(String cellName, int row, int column)
```


Получает индексы строки и столбца ячейки по её имени.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cellName | java.lang.String | Имя ячейки. |
| строка | int | Индекс выходной строки |
| столбец | int | Индекс выходного столбца |

### checkCell(int row, int column) {#checkCell-int-int-}
```
public GridCell checkCell(int row, int column)
```


Получает элемент [GridCell](../../com.aspose.gridweb/gridcell) или null по указанным индексам строки и столбца ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки |
| столбец | int | Индекс столбца |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - Return GridCell object if a GridCell object exists. Return null if the GridCell does not exist.
### checkColumn(int col) {#checkColumn-int-}
```
public GridColumn checkColumn(int col)
```


Получает элемент [GridColumn](../../com.aspose.gridweb/gridcolumn) или null по указанному индексу столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| col | int | Индекс столбца. |

**Returns:**
[GridColumn](../../com.aspose.gridweb/gridcolumn) - The Column object.
### checkRow(int i) {#checkRow-int-}
```
public GridRow checkRow(int i)
```


Получает элемент [GridRow](../../com.aspose.gridweb/gridrow) или null по указанному индексу строки ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| i | int | Индекс строки |

**Returns:**
[GridRow](../../com.aspose.gridweb/gridrow) - Returns [GridRow](../../com.aspose.gridweb/gridrow) object If the row object does exist, otherwise returns null.
### clear() {#clear--}
```
public void clear()
```


Очистить все ячейки в коллекции.

### clearContents(GridCellArea range) {#clearContents-com.aspose.gridweb.GridCellArea-}
```
public void clearContents(GridCellArea range)
```


Очищает содержимое диапазона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| range | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Диапазон для очистки. |

### clearContents(int startRow, int startColumn, int endRow, int endColumn) {#clearContents-int-int-int-int-}
```
public void clearContents(int startRow, int startColumn, int endRow, int endColumn)
```


Очищает содержимое диапазона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | int | Индекс начальной строки. |
| startColumn | int | Индекс начального столбца. |
| endRow | int | Индекс конечной строки. |
| endColumn | int | Индекс конечного столбца. |

### clearFormats(GridCellArea range) {#clearFormats-com.aspose.gridweb.GridCellArea-}
```
public void clearFormats(GridCellArea range)
```


Очищает форматирование диапазона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| range | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Диапазон для очистки. |

### clearFormats(int startRow, int startColumn, int endRow, int endColumn) {#clearFormats-int-int-int-int-}
```
public void clearFormats(int startRow, int startColumn, int endRow, int endColumn)
```


Очищает форматирование диапазона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | int | Индекс начальной строки. |
| startColumn | int | Индекс начального столбца. |
| endRow | int | Индекс конечной строки. |
| endColumn | int | Индекс конечного столбца. |

### clearRange(GridCellArea range) {#clearRange-com.aspose.gridweb.GridCellArea-}
```
public void clearRange(GridCellArea range)
```


Очищает содержимое и форматирование диапазона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| range | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Диапазон для очистки. |

### clearRange(int startRow, int startColumn, int endRow, int endColumn) {#clearRange-int-int-int-int-}
```
public void clearRange(int startRow, int startColumn, int endRow, int endColumn)
```


Очищает содержимое и форматирование диапазона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | int | Индекс начальной строки. |
| startColumn | int | Индекс начального столбца. |
| endRow | int | Индекс конечной строки. |
| endColumn | int | Индекс конечного столбца. |

### columnIndexToName(int column) {#columnIndexToName-int-}
```
public static String columnIndexToName(int column)
```


Получает имя столбца по индексу столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int | Индекс столбца. |

**Returns:**
java.lang.String - Имя столбца.
### columnNameToIndex(String columnName) {#columnNameToIndex-java.lang.String-}
```
public static int columnNameToIndex(String columnName)
```


Получает индекс столбца по имени столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| columnName | java.lang.String | Имя столбца. |

**Returns:**
int - Индекс столбца.
### copyColumn(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex) {#copyColumn-com.aspose.gridweb.GridCells-int-int-}
```
public void copyColumn(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex)
```


Копирует данные и форматирование целого столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | Объект Source Cells содержит данные и форматирование для копирования. |
| sourceColumnIndex | int | Индекс исходного столбца. |
| destinationColumnIndex | int | Индекс целевого столбца. |

### copyColumns(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber) {#copyColumns-com.aspose.gridweb.GridCells-int-int-int-}
```
public void copyColumns(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)
```


Копирует данные и форматирование целого столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | Объект Source Cells содержит данные и форматирование для копирования. |
| sourceColumnIndex | int | Индекс исходного столбца. |
| destinationColumnIndex | int | Индекс целевого столбца. |
| columnNumber | int | Номер скопированного столбца. |

### copyRow(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex) {#copyRow-com.aspose.gridweb.GridCells-int-int-}
```
public void copyRow(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex)
```


Копирует данные и форматирование целой строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | Объект Source Cells содержит данные и форматирование для копирования. |
| sourceRowIndex | int | Индекс исходной строки. |
| destinationRowIndex | int | Индекс целевой строки. |

### copyRows(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber) {#copyRows-com.aspose.gridweb.GridCells-int-int-int-}
```
public void copyRows(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```


Копирует данные и форматирование нескольких целых строк.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | Объект Source Cells содержит данные и форматирование для копирования. |
| sourceRowIndex | int | Индекс исходной строки. |
| destinationRowIndex | int | Индекс целевой строки. |
| rowNumber | int | Номер скопированной строки. |

### deleteBlankColumns() {#deleteBlankColumns--}
```
public void deleteBlankColumns()
```


Удалить все пустые столбцы, которые не содержат никаких данных.

### deleteBlankRows() {#deleteBlankRows--}
```
public void deleteBlankRows()
```


Удалить все пустые строки, которые не содержат данных.

### deleteColumn(int columnIndex) {#deleteColumn-int-}
```
public void deleteColumn(int columnIndex)
```


Удаляет столбец.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | int | Индекс столбца. |

### deleteColumn(int columnIndex, boolean updateReference) {#deleteColumn-int-boolean-}
```
public void deleteColumn(int columnIndex, boolean updateReference)
```


Удаляет столбец.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | int | Индекс столбца. |
| updateReference | boolean | Указывает, следует ли обновлять ссылки в других листах. |

### deleteColumns(int columnIndex, int totalColumns, boolean updateReference) {#deleteColumns-int-int-boolean-}
```
public void deleteColumns(int columnIndex, int totalColumns, boolean updateReference)
```


Удаляет несколько столбцов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | int | Индекс столбца. |
| totalColumns | int | Количество столбцов, подлежащих удалению. |
| updateReference | boolean | Указывает, следует ли обновлять ссылки в других листах. |

### deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType) {#deleteRange-int-int-int-int-int-}
```
public void deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)
```


Удаляет диапазон ячеек и сдвигает ячейки в соответствии с параметром сдвига.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | int | Индекс начальной строки. |
| startColumn | int | Индекс начального столбца. |
| endRow | int | Индекс конечной строки. |
| endColumn | int | Индекс конечного столбца. |
| shiftType | int | [GridShiftType](../../com.aspose.gridweb/gridshifttype). Параметр смещения ячеек. |

### deleteRow(int rowIndex) {#deleteRow-int-}
```
public void deleteRow(int rowIndex)
```


Удаляет строку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | int | Индекс строки. |

### deleteRows(int rowIndex, int totalRows) {#deleteRows-int-int-}
```
public boolean deleteRows(int rowIndex, int totalRows)
```


Удаляет несколько строк.

**Remarks**

Если удаляемый диапазон содержит верхнюю часть (не полностью) таблицы (ListObject), диапазон не может быть удалён, и ничего не будет сделано. Это работает как в MS Excel.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | int | Индекс первой строки, которая будет удалена. |
| totalRows | int | Количество строк, подлежащих удалению. |

**Returns:**
boolean
### deleteRows(int rowIndex, int totalRows, boolean updateReference) {#deleteRows-int-int-boolean-}
```
public boolean deleteRows(int rowIndex, int totalRows, boolean updateReference)
```


Удаляет несколько строк в листе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | int | Индекс строки. |
| totalRows | int | Количество строк, подлежащих удалению. |
| updateReference | boolean | Указывает, следует ли обновлять ссылки в других листах. |

**Returns:**
boolean -
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
### exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns) {#exportArray-int-int-int-int-}
```
public Object[][] exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Экспортирует данные из коллекции [GridCells](../../com.aspose.gridweb/gridcells) в двумерный массив.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | int | Номер строки первой ячейки для экспорта. |
| firstColumn | int | Номер столбца первой ячейки для экспорта. |
| totalRows | int | Количество строк для экспорта |
| totalColumns | int | Количество столбцов для экспорта |

**Returns:**
java.lang.Object[][] - Объект массива экспортированных значений ячеек.
### get(int row, int column) {#get-int-int-}
```
public GridCell get(int row, int column)
```


Получает элемент [GridCell](../../com.aspose.gridweb/gridcell) по указанным индексам строки и столбца ячейки.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridCells cells = GridWeb1.getWorkSheets().get(0).getCells();
         //Gets the cell at "A1"
         GridCell cell = cells.get(0, 0);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |
| столбец | int | Индекс столбца. |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - The [GridCell](../../com.aspose.gridweb/gridcell) object.
### get(String cellName) {#get-java.lang.String-}
```
public GridCell get(String cellName)
```


Получает элемент [GridCell](../../com.aspose.gridweb/gridcell) по указанному имени ячейки.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
          GridCells cells = GridWeb1.getWorkSheets().get(0).getCells();
          GridCell cell = cells.get("A1");	//Gets the cell at "A1"
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cellName | java.lang.String | Имя ячейки, включающее букву столбца и номер строки, например A5. |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - A [GridCell](../../com.aspose.gridweb/gridcell) object
### getCell(int row, int column) {#getCell-int-int-}
```
public GridCell getCell(int row, int column)
```


Получает элемент [GridCell](../../com.aspose.gridweb/gridcell) по указанным индексам строки и столбца ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки |
| столбец | int | Индекс столбца |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - Return Cell object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnWidth(int column) {#getColumnWidth-int-}
```
public double getColumnWidth(int column)
```


Получает ширину указанного столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int | Индекс столбца |

**Returns:**
double - Ширина столбца
### getColumnWidthInch(int column) {#getColumnWidthInch-int-}
```
public double getColumnWidthInch(int column)
```


Получает ширину указанного столбца в дюймах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int | Индекс столбца |

**Returns:**
double - Ширина столбца
### getColumnWidthPixel(int column) {#getColumnWidthPixel-int-}
```
public int getColumnWidthPixel(int column)
```


Получает ширину указанного столбца в пикселях.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int | Индекс столбца |

**Returns:**
int — ширина столбца в обычном виде.
### getColumns() {#getColumns--}
```
public GridColumnCollection getColumns()
```


Получает коллекцию объектов [GridColumn](../../com.aspose.gridweb/gridcolumn), представляющих отдельные столбцы в этом листе.

**Returns:**
[GridColumnCollection](../../com.aspose.gridweb/gridcolumncollection)
### getCount() {#getCount--}
```
public int getCount()
```


Получает количество ячеек.

**Returns:**
int
### getFirstCell() {#getFirstCell--}
```
public GridCell getFirstCell()
```


Получает первую ячейку в этом листе.

**Remarks**

Возвращает null, если в листе нет данных.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getLastCell() {#getLastCell--}
```
public GridCell getLastCell()
```


Получает последнюю ячейку в этом листе.

**Remarks**

Возвращает null, если в листе нет данных.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


Максимальный индекс столбца ячейки, содержащей данные или стиль.

**Remarks**

Возвращает -1, если ячейка отсутствует.

**Returns:**
int
### getMaxDataColumn() {#getMaxDataColumn--}
```
public int getMaxDataColumn()
```


Максимальный индекс столбца ячейки, содержащей данные.

**Remarks**

\-1 будет возвращено, если нет ячейки, содержащей данные. Это свойство требует перебора и проверки всех ячеек в листе, поэтому процесс затратный по времени и не должен вызываться многократно.

**Returns:**
int
### getMaxDataRow() {#getMaxDataRow--}
```
public int getMaxDataRow()
```


Максимальный индекс строки ячейки, содержащей данные.

**Remarks**

Возвращает -1, если нет ячейки, содержащей данные.

**Returns:**
int
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


Максимальный индекс строки ячейки, содержащей данные или стиль.

**Remarks**

Возвращает -1, если в листе нет ячейки, содержащей данные или стиль.

**Returns:**
int
### getMergedCells() {#getMergedCells--}
```
public ArrayList getMergedCells()
```


Получает коллекцию объединённых ячеек.

**Remarks**

В этой коллекции каждый элемент представляет собой структуру [GridCellArea](../../com.aspose.gridweb/gridcellarea), которая представляет область объединённых ячеек.

**Returns:**
java.util.ArrayList
### getMinColumn() {#getMinColumn--}
```
public int getMinColumn()
```


Минимальный индекс столбца тех ячеек, которые были созданы в коллекции (не включает столбец, в котором стиль определён для всего столбца, но ни одна ячейка не была создана в нём).

**Returns:**
int
### getMinDataColumn() {#getMinDataColumn--}
```
public int getMinDataColumn()
```


Минимальный индекс столбца ячейки, содержащей данные.

**Remarks**

\-1 будет возвращено, если нет ячейки, содержащей данные. Это свойство требует перебора и проверки всех ячеек в листе, поэтому процесс затратный по времени и не должен вызываться многократно.

**Returns:**
int
### getMinDataRow() {#getMinDataRow--}
```
public int getMinDataRow()
```


Минимальный индекс строки ячейки, содержащей данные.

**Returns:**
int
### getMinRow() {#getMinRow--}
```
public int getMinRow()
```


Минимальный индекс строки ячейки, содержащей данные или стиль.

**Returns:**
int
### getRow(int i) {#getRow-int-}
```
public GridRow getRow(int i)
```


Получает элемент [GridRow](../../com.aspose.gridweb/gridrow) по указанному индексу строки ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| i | int | Индекс строки |

**Returns:**
[GridRow](../../com.aspose.gridweb/gridrow) - the row object
### getRowEnumerator() {#getRowEnumerator--}
```
public Iterator getRowEnumerator()
```


Получает перечислитель строк

**Returns:**
java.util.Iterator - Перечислитель строк.
### getRowHeight(int row) {#getRowHeight-int-}
```
public double getRowHeight(int row)
```


Получает высоту указанной строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки |

**Returns:**
double — высота строки
### getRowHeightInch(int row) {#getRowHeightInch-int-}
```
public double getRowHeightInch(int row)
```


Получает высоту указанной строки в единицах дюймов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки |

**Returns:**
double — высота строки
### getRowHeightPixel(int row) {#getRowHeightPixel-int-}
```
public int getRowHeightPixel(int row)
```


Получает высоту указанной строки в единицах пикселей.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки |

**Returns:**
int — высота строки
### getRowOutlineLevel(int rowIndex) {#getRowOutlineLevel-int-}
```
public int getRowOutlineLevel(int rowIndex)
```


Получает уровень структуры строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | int | индекс строки. |

**Returns:**
int - уровень контура.
### getRows() {#getRows--}
```
public GridRowCollection getRows()
```


Получает коллекцию объектов [GridRow](../../com.aspose.gridweb/gridrow), представляющих отдельные строки в этом листе.

**Returns:**
[GridRowCollection](../../com.aspose.gridweb/gridrowcollection)
### getStandardHeight() {#getStandardHeight--}
```
public double getStandardHeight()
```


Получает высоту строки по умолчанию в этом листе, в пунктах.

**Returns:**
double
### getStandardHeightPixels() {#getStandardHeightPixels--}
```
public int getStandardHeightPixels()
```


Получает высоту строки по умолчанию в этом листе, в пикселях.

**Returns:**
int
### getStandardWidth() {#getStandardWidth--}
```
public double getStandardWidth()
```


Получает ширину столбца по умолчанию в листе, в единицах символов.

**Returns:**
double
### getStandardWidthInch() {#getStandardWidthInch--}
```
public double getStandardWidthInch()
```


Получает ширину столбца по умолчанию в листе в единицах дюймов.

**Returns:**
double
### getStandardWidthPixels() {#getStandardWidthPixels--}
```
public int getStandardWidthPixels()
```


Получает ширину столбца по умолчанию в листе в единицах пикселей.

**Returns:**
int
### getViewColumnWidthPixel(int column) {#getViewColumnWidthPixel-int-}
```
public int getViewColumnWidthPixel(int column)
```


Получить ширину в разных типах представления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int | Индекс столбца. |

**Returns:**
int — ширина столбца в пикселях
### groupColumns(int firstIndex, int lastIndex) {#groupColumns-int-int-}
```
public void groupColumns(int firstIndex, int lastIndex)
```


Группирует столбцы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| firstIndex | int | Первый индекс столбца для группировки. |
| lastIndex | int | Последний индекс столбца для группировки. |

### groupColumns(int firstIndex, int lastIndex, boolean isHidden) {#groupColumns-int-int-boolean-}
```
public void groupColumns(int firstIndex, int lastIndex, boolean isHidden)
```


Группирует столбцы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| firstIndex | int | Первый индекс столбца для группировки. |
| lastIndex | int | Последний индекс столбца для группировки. |
| isHidden | boolean | Указывает, скрыты ли сгруппированные столбцы. |

### groupRows(int firstIndex, int lastIndex) {#groupRows-int-int-}
```
public void groupRows(int firstIndex, int lastIndex)
```


Группирует строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| firstIndex | int | Первый индекс строки для группировки. |
| lastIndex | int | Последний индекс строки для группировки. |

### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### hideColumn(int column) {#hideColumn-int-}
```
public void hideColumn(int column)
```


Скрывает столбец.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int | Индекс столбца. |

### hideRow(int row) {#hideRow-int-}
```
public void hideRow(int row)
```


Скрывает строку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |

### insertColumn(int columnIndex) {#insertColumn-int-}
```
public void insertColumn(int columnIndex)
```


Вставляет новый столбец в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | int | Индекс столбца. |

### insertColumn(int columnIndex, boolean updateReference) {#insertColumn-int-boolean-}
```
public void insertColumn(int columnIndex, boolean updateReference)
```


Вставляет новый столбец в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | int | Индекс столбца. |
| updateReference | boolean | Указывает, будут ли ссылки в других листах обновлены. |

### insertColumns(int columnIndex, int totalColumns) {#insertColumns-int-int-}
```
public void insertColumns(int columnIndex, int totalColumns)
```


Вставляет несколько столбцов в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | int | Индекс столбца. |
| totalColumns | int | Количество столбцов. |

### insertColumns(int columnIndex, int totalColumns, boolean updateReference) {#insertColumns-int-int-boolean-}
```
public void insertColumns(int columnIndex, int totalColumns, boolean updateReference)
```


Вставляет несколько столбцов в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | int | Индекс столбца. |
| totalColumns | int | Количество столбцов. |
| updateReference | boolean | Указывает, будут ли ссылки в других листах обновлены. |

### insertRange(GridCellArea area, int shiftType) {#insertRange-com.aspose.gridweb.GridCellArea-int-}
```
public void insertRange(GridCellArea area, int shiftType)
```


Вставляет диапазон ячеек и сдвигает ячейки в соответствии с параметром сдвига.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| area | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Сдвинуть область. |
| shiftType | int | [GridShiftType](../../com.aspose.gridweb/gridshifttype). Параметр смещения ячеек. |

### insertRange(GridCellArea area, int shiftNumber, int shiftType, boolean updateReference) {#insertRange-com.aspose.gridweb.GridCellArea-int-int-boolean-}
```
public void insertRange(GridCellArea area, int shiftNumber, int shiftType, boolean updateReference)
```


Вставляет диапазон ячеек и сдвигает ячейки в соответствии с параметром сдвига.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| area | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Сдвинуть область. |
| shiftNumber | int | Количество строк или столбцов, которые будут вставлены. |
| shiftType | int | [GridShiftType](../../com.aspose.gridweb/gridshifttype). Параметр смещения ячеек. |
| updateReference | boolean | Указывает, следует ли обновлять ссылки в других листах. |

### insertRow(int rowIndex) {#insertRow-int-}
```
public void insertRow(int rowIndex)
```


Вставляет новую строку в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | int | Индекс строки. |

### insertRows(int rowIndex, int totalRows) {#insertRows-int-int-}
```
public void insertRows(int rowIndex, int totalRows)
```


Вставляет несколько строк в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | int | Индекс строки. |
| totalRows | int | Количество строк, которые будут вставлены. |

### insertRows(int rowIndex, int totalRows, boolean updateReference) {#insertRows-int-int-boolean-}
```
public void insertRows(int rowIndex, int totalRows, boolean updateReference)
```


Вставляет несколько строк в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | int | Индекс строки. |
| totalRows | int | Количество строк, которые будут вставлены. |
| updateReference | boolean | Указывает, будут ли ссылки в других листах обновлены. |

### isBlankColumn(int columnIndex) {#isBlankColumn-int-}
```
public boolean isBlankColumn(int columnIndex)
```


Проверяет, является ли указанная колонка пустой (не содержит данных).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | int | индекс столбца |

**Returns:**
boolean - true, если указанный столбец не содержит данных
### isColumnHidden(int columnIndex) {#isColumnHidden-int-}
```
public boolean isColumnHidden(int columnIndex)
```


Проверяет, скрыта ли колонка с указанным индексом.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | int | индекс столбца |

**Returns:**
boolean - true, если столбец скрыт.
### isRowHidden(int rowIndex) {#isRowHidden-int-}
```
public boolean isRowHidden(int rowIndex)
```


Проверяет, скрыта ли строка с указанным индексом.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | int | индекс строки |

**Returns:**
boolean - true, если строка скрыта
### iterator() {#iterator--}
```
public Iterator iterator()
```


Получает перечислитель строк

**Returns:**
java.util.Iterator — перечислитель строк
### merge(int firstRow, int firstColumn, int totalRows, int totalColumns) {#merge-int-int-int-int-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Объединяет указанный диапазон ячеек в одну ячейку.

**Remarks**

Ссылка на объединённую ячейку через адрес верхней‑левой ячейки в диапазоне.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | int | Первая строка этого диапазона(нумерация с нуля) |
| firstColumn | int | Первый столбец этого диапазона(нумерация с нуля) |
| totalRows | int | Количество строк(нумерация с 1) |
| totalColumns | int | Количество столбцов (нумерация с 1) |

### moveRange(GridCellArea sourceArea, int destRow, int destColumn) {#moveRange-com.aspose.gridweb.GridCellArea-int-int-}
```
public void moveRange(GridCellArea sourceArea, int destRow, int destColumn)
```


Перемещает диапазон.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Диапазон, который следует переместить. |
| destRow | int | Строка назначения. |
| destColumn | int | Столбец назначения. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeDuplicates(int startRow, int startColumn, int endRow, int endColumn) {#removeDuplicates-int-int-int-int-}
```
public void removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)
```


Удалить дублирующие значения в диапазоне.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | int | Начальная строка. |
| startColumn | int | Начальный столбец |
| endRow | int | Индекс конечной строки. |
| endColumn | int | Индекс конечного столбца. |

### removeFormulas() {#removeFormulas--}
```
public void removeFormulas()
```


Удаляет все формулы и заменяет их значением формулы.

### setBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, int position, WebBorderStyle borderStyle) {#setBorders-int-int-int-int-int-com.aspose.gridweb.WebBorderStyle-}
```
public void setBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, int position, WebBorderStyle borderStyle)
```


Устанавливает границы для диапазона ячеек.

**Example**

```
           GridWeb GridWeb1 = new GridWeb();
           WebBorderStyle borderStyle1 = new WebBorderStyle();
         	 GridWeb1.getWorkSheets().get(0).getCells().setBorders(0, 0, 5, 8, SetBorderPosition.OUTLINE, borderStyle1);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | int | Первый номер строки диапазона (нумерация с нуля). |
| firstColumn | int | Первый номер столбца диапазона (нумерация с нуля). |
| rowNumber | int | Количество строк. |
| columnNumber | int | Количество столбцов. |
| position | int | [SetBorderPosition](../../com.aspose.gridweb/setborderposition). Позиция границы. |
| borderStyle | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) | Стиль границы. |

### setColumnWidth(int column, double width) {#setColumnWidth-int-double-}
```
public void setColumnWidth(int column, double width)
```


Устанавливает ширину указанного столбца.

**Remarks**

Чтобы скрыть столбец, устанавливает ширину столбца в ноль.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int | Индекс столбца. |
| width | double | Ширина столбца. Ширина столбца должна быть от 0 до 255. |

### setColumnWidthInch(int column, double inches) {#setColumnWidthInch-int-double-}
```
public void setColumnWidthInch(int column, double inches)
```


Устанавливает ширину столбца в дюймах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int | Индекс столбца. |
| дюймы | double | Количество дюймов. |

### setColumnWidthPixel(int column, int pixel) {#setColumnWidthPixel-int-int-}
```
public void setColumnWidthPixel(int column, int pixel)
```


Устанавливает ширину столбца в пикселях.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int | Индекс столбца. |
| пиксель | int | Количество пикселей. |

### setRowHeight(int row, double height) {#setRowHeight-int-double-}
```
public void setRowHeight(int row, double height)
```


Устанавливает высоту указанной строки.

**Remarks**

Чтобы скрыть строку, устанавливает высоту строки в ноль.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |
| height | double | Высота строки. В единицах пунктов. Должна быть от 0 до 409,5. |

### setRowHeightInch(int row, double inches) {#setRowHeightInch-int-double-}
```
public void setRowHeightInch(int row, double inches)
```


Устанавливает высоту строки в дюймах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |
| дюймы | double | Количество дюймов. Должно быть от 0 до 409.5/72. |

### setRowHeightPixel(int row, int pixels) {#setRowHeightPixel-int-int-}
```
public void setRowHeightPixel(int row, int pixels)
```


Устанавливает высоту строки в пикселях.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |
| пиксели | int | Количество пикселей. |

### setRowOutlineLevel(int rowIndex, int outlineLevel) {#setRowOutlineLevel-int-int-}
```
public void setRowOutlineLevel(int rowIndex, int outlineLevel)
```


Устанавливает уровень структуры строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | int | индекс строки. |
| outlineLevel | int | уровень контура. |

### setStandardHeight(double value) {#setStandardHeight-double-}
```
public void setStandardHeight(double value)
```


Устанавливает высоту строки по умолчанию в этом листе, в единицах точек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setStandardHeightPixels(int value) {#setStandardHeightPixels-int-}
```
public void setStandardHeightPixels(int value)
```


Устанавливает высоту строки по умолчанию в этом листе, в единицах пикселей.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setStandardWidth(double value) {#setStandardWidth-double-}
```
public void setStandardWidth(double value)
```


Устанавливает ширину столбца по умолчанию в листе, в единицах символов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setStandardWidthInch(double value) {#setStandardWidthInch-double-}
```
public void setStandardWidthInch(double value)
```


Устанавливает ширину столбца по умолчанию в листе, в дюймах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setStandardWidthPixels(int value) {#setStandardWidthPixels-int-}
```
public void setStandardWidthPixels(int value)
```


Устанавливает ширину столбца по умолчанию в листе, в пикселях.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setStyle(int firstRow, int firstColumn, int rowNumber, int columnNumber, GridTableItemStyle style) {#setStyle-int-int-int-int-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(int firstRow, int firstColumn, int rowNumber, int columnNumber, GridTableItemStyle style)
```


Устанавливает стиль для указанного диапазона ячеек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | int | Первая строка этого диапазона(нумерация с нуля) |
| firstColumn | int | Первый столбец этого диапазона(нумерация с нуля) |
| rowNumber | int | Количество строк(нумерация с 1) |
| columnNumber | int | Количество столбцов (нумерация с 1) |
| style | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Объект стиля, который будет установлен |

### setStyle(String cellRange, GridTableItemStyle style) {#setStyle-java.lang.String-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(String cellRange, GridTableItemStyle style)
```


Устанавливает стиль для указанного диапазона ячеек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cellRange | java.lang.String | Диапазон имён ячеек, например "A1:D6" |
| style | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Объект стиля, который будет установлен |

### sort(int startRow, int startColumn, int rows, int columns, int index, boolean isAsending, boolean isCaseSensitive, boolean islefttoright) {#sort-int-int-int-int-int-boolean-boolean-boolean-}
```
public void sort(int startRow, int startColumn, int rows, int columns, int index, boolean isAsending, boolean isCaseSensitive, boolean islefttoright)
```


Сортирует данные по возрастанию/убыванию сверху вниз в диапазоне листа по указанному индексу столбца. Сортирует данные по возрастанию/убыванию слева направо в диапазоне листа по указанному индексу строки.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridWeb1.getWorkSheets().get(0).getCells().sort(1,0,25,6,3,true,true,false);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | int | Номер строки первой ячейки для сортировки. |
| startColumn | int | Номер столбца первой ячейки для сортировки. |
| строки | int | Количество строк для импорта. |
| столбцы | int | Количество столбцов для импорта. |
| индекс | int | Индекс столбца, указывающий сортируемый столбец. Если ориентация сверху вниз, он обозначает индекс столбца, указывающий сортируемый столбец. Если ориентация слева направо, он обозначает индекс строки, указывающий сортируемую строку. |
| isAsending | boolean | является ли порядок сортировки восходящим . |
| isCaseSensitive | boolean | является ли сортировка чувствительной к регистру . |
| islefttoright | boolean | является ли ориентация сортировки слева направо |

### sort(int startRow, int startColumn, int rows, int columns, int[] indexes, int[] orders, int orientation, boolean isCaseSensitive) {#sort-int-int-int-int-int---int---int-boolean-}
```
public void sort(int startRow, int startColumn, int rows, int columns, int[] indexes, int[] orders, int orientation, boolean isCaseSensitive)
```


Сортирует данные по возрастанию/убыванию сверху вниз в диапазоне листа по указанному индексу столбца. Сортирует данные по возрастанию/убыванию слева направо в диапазоне листа по указанному индексу строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | int | Номер строки первой ячейки для сортировки. |
| startColumn | int | Номер столбца первой ячейки для сортировки. |
| строки | int | Количество строк для импорта. |
| столбцы | int | Количество столбцов для импорта. |
| indexes | int[] | Массив индексов столбцов, указывающий столбец сортировки. Если ориентация сверху вниз, он представляет индекс столбца, указывающий столбец сортировки. Если ориентация слева направо, он представляет индекс строки, указывающий строку сортировки. |
| orders | int[] | [SortByOrder](../../com.aspose.gridweb/sortbyorder). массив порядка сортировки . |
| orientation | int | [SortOrientation](../../com.aspose.gridweb/sortorientation). ориентация сортировки |
| isCaseSensitive | boolean | является ли сортировка чувствительной к регистру . |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns) {#unMerge-int-int-int-int-}
```
public void unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Разъединяет указанный диапазон объединённых ячеек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | int | Первая строка этого диапазона(нумерация с нуля) |
| firstColumn | int | Первый столбец этого диапазона(нумерация с нуля) |
| totalRows | int | Количество строк(нумерация с 1) |
| totalColumns | int | Количество столбцов (нумерация с 1) |

### ungroupColumns(int firstIndex, int lastIndex) {#ungroupColumns-int-int-}
```
public void ungroupColumns(int firstIndex, int lastIndex)
```


Разгруппирует столбцы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| firstIndex | int | Индекс первого столбца, который нужно разгруппировать. |
| lastIndex | int | Индекс последнего столбца, который нужно разгруппировать. |

### ungroupRows(int firstIndex, int lastIndex) {#ungroupRows-int-int-}
```
public void ungroupRows(int firstIndex, int lastIndex)
```


Разгруппирует строки.

**Remarks**

Только удаляет внешнюю информацию о группе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| firstIndex | int | Индекс первой строки, которую нужно разгруппировать. |
| lastIndex | int | Индекс последней строки, которую нужно разгруппировать. |

### unhideColumn(int column, double width) {#unhideColumn-int-double-}
```
public void unhideColumn(int column, double width)
```


Отображает скрытый столбец

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int | Индекс столбца. |
| width | double | Ширина столбца..Ширина столбца должна быть от 0 до 255 |

### unhideRow(int row) {#unhideRow-int-}
```
public void unhideRow(int row)
```


Отображает скрытую строку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |

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

