---
title: "Cells"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует коллекцию объектов, связанных с ячейками, таких как   ...и т.д."
type: docs
url: /ru/java/com.aspose.cells/cells/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Cells implements Iterable
```

Инкапсулирует коллекцию объектов, связанных с ячейками, таких как [Cell](../../com.aspose.cells/cell), [Row](../../com.aspose.cells/row), ...и т.д.

**Remarks**

**Example**

```
         Workbook excel = new Workbook();
         	Cells cells = excel.getWorksheets().get(0).getCells();
 
         	//Set default row height
         	cells.setStandardHeight(20);
         	//Set row height
         	cells.setRowHeight(2, 20.5);
 
         	//Set default colum width
         	cells.setStandardWidth(15);
         	//Set column width
         	cells.setColumnWidth(3, 12.57);
 
         	//Merge cells
         	cells.merge(5, 4, 2, 2);
 
         	//Put values to cells
         	cells.get(0, 0).putValue(true);
         	cells.get(0, 1).putValue(1);
         	cells.get(0, 2).putValue("abc");
 
         //Export data
         Object[][] arr = cells.exportArray(0, 0, 10, 10);
```
## Методы

| Метод | Описание |
| --- | --- |
| [addRange(Range rangeObject)](#addRange-com.aspose.cells.Range-) | Добавляет ссылку на объект диапазона в ячейки |
| [applyColumnStyle(int column, Style style, StyleFlag flag)](#applyColumnStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Применяет форматы ко всему столбцу. |
| [applyRowStyle(int row, Style style, StyleFlag flag)](#applyRowStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Применяет форматирование ко всей строке. |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Применяет форматы ко всему листу. |
| [checkCell(int row, int column)](#checkCell-int-int-) | Получает элемент [Cell](../../com.aspose.cells/cell) или null по указанному индексу строки ячейки и индексу столбца. |
| [checkColumn(int columnIndex)](#checkColumn-int-) | Получает элемент [Column](../../com.aspose.cells/column) или null по указанному индексу столбца. |
| [checkRow(int row)](#checkRow-int-) | Получает элемент [Row](../../com.aspose.cells/row) или null по указанному индексу строки ячейки. |
| [clear()](#clear--) | Очищает все данные листа. |
| [clearContents(CellArea range)](#clearContents-com.aspose.cells.CellArea-) | Очищает содержимое диапазона. |
| [clearContents(int startRow, int startColumn, int endRow, int endColumn)](#clearContents-int-int-int-int-) | Очищает содержимое диапазона. |
| [clearFormats(CellArea range)](#clearFormats-com.aspose.cells.CellArea-) | Очищает форматирование диапазона. |
| [clearFormats(int startRow, int startColumn, int endRow, int endColumn)](#clearFormats-int-int-int-int-) | Очищает форматирование диапазона. |
| [clearMergedCells()](#clearMergedCells--) | Очищает все объединённые диапазоны. |
| [clearRange(CellArea range)](#clearRange-com.aspose.cells.CellArea-) | Очищает содержимое и форматирование диапазона. |
| [clearRange(int startRow, int startColumn, int endRow, int endColumn)](#clearRange-int-int-int-int-) | Очищает содержимое и форматирование диапазона. |
| [convertStringToNumericValue()](#convertStringToNumericValue--) | Преобразует все строковые данные в листе в числовые значения, если это возможно. |
| [copyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex)](#copyColumn-com.aspose.cells.Cells-int-int-) | Копирует данные и форматы целого столбца. |
| [copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)](#copyColumns-com.aspose.cells.Cells-int-int-int-) | Копирует данные и форматы целых столбцов. |
| [copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber, PasteOptions pasteOptions)](#copyColumns-com.aspose.cells.Cells-int-int-int-com.aspose.cells.PasteOptions-) | Копирует данные и форматы целого столбца. |
| [copyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, int destinationColumnIndex, int destinationTotalColumns)](#copyColumns-com.aspose.cells.Cells-int-int-int-int-) | Копирует данные и форматы всех столбцов. |
| [copyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex)](#copyRow-com.aspose.cells.Cells-int-int-) | Копирует данные и форматы целой строки. |
| [copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)](#copyRows-com.aspose.cells.Cells-int-int-int-) | Копирует данные и форматы некоторых целых строк. |
| [copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions)](#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-) | Копирует данные и форматы некоторых целых строк. |
| [copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)](#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-com.aspose.cells.PasteOptions-) | Копирует данные и форматы некоторых целых строк. |
| [createRange(int firstIndex, int number, boolean isVertical)](#createRange-int-int-boolean-) | Создаёт объект [Range](../../com.aspose.cells/range) из строк ячеек или столбцов ячеек. |
| [createRange(int firstRow, int firstColumn, int totalRows, int totalColumns)](#createRange-int-int-int-int-) | Создаёт объект [Range](../../com.aspose.cells/range) из диапазона ячеек. |
| [createRange(String address)](#createRange-java.lang.String-) | Создаёт объект [Range](../../com.aspose.cells/range) из адреса диапазона. |
| [createRange(String upperLeftCell, String lowerRightCell)](#createRange-java.lang.String-java.lang.String-) | Создаёт объект [Range](../../com.aspose.cells/range) из диапазона ячеек. |
| [deleteBlankColumns()](#deleteBlankColumns--) | Удалить все пустые столбцы, которые не содержат никаких данных. |
| [deleteBlankColumns(DeleteOptions options)](#deleteBlankColumns-com.aspose.cells.DeleteOptions-) | Удалить все пустые столбцы, которые не содержат никаких данных. |
| [deleteBlankRows()](#deleteBlankRows--) | Удалить все пустые строки, которые не содержат никаких данных или других объектов. |
| [deleteBlankRows(DeleteOptions options)](#deleteBlankRows-com.aspose.cells.DeleteOptions-) | Удалить все пустые строки, которые не содержат никаких данных или некоторых специальных объектов, таких как видимый комментарий, сводная таблица. |
| [deleteColumn(int columnIndex)](#deleteColumn-int-) | Удаляет столбец. |
| [deleteColumn(int columnIndex, boolean updateReference)](#deleteColumn-int-boolean-) | Удаляет столбец. |
| [deleteColumns(int columnIndex, int totalColumns, boolean updateReference)](#deleteColumns-int-int-boolean-) | Удаляет несколько столбцов. |
| [deleteColumns(int columnIndex, int totalColumns, DeleteOptions options)](#deleteColumns-int-int-com.aspose.cells.DeleteOptions-) | Удаляет несколько столбцов. |
| [deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)](#deleteRange-int-int-int-int-int-) | Удаляет диапазон ячеек и сдвигает ячейки в соответствии с параметром сдвига. |
| [deleteRow(int rowIndex)](#deleteRow-int-) | Удаляет строку. |
| [deleteRow(int rowIndex, boolean updateReference)](#deleteRow-int-boolean-) | Удаляет строку. |
| [deleteRows(int rowIndex, int totalRows)](#deleteRows-int-int-) | Удаляет несколько строк. |
| [deleteRows(int rowIndex, int totalRows, boolean updateReference)](#deleteRows-int-int-boolean-) | Удаляет несколько строк в листе. |
| [deleteRows(int rowIndex, int totalRows, DeleteOptions options)](#deleteRows-int-int-com.aspose.cells.DeleteOptions-) | Удаляет несколько строк в листе. |
| [dispose()](#dispose--) | Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [endCellInColumn(int columnIndex)](#endCellInColumn-int-) | Получает последнюю ячейку в этом столбце. |
| [endCellInColumn(int startRow, int endRow, int startColumn, int endColumn)](#endCellInColumn-int-int-int-int-) | Получает последнюю ячейку с максимальным индексом столбца в этом диапазоне. |
| [endCellInRow(int rowIndex)](#endCellInRow-int-) | Получает последнюю ячейку в этой строке. |
| [endCellInRow(int startRow, int endRow, int startColumn, int endColumn)](#endCellInRow-int-int-int-int-) | Получает последнюю ячейку с максимальным индексом строки в этом диапазоне. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)](#exportArray-int-int-int-int-) | Экспортирует данные из коллекции [Cells](../../com.aspose.cells/cells) в двумерный массив. |
| [exportTypeArray(int firstRow, int firstColumn, int totalRows, int totalColumns)](#exportTypeArray-int-int-int-int-) | Экспортирует тип значения ячейки из коллекции [Cells](../../com.aspose.cells/cells) в двумерный массив. |
| [find(Object what, Cell previousCell)](#find-java.lang.Object-com.aspose.cells.Cell-) | Находит ячейку, содержащую входной объект. |
| [find(Object what, Cell previousCell, FindOptions findOptions)](#find-java.lang.Object-com.aspose.cells.Cell-com.aspose.cells.FindOptions-) | Находит ячейку, содержащую входной объект. |
| [get(int row, int column)](#get-int-int-) | Получает элемент [Cell](../../com.aspose.cells/cell) по указанному индексу строки и индексу столбца ячейки. |
| [get(String cellName)](#get-java.lang.String-) | Получает элемент [Cell](../../com.aspose.cells/cell) по указанному имени ячейки. |
| [getCellDisplayStyle(int row, int column)](#getCellDisplayStyle-int-int-) | Получить стиль отображения заданной ячейки. |
| [getCellDisplayStyle(int row, int column, int adjacentBorders)](#getCellDisplayStyle-int-int-int-) | Получить стиль отображения заданной ячейки. |
| [getCellStyle(int row, int column)](#getCellStyle-int-int-) | Получить стиль заданной ячейки. |
| [getCellsWithPlaceInCellPicture()](#getCellsWithPlaceInCellPicture--) | Получает все ячейки, содержащие встроенное изображение. |
| [getClass()](#getClass--) |  |
| [getColumnOriginalWidthPoint(int column)](#getColumnOriginalWidthPoint-int-) | Получает исходную высоту столбца в пунктах, если столбец скрыт |
| [getColumnWidth(int column)](#getColumnWidth-int-) | Получает ширину (в единицах символов) указанного столбца в обычном виде |
| [getColumnWidth(int column, boolean isOriginal, int unitType)](#getColumnWidth-int-boolean-int-) | Получает ширину столбца. |
| [getColumnWidthInch(int column)](#getColumnWidthInch-int-) | Получает ширину указанного столбца в обычном виде, в дюймах. |
| [getColumnWidthPixel(int column)](#getColumnWidthPixel-int-) | Получает ширину указанного столбца в обычном виде, в пикселях. |
| [getColumnWidthPixel(int column, boolean original)](#getColumnWidthPixel-int-boolean-) | Получает ширину указанного столбца в обычном виде, в пикселях. |
| [getColumns()](#getColumns--) | Получает коллекцию объектов [Column](../../com.aspose.cells/column), представляющих отдельные столбцы в этом листе. |
| [getCount()](#getCount--) | Получает общее количество созданных объектов Cell. |
| [getCountLarge()](#getCountLarge--) | Получает общее количество созданных объектов Cell. |
| [getDependents(boolean isAll, int row, int column)](#getDependents-boolean-int-int-) | Получить все ячейки, которые ссылаются на конкретную ячейку. |
| [getDependentsInCalculation(int row, int column, boolean recursive)](#getDependentsInCalculation-int-int-boolean-) | Получает все ячейки, расчётный результат которых зависит от конкретной ячейки. |
| [getFirstCell()](#getFirstCell--) | Получает первую ячейку в этом листе. |
| [getFirstDataRow(int column)](#getFirstDataRow-int-) | Получает индекс первой строки ячейки, содержащей данные в указанном столбце. |
| [getGroupedColumnOutlineLevel(int columnIndex)](#getGroupedColumnOutlineLevel-int-) | Получает уровень структуры (нумерация с нуля) столбца. |
| [getGroupedRowOutlineLevel(int rowIndex)](#getGroupedRowOutlineLevel-int-) | Получает уровень структуры (нумерация с нуля) строки. |
| [getLastCell()](#getLastCell--) | Получает последнюю ячейку в этом листе. |
| [getLastDataRow(int column)](#getLastDataRow-int-) | Получает индекс последней строки ячейки, содержащей данные в указанном столбце. |
| [getMaxColumn()](#getMaxColumn--) | Максимальный индекс столбца среди ячеек, созданных в коллекции (не включает столбец, для которого определён стиль целого столбца, но в нём не создано ни одной ячейки). |
| [getMaxDataColumn()](#getMaxDataColumn--) | Максимальный индекс столбца ячейки, содержащей данные. |
| [getMaxDataRow()](#getMaxDataRow--) | Максимальный индекс строки ячейки, содержащей данные. |
| [getMaxDisplayRange()](#getMaxDisplayRange--) | Получает максимальный диапазон, включающий данные, объединённые ячейки и фигуры. |
| [getMaxGroupedColumnOutlineLevel()](#getMaxGroupedColumnOutlineLevel--) | Получает максимальный уровень структуры сгруппированных столбцов (нумерация с нуля). |
| [getMaxGroupedRowOutlineLevel()](#getMaxGroupedRowOutlineLevel--) | Получает максимальный уровень структуры сгруппированных строк (нумерация с нуля). |
| [getMaxRow()](#getMaxRow--) | Максимальный индекс строки ячейки, содержащей данные или стиль. |
| [getMemorySetting()](#getMemorySetting--) | Получает параметр использования памяти для этих ячеек. |
| [getMergedAreas()](#getMergedAreas--) | Получает все объединённые ячейки. |
| [getMergedCells()](#getMergedCells--) | Получает коллекцию объединённых ячеек. |
| [getMinColumn()](#getMinColumn--) | Минимальный индекс столбца тех ячеек, которые были созданы в коллекции (не включает столбец, в котором стиль определён для всего столбца, но ни одна ячейка не была создана в нём). |
| [getMinDataColumn()](#getMinDataColumn--) | Минимальный индекс столбца ячейки, содержащей данные. |
| [getMinDataRow()](#getMinDataRow--) | Минимальный индекс строки ячейки, содержащей данные. |
| [getMinRow()](#getMinRow--) | Минимальный индекс строки ячейки, содержащей данные или стиль. |
| [getMultiThreadReading()](#getMultiThreadReading--) | Получает, поддерживает ли модель данных ячеек многопоточное чтение. |
| [getOdsCellFields()](#getOdsCellFields--) | Получает список полей ods. |
| [getPreserveString()](#getPreserveString--) | Получает значение, указывающее, сохраняются ли все значения листа в виде строк. |
| [getRanges()](#getRanges--) | Получает коллекцию объектов [Range](../../com.aspose.cells/range), созданных во время выполнения. |
| [getRowEnumerator()](#getRowEnumerator--) | Получает перечислитель строк. |
| [getRowHeight(int row)](#getRowHeight-int-) | Получает высоту указанной строки в единицах пунктов. |
| [getRowHeight(int row, boolean isOriginal, int unitType)](#getRowHeight-int-boolean-int-) | Получает высоту строки. |
| [getRowHeightInch(int row)](#getRowHeightInch-int-) | Получает высоту указанной строки в единицах дюймов. |
| [getRowHeightPixel(int row)](#getRowHeightPixel-int-) | Получает высоту указанной строки в единицах пикселей. |
| [getRowOriginalHeightPoint(int row)](#getRowOriginalHeightPoint-int-) | Получает оригинальную высоту строки в единицах пунктов, если строка скрыта. |
| [getRows()](#getRows--) | Получает коллекцию объектов [Row](../../com.aspose.cells/row), представляющих отдельные строки в этом листе. |
| [getStandardHeight()](#getStandardHeight--) | Получает высоту строки по умолчанию в этом листе в единицах пунктов. |
| [getStandardHeightInch()](#getStandardHeightInch--) | Получает высоту строки по умолчанию в этом листе в единицах дюймов. |
| [getStandardHeightPixels()](#getStandardHeightPixels--) | Получает высоту строки по умолчанию в этом листе в единицах пикселей. |
| [getStandardWidth()](#getStandardWidth--) | Получает ширину столбца по умолчанию в листе в единицах символов. |
| [getStandardWidthInch()](#getStandardWidthInch--) | Получает ширину столбца по умолчанию в листе в единицах дюймов. |
| [getStandardWidthPixels()](#getStandardWidthPixels--) | Получает ширину столбца по умолчанию в листе в единицах пикселей. |
| [getStyle()](#getStyle--) | Получает стиль по умолчанию листа. |
| [getViewColumnWidthPixel(int column)](#getViewColumnWidthPixel-int-) | Получить ширину в разных типах представления. |
| [getViewRowHeight(int row)](#getViewRowHeight-int-) | Получает высоту указанной строки. |
| [getViewRowHeightInch(int row)](#getViewRowHeightInch-int-) | Получает высоту указанной строки в единицах дюймов. |
| [groupColumns(int firstIndex, int lastIndex)](#groupColumns-int-int-) | Группирует столбцы. |
| [groupColumns(int firstIndex, int lastIndex, boolean isHidden)](#groupColumns-int-int-boolean-) | Группирует столбцы. |
| [groupRows(int firstIndex, int lastIndex)](#groupRows-int-int-) | Группирует строки. |
| [groupRows(int firstIndex, int lastIndex, boolean isHidden)](#groupRows-int-int-boolean-) | Группирует строки. |
| [hashCode()](#hashCode--) |  |
| [hideColumn(int column)](#hideColumn-int-) | Скрывает столбец. |
| [hideColumns(int column, int totalColumns)](#hideColumns-int-int-) | Скрывает несколько столбцов. |
| [hideGroupDetail(boolean isVertical, int index)](#hideGroupDetail-boolean-int-) | Сворачивает сгруппированные строки/столбцы. |
| [hideRow(int row)](#hideRow-int-) | Скрывает строку. |
| [hideRows(int row, int totalRows)](#hideRows-int-int-) | Скрывает несколько строк. |
| [importArray(double[] doubleArray, int firstRow, int firstColumn, boolean isVertical)](#importArray-double---int-int-boolean-) | Импортирует массив double в лист. |
| [importArray(double[][] doubleArray, int firstRow, int firstColumn)](#importArray-double-----int-int-) | Импортирует двумерный массив double в лист. |
| [importArray(int[] intArray, int firstRow, int firstColumn, boolean isVertical)](#importArray-int---int-int-boolean-) | Импортирует массив integer в лист. |
| [importArray(int[][] intArray, int firstRow, int firstColumn)](#importArray-int-----int-int-) | Импортирует двумерный массив integer в лист. |
| [importArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)](#importArray-java.lang.String---int-int-boolean-) | Импортирует массив string в лист. |
| [importArray(String[][] stringArray, int firstRow, int firstColumn)](#importArray-java.lang.String-----int-int-) | Импортирует двумерный массив string в лист. |
| [importArrayList(ArrayList arrayList, int firstRow, int firstColumn, boolean isVertical)](#importArrayList-java.util.ArrayList-int-int-boolean-) | Импортирует ArrayList данных в лист. |
| [importCSV(InputStream stream, TxtLoadOptions options, int firstRow, int firstColumn)](#importCSV-java.io.InputStream-com.aspose.cells.TxtLoadOptions-int-int-) | Импортирует CSV‑файл в ячейки. |
| [importCSV(InputStream stream, String splitter, boolean convertNumericData, int firstRow, int firstColumn)](#importCSV-java.io.InputStream-java.lang.String-boolean-int-int-) | Импортирует CSV‑файл в ячейки. |
| [importCSV(String fileName, TxtLoadOptions options, int firstRow, int firstColumn)](#importCSV-java.lang.String-com.aspose.cells.TxtLoadOptions-int-int-) | Импортирует CSV‑файл в ячейки. |
| [importCSV(String fileName, String splitter, boolean convertNumericData, int firstRow, int firstColumn)](#importCSV-java.lang.String-java.lang.String-boolean-int-int-) | Импортирует CSV‑файл в ячейки. |
| [importCustomObjects(Collection list, int firstRow, int firstColumn, ImportTableOptions options)](#importCustomObjects-java.util.Collection-int-int-com.aspose.cells.ImportTableOptions-) | Импортирует пользовательские объекты. |
| [importCustomObjects(Collection list, String[] propertyNames, boolean isPropertyNameShown, int firstRow, int firstColumn, int rowNumber, boolean insertRows, String dateFormatString, boolean convertStringToNumber)](#importCustomObjects-java.util.Collection-java.lang.String---boolean-int-int-int-boolean-java.lang.String-boolean-) | Импортирует пользовательские объекты. |
| [importData(ICellsDataTable table, int firstRow, int firstColumn, ImportTableOptions options)](#importData-com.aspose.cells.ICellsDataTable-int-int-com.aspose.cells.ImportTableOptions-) | Импортирует данные из пользовательской таблицы данных. |
| [importFormulaArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)](#importFormulaArray-java.lang.String---int-int-boolean-) | Импортирует массив формул в лист. |
| [importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical)](#importObjectArray-java.lang.Object---int-int-boolean-) | Импортирует массив данных в лист. |
| [importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical, int skip)](#importObjectArray-java.lang.Object---int-int-boolean-int-) | Импортирует массив данных в лист. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-int-int-boolean-) | Импортирует данные из объекта ResultSet в лист. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)](#importResultSet-java.sql.ResultSet-int-int-boolean-java.lang.String-boolean-) | Импортирует данные из объекта ResultSet в лист. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, ImportTableOptions options)](#importResultSet-java.sql.ResultSet-int-int-com.aspose.cells.ImportTableOptions-) | Импортирует данные из объекта ResultSet в лист. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-) | Импортирует данные из объекта ResultSet в лист. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)](#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-java.lang.String-boolean-) | Импортирует данные из объекта ResultSet в лист. |
| [importResultSet(ResultSet rs, String startCell, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-java.lang.String-boolean-) | Импортирует данные из объекта ResultSet в лист. |
| [importResultSet(ResultSet rs, String startCell, ImportTableOptions options)](#importResultSet-java.sql.ResultSet-java.lang.String-com.aspose.cells.ImportTableOptions-) | Импортирует данные из объекта ResultSet в лист. |
| [importResultSet(ResultSet rs, String startCell, int rowNum, int columnNum, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-java.lang.String-int-int-boolean-) | Импортирует данные из объекта ResultSet в лист. |
| [importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn)](#importTwoDimensionArray-java.lang.Object-----int-int-) | Импортирует двумерный массив данных в лист. |
| [importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn, boolean convertStringToNumber)](#importTwoDimensionArray-java.lang.Object-----int-int-boolean-) | Импортирует двумерный массив данных в лист. |
| [importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, boolean convertStringToNumber)](#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-boolean-) | Импортирует двумерный массив данных в лист. |
| [importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, TxtLoadOptions opts)](#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-com.aspose.cells.TxtLoadOptions-) | Импортирует двумерный массив данных в лист. |
| [insertColumn(int columnIndex)](#insertColumn-int-) | Вставляет новый столбец в лист. |
| [insertColumn(int columnIndex, boolean updateReference)](#insertColumn-int-boolean-) | Вставляет новый столбец в лист. |
| [insertColumns(int columnIndex, int totalColumns)](#insertColumns-int-int-) | Вставляет несколько столбцов в лист. |
| [insertColumns(int columnIndex, int totalColumns, boolean updateReference)](#insertColumns-int-int-boolean-) | Вставляет несколько столбцов в лист. |
| [insertColumns(int columnIndex, int totalColumns, InsertOptions options)](#insertColumns-int-int-com.aspose.cells.InsertOptions-) | Вставляет несколько столбцов в лист. |
| [insertCutCells(Range cutRange, int row, int column, int shiftType)](#insertCutCells-com.aspose.cells.Range-int-int-int-) | Вставить вырезанный диапазон. |
| [insertRange(CellArea area, int shiftType)](#insertRange-com.aspose.cells.CellArea-int-) | Вставляет диапазон ячеек и сдвигает ячейки в соответствии с параметром сдвига. |
| [insertRange(CellArea area, int shiftNumber, int shiftType)](#insertRange-com.aspose.cells.CellArea-int-int-) | Вставляет диапазон ячеек и сдвигает ячейки в соответствии с параметром сдвига. |
| [insertRange(CellArea area, int shiftNumber, int shiftType, boolean updateReference)](#insertRange-com.aspose.cells.CellArea-int-int-boolean-) | Вставляет диапазон ячеек и сдвигает ячейки в соответствии с параметром сдвига. |
| [insertRow(int rowIndex)](#insertRow-int-) | Вставляет новую строку в лист. |
| [insertRows(int rowIndex, int totalRows)](#insertRows-int-int-) | Вставляет несколько строк в лист. |
| [insertRows(int rowIndex, int totalRows, boolean updateReference)](#insertRows-int-int-boolean-) | Вставляет несколько строк в лист. |
| [insertRows(int rowIndex, int totalRows, InsertOptions options)](#insertRows-int-int-com.aspose.cells.InsertOptions-) | Вставляет несколько строк в лист. |
| [isBlankColumn(int columnIndex)](#isBlankColumn-int-) | Проверяет, является ли указанная колонка пустой (не содержит данных). |
| [isColumnHidden(int columnIndex)](#isColumnHidden-int-) | Проверяет, скрыта ли колонка с указанным индексом. |
| [isDefaultColumnHidden()](#isDefaultColumnHidden--) |  |
| [isDefaultRowHeightMatched()](#isDefaultRowHeightMatched--) | Указывает, что высота строки и высота шрифта по умолчанию совпадают |
| [isDefaultRowHidden()](#isDefaultRowHidden--) | Указывает, скрыта ли строка по умолчанию. |
| [isDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns)](#isDeletingRangeEnabled-int-int-int-int-) | Проверьте, может ли диапазон быть удалён. |
| [isRowHidden(int rowIndex)](#isRowHidden-int-) | Проверяет, скрыта ли строка с указанным индексом. |
| [iterator()](#iterator--) | Получает перечислитель ячеек. |
| [linkToXmlMap(String mapName, int row, int column, String path)](#linkToXmlMap-java.lang.String-int-int-java.lang.String-) | Ссылка на XML‑карту. |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#merge-int-int-int-int-) | Объединяет указанный диапазон ячеек в одну ячейку. |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean mergeConflict)](#merge-int-int-int-int-boolean-) | Объединяет указанный диапазон ячеек в одну ячейку. |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean checkConflict, boolean mergeConflict)](#merge-int-int-int-int-boolean-boolean-) | Объединяет указанный диапазон ячеек в одну ячейку. |
| [moveRange(CellArea sourceArea, int destRow, int destColumn)](#moveRange-com.aspose.cells.CellArea-int-int-) | Перемещает диапазон. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeDuplicates()](#removeDuplicates--) | Удаляет дублирующиеся строки на листе. |
| [removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)](#removeDuplicates-int-int-int-int-) | Удаляет дублирующиеся значения в диапазоне. |
| [removeDuplicates(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders, int[] columnOffsets)](#removeDuplicates-int-int-int-int-boolean-int---) | Удаляет дублирующиеся данные диапазона. |
| [removeFormulas()](#removeFormulas--) | Удаляет все формулы и заменяет их значением формулы. |
| [retrieveSubtotalSetting(CellArea ca)](#retrieveSubtotalSetting-com.aspose.cells.CellArea-) | Получает настройки промежуточных итогов диапазона. |
| [setColumnWidth(int column, double width)](#setColumnWidth-int-double-) | Устанавливает ширину указанной колонки в обычном виде. |
| [setColumnWidthInch(int column, double inches)](#setColumnWidthInch-int-double-) | Устанавливает ширину колонки в дюймах в обычном виде. |
| [setColumnWidthPixel(int column, int pixels)](#setColumnWidthPixel-int-int-) | Устанавливает ширину колонки в пикселях в обычном виде. |
| [setDefaultColumnHidden(boolean value)](#setDefaultColumnHidden-boolean-) |  |
| [setDefaultRowHeightMatched(boolean value)](#setDefaultRowHeightMatched-boolean-) | Указывает, что высота строки и высота шрифта по умолчанию совпадают |
| [setDefaultRowHidden(boolean value)](#setDefaultRowHidden-boolean-) | Указывает, скрыта ли строка по умолчанию. |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Устанавливает параметр использования памяти для этих ячеек. |
| [setMultiThreadReading(boolean value)](#setMultiThreadReading-boolean-) | Устанавливает, должна ли модель данных ячеек поддерживать многопоточное чтение. |
| [setPreserveString(boolean value)](#setPreserveString-boolean-) | Устанавливает значение, указывающее, сохраняются ли все значения листа как строки. |
| [setRowHeight(int row, double height)](#setRowHeight-int-double-) | Устанавливает высоту указанной строки. |
| [setRowHeightInch(int row, double inches)](#setRowHeightInch-int-double-) | Устанавливает высоту строки в дюймах. |
| [setRowHeightPixel(int row, int pixels)](#setRowHeightPixel-int-int-) | Устанавливает высоту строки в пикселях. |
| [setStandardHeight(double value)](#setStandardHeight-double-) | Устанавливает высоту строки по умолчанию в этом листе, в пунктах. |
| [setStandardHeightInch(double value)](#setStandardHeightInch-double-) | Устанавливает высоту строки по умолчанию в этом листе, в дюймах. |
| [setStandardHeightPixels(int value)](#setStandardHeightPixels-int-) | Устанавливает высоту строки по умолчанию в этом листе, в пикселях. |
| [setStandardWidth(double value)](#setStandardWidth-double-) | Устанавливает ширину столбца по умолчанию в листе, в символах. |
| [setStandardWidthInch(double value)](#setStandardWidthInch-double-) | Устанавливает ширину столбца по умолчанию в листе, в дюймах. |
| [setStandardWidthPixels(int value)](#setStandardWidthPixels-int-) | Устанавливает ширину столбца по умолчанию в листе, в пикселях. |
| [setStyle(Style value)](#setStyle-com.aspose.cells.Style-) | Устанавливает стиль листа по умолчанию. |
| [setViewColumnWidthPixel(int column, int pixels)](#setViewColumnWidthPixel-int-int-) | Устанавливает ширину столбца в разных представлениях. |
| [showGroupDetail(boolean isVertical, int index)](#showGroupDetail-boolean-int-) | Разворачивает сгруппированные строки/столбцы. |
| [subtotal(CellArea ca, int groupBy, int function, int[] totalList)](#subtotal-com.aspose.cells.CellArea-int-int-int---) | Создаёт промежуточные итоги для диапазона. |
| [subtotal(CellArea ca, int groupBy, int function, int[] totalList, boolean replace, boolean pageBreaks, boolean summaryBelowData)](#subtotal-com.aspose.cells.CellArea-int-int-int---boolean-boolean-boolean-) | Создаёт промежуточные итоги для диапазона. |
| [textToColumns(int row, int column, int totalRows, TxtLoadOptions options)](#textToColumns-int-int-int-com.aspose.cells.TxtLoadOptions-) | Разделяет содержимое указанного столбца на несколько столбцов.. |
| [toString()](#toString--) |  |
| [unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#unMerge-int-int-int-int-) | Разъединяет указанный диапазон объединённых ячеек. |
| [ungroupColumns(int firstIndex, int lastIndex)](#ungroupColumns-int-int-) | Разгруппирует столбцы. |
| [ungroupRows(int firstIndex, int lastIndex)](#ungroupRows-int-int-) | Разгруппирует строки. |
| [ungroupRows(int firstIndex, int lastIndex, boolean isAll)](#ungroupRows-int-int-boolean-) | Разгруппирует строки. |
| [unhideColumn(int column, double width)](#unhideColumn-int-double-) | Отображает скрытый столбец |
| [unhideColumns(int column, int totalColumns, double width)](#unhideColumns-int-int-double-) | Отображает несколько скрытых столбцов. |
| [unhideRow(int row, double height)](#unhideRow-int-double-) | Отображает скрытую строку. |
| [unhideRows(int row, int totalRows, double height)](#unhideRows-int-int-double-) | Отображает скрытые строки. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addRange(Range rangeObject) {#addRange-com.aspose.cells.Range-}
```
public void addRange(Range rangeObject)
```


Добавляет ссылку на объект диапазона в ячейки

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rangeObject | [Range](../../com.aspose.cells/range) | Объект диапазона будет содержаться в ячейках |

### applyColumnStyle(int column, Style style, StyleFlag flag) {#applyColumnStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyColumnStyle(int column, Style style, StyleFlag flag)
```


Применяет форматы ко всему столбцу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int | Индекс столбца. |
| style | [Style](../../com.aspose.cells/style) | Объект стиля, который будет применён. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Флаги, указывающие применённые свойства форматирования. |

### applyRowStyle(int row, Style style, StyleFlag flag) {#applyRowStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyRowStyle(int row, Style style, StyleFlag flag)
```


Применяет форматирование ко всей строке.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |
| style | [Style](../../com.aspose.cells/style) | Объект стиля, который будет применён. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Флаги, указывающие применённые свойства форматирования. |

### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Применяет форматы ко всему листу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Объект стиля, который будет применён. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Флаги, указывающие применённые свойства форматирования. |

### checkCell(int row, int column) {#checkCell-int-int-}
```
public Cell checkCell(int row, int column)
```


Получает элемент [Cell](../../com.aspose.cells/cell) или null по указанному индексу строки ячейки и индексу столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки |
| столбец | int | Индекс столбца |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Return Cell object if a Cell object exists. Return null if the cell does not exist.
### checkColumn(int columnIndex) {#checkColumn-int-}
```
public Column checkColumn(int columnIndex)
```


Получает элемент [Column](../../com.aspose.cells/column) или null по указанному индексу столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | int | Индекс столбца. |

**Returns:**
[Column](../../com.aspose.cells/column) - The Column object.
### checkRow(int row) {#checkRow-int-}
```
public Row checkRow(int row)
```


Получает элемент [Row](../../com.aspose.cells/row) или null по указанному индексу строки ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки |

**Returns:**
[Row](../../com.aspose.cells/row) - Returns [Row](../../com.aspose.cells/row) object If the row object does exist, otherwise returns null.
### clear() {#clear--}
```
public void clear()
```


Очищает все данные листа.

### clearContents(CellArea range) {#clearContents-com.aspose.cells.CellArea-}
```
public void clearContents(CellArea range)
```


Очищает содержимое диапазона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| range | [CellArea](../../com.aspose.cells/cellarea) | Диапазон для очистки. |

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

### clearFormats(CellArea range) {#clearFormats-com.aspose.cells.CellArea-}
```
public void clearFormats(CellArea range)
```


Очищает форматирование диапазона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| range | [CellArea](../../com.aspose.cells/cellarea) | Диапазон для очистки. |

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

### clearMergedCells() {#clearMergedCells--}
```
public void clearMergedCells()
```


Очищает все объединённые диапазоны.

### clearRange(CellArea range) {#clearRange-com.aspose.cells.CellArea-}
```
public void clearRange(CellArea range)
```


Очищает содержимое и форматирование диапазона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| range | [CellArea](../../com.aspose.cells/cellarea) | Диапазон для очистки. |

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

### convertStringToNumericValue() {#convertStringToNumericValue--}
```
public void convertStringToNumericValue()
```


Преобразует все строковые данные в листе в числовые значения, если это возможно.

### copyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex) {#copyColumn-com.aspose.cells.Cells-int-int-}
```
public void copyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex)
```


Копирует данные и форматы целого столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Объект Source Cells содержит данные и форматы для копирования. |
| sourceColumnIndex | int | Индекс исходного столбца. |
| destinationColumnIndex | int | Индекс целевого столбца. |

### copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber) {#copyColumns-com.aspose.cells.Cells-int-int-int-}
```
public void copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)
```


Копирует данные и форматы целых столбцов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Объект Source Cells содержит данные и форматы для копирования. |
| sourceColumnIndex | int | Индекс исходного столбца. |
| destinationColumnIndex | int | Индекс целевого столбца. |
| columnNumber | int | Номер скопированного столбца. |

### copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber, PasteOptions pasteOptions) {#copyColumns-com.aspose.cells.Cells-int-int-int-com.aspose.cells.PasteOptions-}
```
public void copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber, PasteOptions pasteOptions)
```


Копирует данные и форматы целого столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Объект Source Cells содержит данные и форматы для копирования. |
| sourceColumnIndex | int | Индекс исходного столбца. |
| destinationColumnIndex | int | Индекс целевого столбца. |
| columnNumber | int | Номер скопированного столбца. |
| pasteOptions | [PasteOptions](../../com.aspose.cells/pasteoptions) | опции вставки. |

### copyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, int destinationColumnIndex, int destinationTotalColumns) {#copyColumns-com.aspose.cells.Cells-int-int-int-int-}
```
public void copyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, int destinationColumnIndex, int destinationTotalColumns)
```


Копирует данные и форматы всех столбцов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Объект Source Cells содержит данные и форматы для копирования. |
| sourceColumnIndex | int | Индекс исходного столбца. |
| sourceTotalColumns | int | Количество исходных столбцов. |
| destinationColumnIndex | int | Индекс целевого столбца. |
| destinationTotalColumns | int | Количество целевых столбцов. |

### copyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex) {#copyRow-com.aspose.cells.Cells-int-int-}
```
public void copyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex)
```


Копирует данные и форматы целой строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Объект Source Cells содержит данные и форматы для копирования. |
| sourceRowIndex | int | Индекс исходной строки. |
| destinationRowIndex | int | Индекс целевой строки. |

### copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber) {#copyRows-com.aspose.cells.Cells-int-int-int-}
```
public void copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```


Копирует данные и форматы некоторых целых строк.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Объект Source Cells содержит данные и форматы для копирования. |
| sourceRowIndex | int | Индекс исходной строки. |
| destinationRowIndex | int | Индекс целевой строки. |
| rowNumber | int | Номер скопированной строки. |

### copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions) {#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-}
```
public void copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions)
```


Копирует данные и форматы некоторых целых строк.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Объект Source Cells содержит данные и форматы для копирования. |
| sourceRowIndex | int | Индекс исходной строки. |
| destinationRowIndex | int | Индекс целевой строки. |
| rowNumber | int | Номер скопированной строки. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Опции копирования. |

### copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions) {#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-com.aspose.cells.PasteOptions-}
```
public void copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)
```


Копирует данные и форматы некоторых целых строк.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceCells0 | [Cells](../../com.aspose.cells/cells) | Объект Source Cells содержит данные и форматы для копирования. |
| sourceRowIndex | int | Индекс исходной строки. |
| destinationRowIndex | int | Индекс целевой строки. |
| rowNumber | int | Номер скопированной строки. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Опции копирования. |
| pasteOptions | [PasteOptions](../../com.aspose.cells/pasteoptions) | опции вставки. |

### createRange(int firstIndex, int number, boolean isVertical) {#createRange-int-int-boolean-}
```
public Range createRange(int firstIndex, int number, boolean isVertical)
```


Создаёт объект [Range](../../com.aspose.cells/range) из строк ячеек или столбцов ячеек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| firstIndex | int | Первый индекс строки или первый индекс столбца, нулевой базис. |
| number | int | Общее количество строк или столбцов, единичный базис. |
| isVertical | boolean | True — диапазон создан из столбцов ячеек. False — диапазон создан из строк ячеек. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object.
### createRange(int firstRow, int firstColumn, int totalRows, int totalColumns) {#createRange-int-int-int-int-}
```
public Range createRange(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Создаёт объект [Range](../../com.aspose.cells/range) из диапазона ячеек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | int | Первая строка этого диапазона |
| firstColumn | int | Первый столбец этого диапазона |
| totalRows | int | Количество строк |
| totalColumns | int | Количество столбцов |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### createRange(String address) {#createRange-java.lang.String-}
```
public Range createRange(String address)
```


Создаёт объект [Range](../../com.aspose.cells/range) из адреса диапазона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| адрес | java.lang.String | Адрес диапазона. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### createRange(String upperLeftCell, String lowerRightCell) {#createRange-java.lang.String-java.lang.String-}
```
public Range createRange(String upperLeftCell, String lowerRightCell)
```


Создаёт объект [Range](../../com.aspose.cells/range) из диапазона ячеек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| upperLeftCell | java.lang.String | Имя ячейки в верхнем левом углу. |
| lowerRightCell | java.lang.String | Имя ячейки в нижнем правом углу. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### deleteBlankColumns() {#deleteBlankColumns--}
```
public void deleteBlankColumns()
```


Удалить все пустые столбцы, которые не содержат никаких данных.

### deleteBlankColumns(DeleteOptions options) {#deleteBlankColumns-com.aspose.cells.DeleteOptions-}
```
public void deleteBlankColumns(DeleteOptions options)
```


Удалить все пустые столбцы, которые не содержат никаких данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | Опции удаления диапазона. |

### deleteBlankRows() {#deleteBlankRows--}
```
public void deleteBlankRows()
```


Удалить все пустые строки, которые не содержат никаких данных или других объектов.

### deleteBlankRows(DeleteOptions options) {#deleteBlankRows-com.aspose.cells.DeleteOptions-}
```
public void deleteBlankRows(DeleteOptions options)
```


Удалить все пустые строки, которые не содержат никаких данных или некоторых специальных объектов, таких как видимый комментарий, сводная таблица.

**Remarks**

Для пустых строк, которые будут удалены, требуется не только, чтобы [Row.isBlank()](../../com.aspose.cells/row\#isBlank--) было истинным, но также не должно быть видимых комментариев, определённых для любой ячейки в этих строках, и не должно быть сводной таблицы, диапазон которой пересекается с ними.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | Опции удаления диапазона. |

### deleteColumn(int columnIndex) {#deleteColumn-int-}
```
public void deleteColumn(int columnIndex)
```


Удаляет столбец.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | int | Индекс столбца, который будет удалён. |

### deleteColumn(int columnIndex, boolean updateReference) {#deleteColumn-int-boolean-}
```
public void deleteColumn(int columnIndex, boolean updateReference)
```


Удаляет столбец.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | int | Индекс столбца, который будет удалён. |
| updateReference | boolean | Указывает, следует ли обновлять ссылки в других листах. |

### deleteColumns(int columnIndex, int totalColumns, boolean updateReference) {#deleteColumns-int-int-boolean-}
```
public void deleteColumns(int columnIndex, int totalColumns, boolean updateReference)
```


Удаляет несколько столбцов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | int | Индекс первого столбца, который будет удалён. |
| totalColumns | int | Количество столбцов, которые будут удалены. |
| updateReference | boolean | Указывает, следует ли обновлять ссылки в других листах. |

### deleteColumns(int columnIndex, int totalColumns, DeleteOptions options) {#deleteColumns-int-int-com.aspose.cells.DeleteOptions-}
```
public void deleteColumns(int columnIndex, int totalColumns, DeleteOptions options)
```


Удаляет несколько столбцов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | int | Индекс первого столбца, который будет удалён. |
| totalColumns | int | Количество столбцов, которые будут удалены. |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | Опции операции удаления |

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
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Опция смещения ячеек. |

### deleteRow(int rowIndex) {#deleteRow-int-}
```
public void deleteRow(int rowIndex)
```


Удаляет строку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | int | Индекс строки, которая будет удалена. |

### deleteRow(int rowIndex, boolean updateReference) {#deleteRow-int-boolean-}
```
public void deleteRow(int rowIndex, boolean updateReference)
```


Удаляет строку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | int | Индекс строки, которая будет удалена. |
| updateReference | boolean | Указывает, следует ли обновлять ссылки в других листах. |

### deleteRows(int rowIndex, int totalRows) {#deleteRows-int-int-}
```
public boolean deleteRows(int rowIndex, int totalRows)
```


Удаляет несколько строк.

**Remarks**

Если удаляемый диапазон содержит верхнюю часть (не полностью) таблицы (ListObject), диапазон не может быть удалён и ничего не будет сделано. Это работает так же, как в MS Excel.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | int | Индекс первой строки, которая будет удалена. |
| totalRows | int | Количество строк, которые будут удалены. |

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
| rowIndex | int | Индекс первой строки, которая будет удалена. |
| totalRows | int | Количество строк, которые будут удалены. |
| updateReference | boolean | Указывает, следует ли обновлять ссылки в других листах. |

**Returns:**
boolean -
### deleteRows(int rowIndex, int totalRows, DeleteOptions options) {#deleteRows-int-int-com.aspose.cells.DeleteOptions-}
```
public boolean deleteRows(int rowIndex, int totalRows, DeleteOptions options)
```


Удаляет несколько строк в листе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | int | Индекс первой строки, которая будет удалена. |
| totalRows | int | Количество строк, которые будут удалены. |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | Опции операции удаления |

**Returns:**
boolean -
### dispose() {#dispose--}
```
public void dispose()
```


Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов.

### endCellInColumn(int columnIndex) {#endCellInColumn-int-}
```
public Cell endCellInColumn(int columnIndex)
```


Получает последнюю ячейку в этом столбце.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | int | Индекс столбца. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### endCellInColumn(int startRow, int endRow, int startColumn, int endColumn) {#endCellInColumn-int-int-int-int-}
```
public Cell endCellInColumn(int startRow, int endRow, int startColumn, int endColumn)
```


Получает последнюю ячейку с максимальным индексом столбца в этом диапазоне.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | int | Индекс начальной строки. |
| endRow | int | Индекс конечной строки. |
| startColumn | int | Индекс начального столбца. |
| endColumn | int | Индекс конечного столбца. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### endCellInRow(int rowIndex) {#endCellInRow-int-}
```
public Cell endCellInRow(int rowIndex)
```


Получает последнюю ячейку в этой строке.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | int | Индекс строки. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### endCellInRow(int startRow, int endRow, int startColumn, int endColumn) {#endCellInRow-int-int-int-int-}
```
public Cell endCellInRow(int startRow, int endRow, int startColumn, int endColumn)
```


Получает последнюю ячейку с максимальным индексом строки в этом диапазоне.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | int | Индекс начальной строки. |
| endRow | int | Индекс конечной строки. |
| startColumn | int | Индекс начального столбца. |
| endColumn | int | Индекс конечного столбца. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
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


Экспортирует данные из коллекции [Cells](../../com.aspose.cells/cells) в двумерный массив.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | int | Номер строки первой ячейки для экспорта. |
| firstColumn | int | Номер столбца первой ячейки для экспорта. |
| totalRows | int | Количество строк для экспорта |
| totalColumns | int | Количество столбцов для экспорта |

**Returns:**
java.lang.Object[][] - Объект массива экспортированных значений ячеек.
### exportTypeArray(int firstRow, int firstColumn, int totalRows, int totalColumns) {#exportTypeArray-int-int-int-int-}
```
public int[][] exportTypeArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Экспортирует тип значения ячейки из коллекции [Cells](../../com.aspose.cells/cells) в двумерный массив.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | int | Номер строки первой ячейки для экспорта. |
| firstColumn | int | Номер столбца первой ячейки для экспорта. |
| totalRows | int | Количество строк для экспорта. |
| totalColumns | int | Количество столбцов для экспорта. |

**Returns:**
int[][] — [CellValueType](../../com.aspose.cells/cellvaluetype). Экспортированный массивный объект, представляющий типы значений ячеек.
### find(Object what, Cell previousCell) {#find-java.lang.Object-com.aspose.cells.Cell-}
```
public Cell find(Object what, Cell previousCell)
```


Находит ячейку, содержащую входной объект.

**Remarks**

Возвращает null (Nothing), если ячейка не найдена.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| что | java.lang.Object | Объект для поиска. Тип должен быть int, double, DateTime, string, bool. |
| previousCell | [Cell](../../com.aspose.cells/cell) | Предыдущая ячейка с тем же объектом. Этот параметр можно установить в null, если поиск начинается с начала. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### find(Object what, Cell previousCell, FindOptions findOptions) {#find-java.lang.Object-com.aspose.cells.Cell-com.aspose.cells.FindOptions-}
```
public Cell find(Object what, Cell previousCell, FindOptions findOptions)
```


Находит ячейку, содержащую входной объект.

**Remarks**

Возвращает null (Nothing), если ячейка не найдена.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| что | java.lang.Object | Объект для поиска. Тип должен быть int, double, DateTime, string, bool. |
| previousCell | [Cell](../../com.aspose.cells/cell) | Предыдущая ячейка с тем же объектом. Этот параметр можно установить в null, если поиск начинается с начала. |
| findOptions | [FindOptions](../../com.aspose.cells/findoptions) | Параметры поиска |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### get(int row, int column) {#get-int-int-}
```
public Cell get(int row, int column)
```


Получает элемент [Cell](../../com.aspose.cells/cell) по указанному индексу строки и индексу столбца ячейки.

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
         Cell cell = cells.get(0, 0);	//Gets the cell at "A1"
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |
| столбец | int | Индекс столбца. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - The [Cell](../../com.aspose.cells/cell) object.
### get(String cellName) {#get-java.lang.String-}
```
public Cell get(String cellName)
```


Получает элемент [Cell](../../com.aspose.cells/cell) по указанному имени ячейки.

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
         Cell cell = cells.get("A1");	//Gets the cell at "A1"
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cellName | java.lang.String | Имя ячейки, включающее букву столбца и номер строки, например A5. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - A [Cell](../../com.aspose.cells/cell) object
### getCellDisplayStyle(int row, int column) {#getCellDisplayStyle-int-int-}
```
public Style getCellDisplayStyle(int row, int column)
```


Получить стиль отображения заданной ячейки.

**Remarks**

То же самое, что и у [Cell.getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--), и то же при использовании [BorderType.SIDE\_BORDERS](../../com.aspose.cells/bordertype\#SIDE-BORDERS) для [getCellDisplayStyle(int,int,int)](../../com.aspose.cells/cells\#getCellDisplayStyle-int-int-int-).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | индекс строки заданной ячейки |
| столбец | int | столбец заданной ячейки |

**Returns:**
[Style](../../com.aspose.cells/style) - the display style of given cell.
### getCellDisplayStyle(int row, int column, int adjacentBorders) {#getCellDisplayStyle-int-int-int-}
```
public Style getCellDisplayStyle(int row, int column, int adjacentBorders)
```


Получить стиль отображения заданной ячейки.

**Remarks**

Если ячейка также затронута другими настройками, такими как условное форматирование, объекты списка и т.д., то стиль отображения может отличаться от [getCellStyle(int,int)](../../com.aspose.cells/cells\#getCellStyle-int-int-). И поскольку эти настройки могут применяться к пустым (несуществующим) ячейкам, использование этого метода позволяет избежать создания этих пустых ячеек, поэтому производительность будет лучше, чем получение экземпляра Cell из Cells и последующий вызов [Cell.getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | индекс строки заданной ячейки |
| столбец | int | столбец заданной ячейки |
| adjacentBorders | int | [BorderType](../../com.aspose.cells/bordertype). Указывает, какие границы необходимо проверять и корректировать в соответствии с границами соседних ячеек. Пожалуйста, см. описание того же параметра в [Cell.getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-). |

**Returns:**
[Style](../../com.aspose.cells/style) - the display style of given cell.
### getCellStyle(int row, int column) {#getCellStyle-int-int-}
```
public Style getCellStyle(int row, int column)
```


Получить стиль заданной ячейки.

**Remarks**

Возвращаемый стиль — это только тот, который установлен для ячейки или унаследован от строки/столбца ячейки, он не включает свойства, применённые другими настройками, такими как условное форматирование.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | индекс строки |
| столбец | int | столбец |

**Returns:**
[Style](../../com.aspose.cells/style) - the style of given cell.
### getCellsWithPlaceInCellPicture() {#getCellsWithPlaceInCellPicture--}
```
public Iterator getCellsWithPlaceInCellPicture()
```


Получает все ячейки, содержащие встроенное изображение.

**Remarks**

Если в этом листе нет изображения, установленного как "Place in Cell", будет возвращено null.

**Returns:**
java.util.Iterator — перечислитель для перебора всех объектов Cell, содержащих встроенное изображение
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnOriginalWidthPoint(int column) {#getColumnOriginalWidthPoint-int-}
```
public double getColumnOriginalWidthPoint(int column)
```


Получает исходную высоту столбца в пунктах, если столбец скрыт

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод Cells.GetColumnWidth(int, bool, CellsUnitType). Этот метод будет удалён через 12 месяцев, начиная с апреля 2024 года. Aspose просит прощения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int | Индекс строки. |

**Returns:**
double — ширина столбца в обычном виде.
### getColumnWidth(int column) {#getColumnWidth-int-}
```
public double getColumnWidth(int column)
```


Получает ширину (в единицах символов) указанного столбца в обычном виде

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int | Индекс столбца |

**Returns:**
double — ширина столбца. Для электронных таблиц ширина столбца измеряется количеством символов максимальной ширины цифр 0~9, отображаемых шрифтом обычного стиля.
### getColumnWidth(int column, boolean isOriginal, int unitType) {#getColumnWidth-int-boolean-int-}
```
public double getColumnWidth(int column, boolean isOriginal, int unitType)
```


Получает ширину столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int | Индекс столбца. |
| isOriginal | boolean | Указывает, следует ли получать оригинальную ширину. |
| unitType | int | [CellsUnitType](../../com.aspose.cells/cellsunittype). |

**Returns:**
double -
### getColumnWidthInch(int column) {#getColumnWidthInch-int-}
```
public double getColumnWidthInch(int column)
```


Получает ширину указанного столбца в обычном виде, в дюймах.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод Cells.GetColumnWidth(int, bool, CellsUnitType). Этот метод будет удалён через 12 месяцев, начиная с апреля 2024 года. Aspose просит прощения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int | Индекс столбца |

**Returns:**
double — ширина столбца в обычном виде.
### getColumnWidthPixel(int column) {#getColumnWidthPixel-int-}
```
public int getColumnWidthPixel(int column)
```


Получает ширину указанного столбца в обычном виде, в пикселях.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int | Индекс столбца |

**Returns:**
int — ширина столбца в обычном виде.
### getColumnWidthPixel(int column, boolean original) {#getColumnWidthPixel-int-boolean-}
```
public int getColumnWidthPixel(int column, boolean original)
```


Получает ширину указанного столбца в обычном виде, в пикселях.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод Cells.GetColumnWidth(int, bool, CellsUnitType). Этот метод будет удалён через 12 месяцев, начиная с апреля 2024 года. Aspose просит прощения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int | Индекс столбца |
| исходная | boolean | Указывает, следует ли возвращать исходную ширину, даже если столбец скрыт |

**Returns:**
int — ширина столбца в обычном виде.
### getColumns() {#getColumns--}
```
public ColumnCollection getColumns()
```


Получает коллекцию объектов [Column](../../com.aspose.cells/column), представляющих отдельные столбцы в этом листе.

**Returns:**
[ColumnCollection](../../com.aspose.cells/columncollection)
### getCount() {#getCount--}
```
public int getCount()
```


Получает общее количество созданных объектов Cell.

**Returns:**
int
### getCountLarge() {#getCountLarge--}
```
public long getCountLarge()
```


Получает общее количество созданных объектов Cell.

**Returns:**
long
### getDependents(boolean isAll, int row, int column) {#getDependents-boolean-int-int-}
```
public Cell[] getDependents(boolean isAll, int row, int column)
```


Получить все ячейки, которые ссылаются на конкретную ячейку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| isAll | boolean | Указывает, следует ли проверять другие листы |
| строка | int | Индекс строки. |
| столбец | int | Индекс столбца. |

**Returns:**
com.aspose.cells.Cell[] -
### getDependentsInCalculation(int row, int column, boolean recursive) {#getDependentsInCalculation-int-int-boolean-}
```
public Iterator getDependentsInCalculation(int row, int column, boolean recursive)
```


Получает все ячейки, расчётный результат которых зависит от конкретной ячейки.

**Remarks**

Чтобы использовать этот метод, убедитесь, что для рабочей книги установлено значение true для [FormulaSettings.getEnableCalculationChain()](../../com.aspose.cells/formulasettings\#getEnableCalculationChain--) и что она полностью вычислена с этим параметром. Если нет ссылки на формулу в этой ячейке, будет возвращено null. Для получения более подробной информации и примера, пожалуйста, см. [Cell.getDependentsInCalculation(boolean)](../../com.aspose.cells/cell\#getDependentsInCalculation-boolean-).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки конкретной ячейки |
| столбец | int | Индекс столбца конкретной ячейки. |
| recursive | boolean | Возвращает ли те зависимости, которые не ссылаются непосредственно на конкретную ячейку, а ссылаются на другие листовые элементы этой ячейки. |

**Returns:**
java.util.Iterator - перечислитель для перечисления всех зависимых (объекты Cell)
### getFirstCell() {#getFirstCell--}
```
public Cell getFirstCell()
```


Получает первую ячейку в этом листе.

**Remarks**

Возвращает null, если в листе нет данных.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getFirstDataRow(int column) {#getFirstDataRow-int-}
```
public int getFirstDataRow(int column)
```


Получает индекс первой строки ячейки, содержащей данные в указанном столбце.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int | Индекс столбца. |

**Returns:**
int — индекс первой строки.
### getGroupedColumnOutlineLevel(int columnIndex) {#getGroupedColumnOutlineLevel-int-}
```
public int getGroupedColumnOutlineLevel(int columnIndex)
```


Получает уровень структуры (нумерация с нуля) столбца.

**Remarks**

Если столбец не сгруппирован, возвращает ноль.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | int | Индекс столбца |

**Returns:**
int — уровень структуры столбца
### getGroupedRowOutlineLevel(int rowIndex) {#getGroupedRowOutlineLevel-int-}
```
public int getGroupedRowOutlineLevel(int rowIndex)
```


Получает уровень структуры (нумерация с нуля) строки.

**Remarks**

Если строка не сгруппирована, возвращает ноль.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | int | Индекс строки. |

**Returns:**
int — уровень структуры (нумерация с нуля) строки.
### getLastCell() {#getLastCell--}
```
public Cell getLastCell()
```


Получает последнюю ячейку в этом листе.

**Remarks**

Возвращает null, если в листе нет данных.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getLastDataRow(int column) {#getLastDataRow-int-}
```
public int getLastDataRow(int column)
```


Получает индекс последней строки ячейки, содержащей данные в указанном столбце.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int | Индекс столбца. |

**Returns:**
int — индекс последней строки.
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


Максимальный индекс столбца среди ячеек, созданных в коллекции (не включает столбец, для которого определён стиль целого столбца, но в нём не создано ни одной ячейки).

**Remarks**

Возвращает -1, если ни одна ячейка не была создана.

**Returns:**
int
### getMaxDataColumn() {#getMaxDataColumn--}
```
public int getMaxDataColumn()
```


Максимальный индекс столбца ячейки, содержащей данные.

**Remarks**

\-1 будет возвращено, если нет ячейки, содержащей данные. Это свойство должно перебрать и проверить все ячейки листа динамически, поэтому это затратный по времени процесс и не должно вызываться многократно, например, использовать его напрямую в условии цикла.

**Returns:**
int
### getMaxDataRow() {#getMaxDataRow--}
```
public int getMaxDataRow()
```


Максимальный индекс строки ячейки, содержащей данные.

**Remarks**

Возвращает -1, если нет ячейки, содержащей данные. Это свойство должно перебрать и проверить ячейки и строки динамически, поэтому это затратный по времени процесс и не должно вызываться многократно, например, использовать его напрямую в условии цикла.

**Returns:**
int
### getMaxDisplayRange() {#getMaxDisplayRange--}
```
public Range getMaxDisplayRange()
```


Получает максимальный диапазон, включающий данные, объединённые ячейки и фигуры.

**Remarks**

Возвращает null, если лист пуст, начиная с Aspose.Cells 21.5.2.

**Returns:**
[Range](../../com.aspose.cells/range)
### getMaxGroupedColumnOutlineLevel() {#getMaxGroupedColumnOutlineLevel--}
```
public int getMaxGroupedColumnOutlineLevel()
```


Получает максимальный уровень структуры сгруппированных столбцов (нумерация с нуля).

**Returns:**
int — максимальный уровень структуры сгруппированных столбцов (нумерация с нуля)
### getMaxGroupedRowOutlineLevel() {#getMaxGroupedRowOutlineLevel--}
```
public int getMaxGroupedRowOutlineLevel()
```


Получает максимальный уровень структуры сгруппированных строк (нумерация с нуля).

**Returns:**
int — максимальный уровень структуры сгруппированных строк (нумерация с нуля)
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


Максимальный индекс строки ячейки, содержащей данные или стиль.

**Remarks**

Возвращает -1, если в листе нет ячейки, содержащей данные или стиль. Это свойство должно перебрать и проверить ячейки и строки динамически, поэтому это затратный по времени процесс и не должно вызываться многократно, например, использовать его напрямую в условии цикла.

**Returns:**
int
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


Получает параметр использования памяти для этих ячеек.

Смотрите [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Заметные ограничения и рекомендуемые операции для некоторых режимов:

| Режим | Примечания | Поддерживается |
| ------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
| [MemorySetting.MEMORY\_PREFERENCE](../../com.aspose.cells/memorysetting\#MEMORY-PREFERENCE) | Cells data will be maintained in compact format to decrease the memory cost. On other hand, the compact data also may cause higher time cost, especially when updating the cells data, or accessing cells/rows randomly | v8.0.0 |
|  | [MemorySetting.FILE\_CACHE](../../com.aspose.cells/memorysetting\#FILE-CACHE) | Когда этот режим используется для любого листа в рабочей книге, следует вызвать [Workbook.dispose()](../../com.aspose.cells/workbook\#dispose--) в конце работы, чтобы освободить все ресурсы, такие как временные файлы. |
 
Случайный доступ к ячейкам приводит к плохой производительности, потому что данные необходимо читать/обновлять случайным и повторяющимся образом (из‑за чего указатель в файле будет изменяться соответственно и операции ввода‑вывода будут требоваться многократно). По возможности, всегда обращайтесь к данным последовательно (строка за строкой).
 
Когда данные одной строки/ячейки изменяются, данные других ячеек/строк также могут быть затронуты (например, данные могут быть смещены/перемещены в другие места для выделения достаточного пространства под изменённые данные). Поэтому каждое изменение любых данных требует синхронизации других существующих объектов (например, объектов Row или Cell). Чтобы получить лучшую производительность, пожалуйста, не поддерживайте одновременно несколько Row/Cell. Обработка их по одной уменьшит синхронизацию данных и немного повысит производительность. | v25.7     |

**Returns:**
int
### getMergedAreas() {#getMergedAreas--}
```
public CellArea[] getMergedAreas()
```


Получает все объединённые ячейки.

**Returns:**
com.aspose.cells.CellArea[]
### getMergedCells() {#getMergedCells--}
```
public ArrayList getMergedCells()
```


Получает коллекцию объединённых ячеек.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод Cells.GetMergedAreas(). Этот метод будет удалён через 12 месяцев, начиная с ноября 2023 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

**Returns:**
java.util.ArrayList
### getMinColumn() {#getMinColumn--}
```
public int getMinColumn()
```


Минимальный индекс столбца тех ячеек, которые были созданы в коллекции (не включает столбец, в котором стиль определён для всего столбца, но ни одна ячейка не была создана в нём).

**Remarks**

Это свойство требует итерации и динамической проверки ячеек и строк, поэтому это затратный по времени процесс и не должно вызываться многократно, например использовать его напрямую в качестве условия в цикле.

**Returns:**
int
### getMinDataColumn() {#getMinDataColumn--}
```
public int getMinDataColumn()
```


Минимальный индекс столбца ячейки, содержащей данные.

**Remarks**

\-1 будет возвращено, если нет ячейки, содержащей данные. Это свойство должно перебрать и проверить все ячейки листа динамически, поэтому это затратный по времени процесс и не должно вызываться многократно, например, использовать его напрямую в условии цикла.

**Returns:**
int
### getMinDataRow() {#getMinDataRow--}
```
public int getMinDataRow()
```


Минимальный индекс строки ячейки, содержащей данные.

**Remarks**

Возвращает -1, если нет ячейки, содержащей данные. Это свойство должно перебрать и проверить ячейки и строки динамически, поэтому это затратный по времени процесс и не должно вызываться многократно, например, использовать его напрямую в условии цикла.

**Returns:**
int
### getMinRow() {#getMinRow--}
```
public int getMinRow()
```


Минимальный индекс строки ячейки, содержащей данные или стиль.

**Remarks**

Это свойство требует итерации и динамической проверки ячеек и строк, поэтому это затратный по времени процесс и не должно вызываться многократно, например использовать его напрямую в качестве условия в цикле.

**Returns:**
int
### getMultiThreadReading() {#getMultiThreadReading--}
```
public boolean getMultiThreadReading()
```


Возвращает, должна ли модель данных ячеек поддерживать многопоточное чтение. Значение по умолчанию этого свойства — false.

**Remarks**

Если в этой коллекции одновременно читаются объекты Row/Cell несколькими потоками, это свойство следует установить в true, иначе могут возникнуть неожиданные результаты. Поддержка многопоточного чтения может ухудшить производительность доступа к объектам Row/Cell из этой коллекции. Обратите внимание, что некоторые функции не поддерживают многопоточное чтение, например форматирование значений (через [Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--), [Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), и т.д.). Поэтому даже при установленном значении true эти API могут давать неожиданные результаты при многопоточном чтении.

**Returns:**
boolean
### getOdsCellFields() {#getOdsCellFields--}
```
public OdsCellFieldCollection getOdsCellFields()
```


Получает список полей ods.

**Returns:**
[OdsCellFieldCollection](../../com.aspose.cells/odscellfieldcollection)
### getPreserveString() {#getPreserveString--}
```
public boolean getPreserveString()
```


Возвращает значение, указывающее, сохраняются ли все значения листов как строки. По умолчанию — false.

**Returns:**
boolean
### getRanges() {#getRanges--}
```
public RangeCollection getRanges()
```


Получает коллекцию объектов [Range](../../com.aspose.cells/range), созданных во время выполнения.

**Returns:**
[RangeCollection](../../com.aspose.cells/rangecollection)
### getRowEnumerator() {#getRowEnumerator--}
```
public Iterator getRowEnumerator()
```


Получает перечислитель строк.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод RowCollection.GetEnumerator(). Этот метод будет удалён через 12 месяцев, начиная с мая 2023 года. Aspose приносит извинения за любые причинённые неудобства.

**Returns:**
java.util.Iterator — перечислитель строк.
### getRowHeight(int row) {#getRowHeight-int-}
```
public double getRowHeight(int row)
```


Получает высоту указанной строки в единицах пунктов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки |

**Returns:**
double — высота строки
### getRowHeight(int row, boolean isOriginal, int unitType) {#getRowHeight-int-boolean-int-}
```
public double getRowHeight(int row, boolean isOriginal, int unitType)
```


Получает высоту строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |
| isOriginal | boolean | Возвращает оригинальную высоту строки или 0 для скрытой строки. |
| unitType | int | [CellsUnitType](../../com.aspose.cells/cellsunittype). Тип единицы возвращаемого значения высоты |

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
### getRowOriginalHeightPoint(int row) {#getRowOriginalHeightPoint-int-}
```
public double getRowOriginalHeightPoint(int row)
```


Получает оригинальную высоту строки в единицах пунктов, если строка скрыта.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод Cells.GetRowHeight(int,bool,CellsUnitType). Этот метод будет удалён через 12 месяцев, начиная с апреля 2024 года. Aspose приносит извинения за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |

**Returns:**
double -
### getRows() {#getRows--}
```
public RowCollection getRows()
```


Получает коллекцию объектов [Row](../../com.aspose.cells/row), представляющих отдельные строки в этом листе.

**Returns:**
[RowCollection](../../com.aspose.cells/rowcollection)
### getStandardHeight() {#getStandardHeight--}
```
public double getStandardHeight()
```


Получает высоту строки по умолчанию в этом листе в единицах пунктов.

**Returns:**
double
### getStandardHeightInch() {#getStandardHeightInch--}
```
public double getStandardHeightInch()
```


Получает высоту строки по умолчанию в этом листе в единицах дюймов.

**Returns:**
double
### getStandardHeightPixels() {#getStandardHeightPixels--}
```
public int getStandardHeightPixels()
```


Получает высоту строки по умолчанию в этом листе в единицах пикселей.

**Returns:**
int
### getStandardWidth() {#getStandardWidth--}
```
public double getStandardWidth()
```


Получает ширину столбца по умолчанию в листе в единицах символов.

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
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Получает стиль по умолчанию листа.

**Returns:**
[Style](../../com.aspose.cells/style)
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
### getViewRowHeight(int row) {#getViewRowHeight-int-}
```
public double getViewRowHeight(int row)
```


Получает высоту указанной строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |

**Returns:**
double — высота строки.
### getViewRowHeightInch(int row) {#getViewRowHeightInch-int-}
```
public double getViewRowHeightInch(int row)
```


Получает высоту указанной строки в единицах дюймов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки |

**Returns:**
double — высота строки
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

### groupRows(int firstIndex, int lastIndex, boolean isHidden) {#groupRows-int-int-boolean-}
```
public void groupRows(int firstIndex, int lastIndex, boolean isHidden)
```


Группирует строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| firstIndex | int | Первый индекс строки для группировки. |
| lastIndex | int | Последний индекс строки для группировки. |
| isHidden | boolean | Указывает, скрыты ли сгруппированные строки. |

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

### hideColumns(int column, int totalColumns) {#hideColumns-int-int-}
```
public void hideColumns(int column, int totalColumns)
```


Скрывает несколько столбцов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int | Индекс столбца. |
| totalColumns | int | Номер столбца. |

### hideGroupDetail(boolean isVertical, int index) {#hideGroupDetail-boolean-int-}
```
public void hideGroupDetail(boolean isVertical, int index)
```


Сворачивает сгруппированные строки/столбцы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| isVertical | boolean | True, свернуть сгруппированные строки. |
| индекс | int | Индекс строки/столбца |

### hideRow(int row) {#hideRow-int-}
```
public void hideRow(int row)
```


Скрывает строку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |

### hideRows(int row, int totalRows) {#hideRows-int-int-}
```
public void hideRows(int row, int totalRows)
```


Скрывает несколько строк.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |
| totalRows | int | Номер строки. |

### importArray(double[] doubleArray, int firstRow, int firstColumn, boolean isVertical) {#importArray-double---int-int-boolean-}
```
public void importArray(double[] doubleArray, int firstRow, int firstColumn, boolean isVertical)
```


Импортирует массив double в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| doubleArray | double[] | Массив double. |
| firstRow | int | Номер строки первой ячейки для импорта. |
| firstColumn | int | Номер столбца первой ячейки для импорта. |
| isVertical | boolean | Указывает импортировать данные вертикально или горизонтально. |

### importArray(double[][] doubleArray, int firstRow, int firstColumn) {#importArray-double-----int-int-}
```
public void importArray(double[][] doubleArray, int firstRow, int firstColumn)
```


Импортирует двумерный массив double в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| doubleArray | double[][] | Двумерный массив double. |
| firstRow | int | Номер строки первой ячейки для импорта. |
| firstColumn | int | Номер столбца первой ячейки для импорта. |

### importArray(int[] intArray, int firstRow, int firstColumn, boolean isVertical) {#importArray-int---int-int-boolean-}
```
public void importArray(int[] intArray, int firstRow, int firstColumn, boolean isVertical)
```


Импортирует массив integer в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| intArray | int[] | Массив целых чисел. |
| firstRow | int | Номер строки первой ячейки для импорта. |
| firstColumn | int | Номер столбца первой ячейки для импорта. |
| isVertical | boolean | Указывает импортировать данные вертикально или горизонтально. |

### importArray(int[][] intArray, int firstRow, int firstColumn) {#importArray-int-----int-int-}
```
public void importArray(int[][] intArray, int firstRow, int firstColumn)
```


Импортирует двумерный массив integer в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| intArray | int[][] | Двумерный массив целых чисел. |
| firstRow | int | Номер строки первой ячейки для импорта. |
| firstColumn | int | Номер столбца первой ячейки для импорта. |

### importArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical) {#importArray-java.lang.String---int-int-boolean-}
```
public void importArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)
```


Импортирует массив string в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stringArray | java.lang.String[] | Массив строк. |
| firstRow | int | Номер строки первой ячейки для импорта. |
| firstColumn | int | Номер столбца первой ячейки для импорта. |
| isVertical | boolean | Указывает импортировать данные вертикально или горизонтально. |

### importArray(String[][] stringArray, int firstRow, int firstColumn) {#importArray-java.lang.String-----int-int-}
```
public void importArray(String[][] stringArray, int firstRow, int firstColumn)
```


Импортирует двумерный массив string в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stringArray | java.lang.String[][] | Двумерный массив строк. |
| firstRow | int | Номер строки первой ячейки для импорта. |
| firstColumn | int | Номер столбца первой ячейки для импорта. |

### importArrayList(ArrayList arrayList, int firstRow, int firstColumn, boolean isVertical) {#importArrayList-java.util.ArrayList-int-int-boolean-}
```
public void importArrayList(ArrayList arrayList, int firstRow, int firstColumn, boolean isVertical)
```


Импортирует ArrayList данных в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arrayList | java.util.ArrayList | Данные arraylist. |
| firstRow | int | Номер строки первой ячейки для импорта. |
| firstColumn | int | Номер столбца первой ячейки для импорта. |
| isVertical | boolean | Указывает импортировать данные вертикально или горизонтально. |

### importCSV(InputStream stream, TxtLoadOptions options, int firstRow, int firstColumn) {#importCSV-java.io.InputStream-com.aspose.cells.TxtLoadOptions-int-int-}
```
public void importCSV(InputStream stream, TxtLoadOptions options, int firstRow, int firstColumn)
```


Импортирует CSV‑файл в ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.InputStream | Поток CSV‑файла. |
| options | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | Параметры загрузки для чтения текстового файла |
| firstRow | int | Номер строки первой ячейки для импорта. |
| firstColumn | int | Номер столбца первой ячейки для импорта. |

### importCSV(InputStream stream, String splitter, boolean convertNumericData, int firstRow, int firstColumn) {#importCSV-java.io.InputStream-java.lang.String-boolean-int-int-}
```
public void importCSV(InputStream stream, String splitter, boolean convertNumericData, int firstRow, int firstColumn)
```


Импортирует CSV‑файл в ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.InputStream | Поток CSV‑файла. |
| splitter | java.lang.String | Разделитель |
| convertNumericData | boolean | Определяет, преобразуется ли строка в текстовом файле в числовые данные. |
| firstRow | int | Номер строки первой ячейки для импорта. |
| firstColumn | int | Номер столбца первой ячейки для импорта. |

### importCSV(String fileName, TxtLoadOptions options, int firstRow, int firstColumn) {#importCSV-java.lang.String-com.aspose.cells.TxtLoadOptions-int-int-}
```
public void importCSV(String fileName, TxtLoadOptions options, int firstRow, int firstColumn)
```


Импортирует CSV‑файл в ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | Имя CSV‑файла. |
| options | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | Параметры загрузки для чтения текстового файла |
| firstRow | int | Номер строки первой ячейки для импорта. |
| firstColumn | int | Номер столбца первой ячейки для импорта. |

### importCSV(String fileName, String splitter, boolean convertNumericData, int firstRow, int firstColumn) {#importCSV-java.lang.String-java.lang.String-boolean-int-int-}
```
public void importCSV(String fileName, String splitter, boolean convertNumericData, int firstRow, int firstColumn)
```


Импортирует CSV‑файл в ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | Имя CSV‑файла. |
| splitter | java.lang.String | Разделитель |
| convertNumericData | boolean | Определяет, преобразуется ли строка в текстовом файле в числовые данные. |
| firstRow | int | Номер строки первой ячейки для импорта. |
| firstColumn | int | Номер столбца первой ячейки для импорта. |

### importCustomObjects(Collection list, int firstRow, int firstColumn, ImportTableOptions options) {#importCustomObjects-java.util.Collection-int-int-com.aspose.cells.ImportTableOptions-}
```
public int importCustomObjects(Collection list, int firstRow, int firstColumn, ImportTableOptions options)
```


Импортирует пользовательские объекты.

**Remarks**

Пользовательские объекты должны быть одного типа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| список | java.util.Collection | Пользовательский объект |
| firstRow | int | Номер строки первой ячейки для импорта. |
| firstColumn | int | Номер столбца первой ячейки для импорта. |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | Параметры импорта. |

**Returns:**
int — Общее количество импортированных строк.
### importCustomObjects(Collection list, String[] propertyNames, boolean isPropertyNameShown, int firstRow, int firstColumn, int rowNumber, boolean insertRows, String dateFormatString, boolean convertStringToNumber) {#importCustomObjects-java.util.Collection-java.lang.String---boolean-int-int-int-boolean-java.lang.String-boolean-}
```
public int importCustomObjects(Collection list, String[] propertyNames, boolean isPropertyNameShown, int firstRow, int firstColumn, int rowNumber, boolean insertRows, String dateFormatString, boolean convertStringToNumber)
```


Импортирует пользовательские объекты.

**Remarks**

Пользовательские объекты должны быть одного типа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| список | java.util.Collection | Пользовательский объект |
| propertyNames | java.lang.String[] | Имена свойств. Если значение null, будут импортированы все свойства объекта. |
| isPropertyNameShown | boolean | Указывает, будет ли имя свойства импортировано в первую строку. |
| firstRow | int | Номер строки первой ячейки для импорта. |
| firstColumn | int | Номер столбца первой ячейки для импорта. |
| rowNumber | int | Количество строк для импорта. |
| insertRows | boolean | Указывает, добавляются ли дополнительные строки для размещения данных. |
| dateFormatString | java.lang.String | Строка формата даты для ячеек. |
| convertStringToNumber | boolean | Указывает, будет ли этот метод пытаться преобразовать строку в число. |

**Returns:**
int — Общее количество импортированных строк.
### importData(ICellsDataTable table, int firstRow, int firstColumn, ImportTableOptions options) {#importData-com.aspose.cells.ICellsDataTable-int-int-com.aspose.cells.ImportTableOptions-}
```
public int importData(ICellsDataTable table, int firstRow, int firstColumn, ImportTableOptions options)
```


Импортирует данные из пользовательской таблицы данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| table | [ICellsDataTable](../../com.aspose.cells/icellsdatatable) | Пользовательская таблица данных. |
| firstRow | int | Индекс первой строки. |
| firstColumn | int | Индекс первого столбца. |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | Параметры импорта |

**Returns:**
int -
### importFormulaArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical) {#importFormulaArray-java.lang.String---int-int-boolean-}
```
public void importFormulaArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)
```


Импортирует массив формул в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stringArray | java.lang.String[] | Массив формул. |
| firstRow | int | Номер строки первой ячейки для импорта. |
| firstColumn | int | Номер столбца первой ячейки для импорта. |
| isVertical | boolean | Указывает импортировать данные вертикально или горизонтально. |

### importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical) {#importObjectArray-java.lang.Object---int-int-boolean-}
```
public void importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical)
```


Импортирует массив данных в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| objArray | java.lang.Object[] | Массив данных. |
| firstRow | int | Номер строки первой ячейки для импорта. |
| firstColumn | int | Номер столбца первой ячейки для импорта. |
| isVertical | boolean | Указывает импортировать данные вертикально или горизонтально. |

### importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical, int skip) {#importObjectArray-java.lang.Object---int-int-boolean-int-}
```
public void importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical, int skip)
```


Импортирует массив данных в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| objArray | java.lang.Object[] | Массив данных. |
| firstRow | int | Номер строки первой ячейки для импорта. |
| firstColumn | int | Номер столбца первой ячейки для импорта. |
| isVertical | boolean | Указывает импортировать данные вертикально или горизонтально. |
| пропустить | int | Пропущено количество строк или столбцов. |

### importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-int-int-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown)
```


Импортирует данные из объекта ResultSet в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rs | java.sql.ResultSet | объект ResultSet, из которого импортировать. |
| rowIndex | int | индекс начальной строки в листе. |
| columnIndex | int | индекс начального столбца в листе. |
| isFieldNameShown | boolean | Указывает, будет ли имя поля resultset импортировано в первую строку. |

**Returns:**
int — сколько строк фактически импортировано.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber) {#importResultSet-java.sql.ResultSet-int-int-boolean-java.lang.String-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)
```


Импортирует данные из объекта ResultSet в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rs | java.sql.ResultSet | объект ResultSet, из которого импортировать. |
| rowIndex | int | индекс начальной строки в листе. |
| columnIndex | int | индекс начального столбца в листе. |
| isFieldNameShown | boolean | Указывает, будет ли имя поля resultset импортировано в первую строку. |
| customDateFormatString | java.lang.String | Строка формата даты для ячеек, содержащих значение даты. |
| convertStringToNumber | boolean | Указывает, будет ли этот метод пытаться преобразовать строку в число. |

**Returns:**
int — сколько строк фактически импортировано.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, ImportTableOptions options) {#importResultSet-java.sql.ResultSet-int-int-com.aspose.cells.ImportTableOptions-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, ImportTableOptions options)
```


Импортирует данные из объекта ResultSet в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rs | java.sql.ResultSet | объект ResultSet, из которого импортировать. |
| rowIndex | int | индекс начальной строки в листе. |
| columnIndex | int | индекс начального столбца в листе. |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | Параметры импорта |

**Returns:**
int — сколько строк фактически импортировано.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown)
```


Импортирует данные из объекта ResultSet в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rs | java.sql.ResultSet | объект ResultSet, из которого импортировать. |
| rowIndex | int | индекс начальной строки в листе. |
| columnIndex | int | индекс начального столбца в листе. |
| rowNum | int | количество строк для импорта. -1 — импортировать все записи в заданном resultset. |
| columnNum | int | количество столбцов для импорта. -1 — импортировать все столбцы в заданном resultset. |
| isFieldNameShown | boolean | Указывает, будет ли имя поля resultset импортировано в первую строку. |

**Returns:**
int — сколько строк фактически импортировано.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber) {#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-java.lang.String-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)
```


Импортирует данные из объекта ResultSet в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rs | java.sql.ResultSet | объект ResultSet, из которого импортировать. |
| rowIndex | int | индекс начальной строки в листе. |
| columnIndex | int | индекс начального столбца в листе. |
| rowNum | int | количество строк для импорта. -1 — импортировать все записи в заданном resultset. |
| columnNum | int | количество столбцов для импорта. -1 — импортировать все столбцы в заданном resultset. |
| isFieldNameShown | boolean | Указывает, будет ли имя поля resultset импортировано в первую строку. |
| customDateFormatString | java.lang.String | Строка формата даты для ячеек, содержащих значение даты. |
| convertStringToNumber | boolean | Указывает, будет ли этот метод пытаться преобразовать строку в число. |

**Returns:**
int — сколько строк фактически импортировано.
### importResultSet(ResultSet rs, String startCell, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-java.lang.String-boolean-}
```
public int importResultSet(ResultSet rs, String startCell, boolean isFieldNameShown)
```


Импортирует данные из объекта ResultSet в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rs | java.sql.ResultSet | объект ResultSet, из которого импортировать. |
| startCell | java.lang.String | имя начальной ячейки для вставки resultset, например "A1". |
| isFieldNameShown | boolean | Указывает, будет ли имя поля resultset импортировано в первую строку. |

**Returns:**
int — сколько строк фактически импортировано.
### importResultSet(ResultSet rs, String startCell, ImportTableOptions options) {#importResultSet-java.sql.ResultSet-java.lang.String-com.aspose.cells.ImportTableOptions-}
```
public int importResultSet(ResultSet rs, String startCell, ImportTableOptions options)
```


Импортирует данные из объекта ResultSet в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rs | java.sql.ResultSet | объект ResultSet, из которого импортировать. |
| startCell | java.lang.String | имя начальной ячейки для вставки resultset, например "A1". |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | Параметры импорта |

**Returns:**
int — сколько строк фактически импортировано.
### importResultSet(ResultSet rs, String startCell, int rowNum, int columnNum, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-java.lang.String-int-int-boolean-}
```
public int importResultSet(ResultSet rs, String startCell, int rowNum, int columnNum, boolean isFieldNameShown)
```


Импортирует данные из объекта ResultSet в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rs | java.sql.ResultSet | объект ResultSet, из которого импортировать. |
| startCell | java.lang.String | имя начальной ячейки для вставки resultset, например "A1". |
| rowNum | int | количество строк для импорта. -1 — импортировать все записи в заданном resultset. |
| columnNum | int | количество столбцов для импорта. -1 — импортировать все столбцы в заданном resultset. |
| isFieldNameShown | boolean | Указывает, будет ли имя поля resultset импортировано в первую строку. |

**Returns:**
int — сколько строк фактически импортировано.
### importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn) {#importTwoDimensionArray-java.lang.Object-----int-int-}
```
public void importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn)
```


Импортирует двумерный массив данных в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| objArray | java.lang.Object[][] | Двумерный массив данных. |
| firstRow | int | Номер строки первой ячейки для импорта. |
| firstColumn | int | Номер столбца первой ячейки для импорта. |

### importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn, boolean convertStringToNumber) {#importTwoDimensionArray-java.lang.Object-----int-int-boolean-}
```
public void importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn, boolean convertStringToNumber)
```


Импортирует двумерный массив данных в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| objArray | java.lang.Object[][] | Двумерный массив данных. |
| firstRow | int | Номер строки первой ячейки для импорта. |
| firstColumn | int | Номер столбца первой ячейки для импорта. |
| convertStringToNumber | boolean | Указывает, будет ли этот метод пытаться преобразовать строку в число. |

### importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, boolean convertStringToNumber) {#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-boolean-}
```
public void importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, boolean convertStringToNumber)
```


Импортирует двумерный массив данных в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| objArray | java.lang.Object[][] | Двумерный массив данных. |
| стили | java.lang.Object[][] | Стиль двумерных данных. |
| firstRow | int | Номер строки первой ячейки для импорта. |
| firstColumn | int | Номер столбца первой ячейки для импорта. |
| convertStringToNumber | boolean | Указывает, будет ли этот метод пытаться преобразовать строку в число. |

### importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, TxtLoadOptions opts) {#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-com.aspose.cells.TxtLoadOptions-}
```
public void importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, TxtLoadOptions opts)
```


Импортирует двумерный массив данных в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| objArray | java.lang.Object[][] | Двумерный массив данных. |
| стили | java.lang.Object[][] | Стиль двумерных данных. |
| firstRow | int | Номер строки первой ячейки для импорта. |
| firstColumn | int | Номер столбца первой ячейки для импорта. |
| opts | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | Параметры преобразования строковых значений |

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

### insertColumns(int columnIndex, int totalColumns, InsertOptions options) {#insertColumns-int-int-com.aspose.cells.InsertOptions-}
```
public void insertColumns(int columnIndex, int totalColumns, InsertOptions options)
```


Вставляет несколько столбцов в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | int | Индекс столбца. |
| totalColumns | int | Количество столбцов. |
| options | [InsertOptions](../../com.aspose.cells/insertoptions) | Параметры операции вставки. |

### insertCutCells(Range cutRange, int row, int column, int shiftType) {#insertCutCells-com.aspose.cells.Range-int-int-int-}
```
public void insertCutCells(Range cutRange, int row, int column, int shiftType)
```


Вставить вырезанный диапазон.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cutRange | [Range](../../com.aspose.cells/range) | Диапазон вырезки. |
| строка | int | Строка. |
| столбец | int | Столбец. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Указывает, как сдвигать другие объекты целевого диапазона при вставке вырезанного диапазона. |

### insertRange(CellArea area, int shiftType) {#insertRange-com.aspose.cells.CellArea-int-}
```
public void insertRange(CellArea area, int shiftType)
```


Вставляет диапазон ячеек и сдвигает ячейки в соответствии с параметром сдвига.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| area | [CellArea](../../com.aspose.cells/cellarea) | Сдвинуть область. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Опция смещения ячеек. |

### insertRange(CellArea area, int shiftNumber, int shiftType) {#insertRange-com.aspose.cells.CellArea-int-int-}
```
public void insertRange(CellArea area, int shiftNumber, int shiftType)
```


Вставляет диапазон ячеек и сдвигает ячейки в соответствии с параметром сдвига.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| area | [CellArea](../../com.aspose.cells/cellarea) | Сдвинуть область. |
| shiftNumber | int | Количество строк или столбцов, которые будут вставлены. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Опция смещения ячеек. |

### insertRange(CellArea area, int shiftNumber, int shiftType, boolean updateReference) {#insertRange-com.aspose.cells.CellArea-int-int-boolean-}
```
public void insertRange(CellArea area, int shiftNumber, int shiftType, boolean updateReference)
```


Вставляет диапазон ячеек и сдвигает ячейки в соответствии с параметром сдвига.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| area | [CellArea](../../com.aspose.cells/cellarea) | Сдвинуть область. |
| shiftNumber | int | Количество строк или столбцов, которые будут вставлены. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Опция смещения ячеек. |
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

### insertRows(int rowIndex, int totalRows, InsertOptions options) {#insertRows-int-int-com.aspose.cells.InsertOptions-}
```
public void insertRows(int rowIndex, int totalRows, InsertOptions options)
```


Вставляет несколько строк в лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | int | Индекс строки. |
| totalRows | int | Количество строк, которые будут вставлены. |
| options | [InsertOptions](../../com.aspose.cells/insertoptions) | Параметры операции вставки. |

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
### isDefaultColumnHidden() {#isDefaultColumnHidden--}
```
public boolean isDefaultColumnHidden()
```




**Returns:**
boolean
### isDefaultRowHeightMatched() {#isDefaultRowHeightMatched--}
```
public boolean isDefaultRowHeightMatched()
```


Указывает, что высота строки и высота шрифта по умолчанию совпадают

**Returns:**
boolean
### isDefaultRowHidden() {#isDefaultRowHidden--}
```
public boolean isDefaultRowHidden()
```


Указывает, скрыта ли строка по умолчанию.

**Returns:**
boolean
### isDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns) {#isDeletingRangeEnabled-int-int-int-int-}
```
public boolean isDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns)
```


Проверьте, может ли диапазон быть удалён.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | int | Начальный индекс строки диапазона. |
| startColumn | int | Начальный индекс столбца диапазона. |
| totalRows | int | Количество строк в диапазоне. |
| totalColumns | int | Количество столбцов в диапазоне. |

**Returns:**
boolean -
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


Получает перечислитель ячеек.

**Remarks**

При обходе элементов с помощью возвращённого Enumerator коллекцию ячеек не следует изменять(например, операции, которые создают новые Cell/Row или удаляют существующие Cell/Row). В противном случае enumerator может не суметь корректно пройти все ячейки(некоторые элементы могут быть пройдены несколько раз или пропущены).

**Example**

```
         Workbook workbook = new Workbook("template.xlsx");
         	Cells cells = workbook.getWorksheets().get(0).getCells();
 
         	Iterator en = cells.iterator();
         	while (en.hasNext())
         	{
         	    Cell cell = (Cell)en.next();
         	    System.out.println(cell.getName() + ": " + cell.getValue());
         	}
```

**Returns:**
java.util.Iterator - Enumerator ячеек
### linkToXmlMap(String mapName, int row, int column, String path) {#linkToXmlMap-java.lang.String-int-int-java.lang.String-}
```
public void linkToXmlMap(String mapName, int row, int column, String path)
```


Ссылка на XML‑карту.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| mapName | java.lang.String | имя xml карты |
| строка | int | строка целевой ячейки |
| столбец | int | столбец целевой ячейки |
| путь | java.lang.String | путь xml элемента в xml карте |

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

### merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean mergeConflict) {#merge-int-int-int-int-boolean-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean mergeConflict)
```


Объединяет указанный диапазон ячеек в одну ячейку.

**Remarks**

Ссылка на объединённую ячейку осуществляется через адрес верхней левой ячейки в диапазоне. Если mergeConflict равно true и объединённый диапазон конфликтует с другими объединёнными ячейками, другие объединённые ячейки будут автоматически удалены.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | int | Первая строка этого диапазона(нумерация с нуля) |
| firstColumn | int | Первый столбец этого диапазона(нумерация с нуля) |
| totalRows | int | Количество строк(нумерация с 1) |
| totalColumns | int | Количество столбцов (нумерация с 1) |
| mergeConflict | boolean | Конфликт объединения объединённых диапазонов. |

### merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean checkConflict, boolean mergeConflict) {#merge-int-int-int-int-boolean-boolean-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean checkConflict, boolean mergeConflict)
```


Объединяет указанный диапазон ячеек в одну ячейку.

**Remarks**

Ссылка на объединённую ячейку осуществляется через адрес верхней левой ячейки в диапазоне. Если mergeConflict равно true и объединённый диапазон конфликтует с другими объединёнными ячейками, другие объединённые ячейки будут автоматически удалены.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | int | Первая строка этого диапазона(нумерация с нуля) |
| firstColumn | int | Первый столбец этого диапазона(нумерация с нуля) |
| totalRows | int | Количество строк(нумерация с 1) |
| totalColumns | int | Количество столбцов (нумерация с 1) |
| checkConflict | boolean | Указывает, проверяется ли пересечение объединённых ячеек с другими объединёнными ячейками |
| mergeConflict | boolean | Конфликт объединения объединённых диапазонов. |

### moveRange(CellArea sourceArea, int destRow, int destColumn) {#moveRange-com.aspose.cells.CellArea-int-int-}
```
public void moveRange(CellArea sourceArea, int destRow, int destColumn)
```


Перемещает диапазон.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceArea | [CellArea](../../com.aspose.cells/cellarea) | Диапазон, который следует переместить. |
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




### removeDuplicates() {#removeDuplicates--}
```
public void removeDuplicates()
```


Удаляет дублирующиеся строки на листе.

### removeDuplicates(int startRow, int startColumn, int endRow, int endColumn) {#removeDuplicates-int-int-int-int-}
```
public void removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)
```


Удаляет дублирующиеся значения в диапазоне.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | int | Начальная строка. |
| startColumn | int | Начальный столбец |
| endRow | int | Индекс конечной строки. |
| endColumn | int | Индекс конечного столбца. |

### removeDuplicates(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders, int[] columnOffsets) {#removeDuplicates-int-int-int-int-boolean-int---}
```
public void removeDuplicates(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders, int[] columnOffsets)
```


Удаляет дублирующиеся данные диапазона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | int | Начальная строка. |
| startColumn | int | Начальный столбец |
| endRow | int | Индекс конечной строки. |
| endColumn | int | Индекс конечного столбца. |
| hasHeaders | boolean | Указывает, содержит ли диапазон заголовки. |
| columnOffsets | int[] | Смещения столбцов. |

### removeFormulas() {#removeFormulas--}
```
public void removeFormulas()
```


Удаляет все формулы и заменяет их значением формулы.

### retrieveSubtotalSetting(CellArea ca) {#retrieveSubtotalSetting-com.aspose.cells.CellArea-}
```
public SubtotalSetting retrieveSubtotalSetting(CellArea ca)
```


Получает настройки промежуточных итогов диапазона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Диапазон |

**Returns:**
[SubtotalSetting](../../com.aspose.cells/subtotalsetting) - 
### setColumnWidth(int column, double width) {#setColumnWidth-int-double-}
```
public void setColumnWidth(int column, double width)
```


Устанавливает ширину указанной колонки в обычном виде.

**Remarks**

Для электронных таблиц ширина столбца измеряется в количестве символов максимальной ширины цифр 0~9, отображаемых шрифтом обычного стиля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int | Индекс столбца. |
| width | double | Ширина столбца в единицах символов. Ширина столбца должна быть от 0 до 255. |

### setColumnWidthInch(int column, double inches) {#setColumnWidthInch-int-double-}
```
public void setColumnWidthInch(int column, double inches)
```


Устанавливает ширину колонки в дюймах в обычном виде.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int | Индекс столбца. |
| дюймы | double | Количество дюймов. |

### setColumnWidthPixel(int column, int pixels) {#setColumnWidthPixel-int-int-}
```
public void setColumnWidthPixel(int column, int pixels)
```


Устанавливает ширину колонки в пикселях в обычном виде.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int | Индекс столбца. |
| пиксели | int | Количество пикселей. |

### setDefaultColumnHidden(boolean value) {#setDefaultColumnHidden-boolean-}
```
public void setDefaultColumnHidden(boolean value)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setDefaultRowHeightMatched(boolean value) {#setDefaultRowHeightMatched-boolean-}
```
public void setDefaultRowHeightMatched(boolean value)
```


Указывает, что высота строки и высота шрифта по умолчанию совпадают

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setDefaultRowHidden(boolean value) {#setDefaultRowHidden-boolean-}
```
public void setDefaultRowHidden(boolean value)
```


Указывает, скрыта ли строка по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


Устанавливает параметр использования памяти для этих ячеек.

Смотрите [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Заметные ограничения и рекомендуемые операции для некоторых режимов:

| Режим | Примечания | Поддерживается |
| ------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
| [MemorySetting.MEMORY\_PREFERENCE](../../com.aspose.cells/memorysetting\#MEMORY-PREFERENCE) | Cells data will be maintained in compact format to decrease the memory cost. On other hand, the compact data also may cause higher time cost, especially when updating the cells data, or accessing cells/rows randomly | v8.0.0 |
|  | [MemorySetting.FILE\_CACHE](../../com.aspose.cells/memorysetting\#FILE-CACHE) | Когда этот режим используется для любого листа в рабочей книге, следует вызвать [Workbook.dispose()](../../com.aspose.cells/workbook\#dispose--) в конце работы, чтобы освободить все ресурсы, такие как временные файлы. |
 
Случайный доступ к ячейкам приводит к плохой производительности, потому что данные необходимо читать/обновлять случайным и повторяющимся образом (из‑за чего указатель в файле будет изменяться соответственно и операции ввода‑вывода будут требоваться многократно). По возможности, всегда обращайтесь к данным последовательно (строка за строкой).
 
Когда данные одной строки/ячейки изменяются, данные других ячеек/строк также могут быть затронуты (например, данные могут быть смещены/перемещены в другие места для выделения достаточного пространства под изменённые данные). Поэтому каждое изменение любых данных требует синхронизации других существующих объектов (например, объектов Row или Cell). Чтобы получить лучшую производительность, пожалуйста, не поддерживайте одновременно несколько Row/Cell. Обработка их по одной уменьшит синхронизацию данных и немного повысит производительность. | v25.7     |

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMultiThreadReading(boolean value) {#setMultiThreadReading-boolean-}
```
public void setMultiThreadReading(boolean value)
```


Устанавливает, должна ли модель данных ячеек поддерживать многопоточное чтение. Значение по умолчанию этого свойства — false.

**Remarks**

Если в этой коллекции одновременно читаются объекты Row/Cell несколькими потоками, это свойство следует установить в true, иначе могут возникнуть неожиданные результаты. Поддержка многопоточного чтения может ухудшить производительность доступа к объектам Row/Cell из этой коллекции. Обратите внимание, что некоторые функции не поддерживают многопоточное чтение, например форматирование значений (через [Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--), [Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), и т.д.). Поэтому даже при установленном значении true эти API могут давать неожиданные результаты при многопоточном чтении.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setPreserveString(boolean value) {#setPreserveString-boolean-}
```
public void setPreserveString(boolean value)
```


Устанавливает значение, указывающее, сохраняются ли все значения листа как строки. По умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setRowHeight(int row, double height) {#setRowHeight-int-double-}
```
public void setRowHeight(int row, double height)
```


Устанавливает высоту указанной строки.

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
| дюймы | double | Количество дюймов. Должно быть от 0 до 409,5/72. |

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

### setStandardHeight(double value) {#setStandardHeight-double-}
```
public void setStandardHeight(double value)
```


Устанавливает высоту строки по умолчанию в этом листе, в пунктах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setStandardHeightInch(double value) {#setStandardHeightInch-double-}
```
public void setStandardHeightInch(double value)
```


Устанавливает высоту строки по умолчанию в этом листе, в дюймах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setStandardHeightPixels(int value) {#setStandardHeightPixels-int-}
```
public void setStandardHeightPixels(int value)
```


Устанавливает высоту строки по умолчанию в этом листе, в пикселях.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setStandardWidth(double value) {#setStandardWidth-double-}
```
public void setStandardWidth(double value)
```


Устанавливает ширину столбца по умолчанию в листе, в символах.

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

### setStyle(Style value) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style value)
```


Устанавливает стиль листа по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setViewColumnWidthPixel(int column, int pixels) {#setViewColumnWidthPixel-int-int-}
```
public void setViewColumnWidthPixel(int column, int pixels)
```


Устанавливает ширину столбца в разных представлениях.

**Remarks**

Если текущий тип представления — [ViewType.PAGE\_LAYOUT\_VIEW](../../com.aspose.cells/viewtype\#PAGE-LAYOUT-VIEW), ширина столбца будет такой же, как печатная ширина.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int | Индекс столбца. |
| пиксели | int | Ширина в пикселях. |

### showGroupDetail(boolean isVertical, int index) {#showGroupDetail-boolean-int-}
```
public void showGroupDetail(boolean isVertical, int index)
```


Разворачивает сгруппированные строки/столбцы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| isVertical | boolean | True, расширяет сгруппированные строки. |
| индекс | int | Индекс строки/столбца |

### subtotal(CellArea ca, int groupBy, int function, int[] totalList) {#subtotal-com.aspose.cells.CellArea-int-int-int---}
```
public void subtotal(CellArea ca, int groupBy, int function, int[] totalList)
```


Создаёт промежуточные итоги для диапазона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Диапазон |
| groupBy | int | Поле для группировки, как целочисленное смещение, начиная с нуля |
| function | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Функция подытога. |
| totalList | int[] | Массив целочисленных смещений полей, начиная с нуля, указывающий поля, к которым добавляются подытоги. |

### subtotal(CellArea ca, int groupBy, int function, int[] totalList, boolean replace, boolean pageBreaks, boolean summaryBelowData) {#subtotal-com.aspose.cells.CellArea-int-int-int---boolean-boolean-boolean-}
```
public void subtotal(CellArea ca, int groupBy, int function, int[] totalList, boolean replace, boolean pageBreaks, boolean summaryBelowData)
```


Создаёт промежуточные итоги для диапазона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Диапазон |
| groupBy | int | Поле для группировки, как целочисленное смещение, начиная с нуля |
| function | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Функция подытога. |
| totalList | int[] | Массив целочисленных смещений полей, начиная с нуля, указывающий поля, к которым добавляются подытоги. |
| replace | boolean | Указывает, следует ли заменять текущие подытоги |
| pageBreaks | boolean | Указывает, следует ли добавлять разрыв страницы между группами |
| summaryBelowData | boolean | Указывает, следует ли добавлять сводку под данными. |

### textToColumns(int row, int column, int totalRows, TxtLoadOptions options) {#textToColumns-int-int-int-com.aspose.cells.TxtLoadOptions-}
```
public int textToColumns(int row, int column, int totalRows, TxtLoadOptions options)
```


Разделяет содержимое указанного столбца на несколько столбцов..

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |
| столбец | int | Индекс столбца. |
| totalRows | int | Количество строк. |
| options | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | Параметры разделения. |

**Returns:**
int — Общее количество столбцов разделённых значений.
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

Удаляет только внешнюю информацию о группе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| firstIndex | int | Индекс первой строки, которую нужно разгруппировать. |
| lastIndex | int | Индекс последней строки, которую нужно разгруппировать. |

### ungroupRows(int firstIndex, int lastIndex, boolean isAll) {#ungroupRows-int-int-boolean-}
```
public void ungroupRows(int firstIndex, int lastIndex, boolean isAll)
```


Разгруппирует строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| firstIndex | int | Индекс первой строки, которую нужно разгруппировать. |
| lastIndex | int | Индекс последней строки, которую нужно разгруппировать. |
| isAll | boolean | True, удаляет всю информацию о группировке. Иначе удаляет внешнюю информацию о группе. |

### unhideColumn(int column, double width) {#unhideColumn-int-double-}
```
public void unhideColumn(int column, double width)
```


Отображает скрытый столбец

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int | Индекс столбца. |
| width | double | Ширина столбца. |

### unhideColumns(int column, int totalColumns, double width) {#unhideColumns-int-int-double-}
```
public void unhideColumns(int column, int totalColumns, double width)
```


Отображает несколько скрытых столбцов.

**Remarks**

Применяется только к скрытым столбцам.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int | Индекс столбца. |
| totalColumns | int | Номер столбца |
| width | double | Ширина столбца. |

### unhideRow(int row, double height) {#unhideRow-int-double-}
```
public void unhideRow(int row, double height)
```


Отображает скрытую строку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |
| height | double | Высота строки. Высота строки будет изменена только когда строка скрыта и заданное значение высоты положительно. |

### unhideRows(int row, int totalRows, double height) {#unhideRows-int-int-double-}
```
public void unhideRows(int row, int totalRows, double height)
```


Отображает скрытые строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |
| totalRows | int | Номер строки. |
| height | double | Высота строки. Высота строки будет изменена только когда строка скрыта и заданное значение высоты положительно. |

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

