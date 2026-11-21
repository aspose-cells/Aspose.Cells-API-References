---
title: "Celdas"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula una colección de objetos relevantes de celda, como ...etc."
type: docs
url: /es/java/com.aspose.cells/cells/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Cells implements Iterable
```

Encapsula una colección de objetos relevantes de celda, como [Cell](../../com.aspose.cells/cell), [Row](../../com.aspose.cells/row), ...etc.

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
## Métodos

| Método | Descripción |
| --- | --- |
| [addRange(Range rangeObject)](#addRange-com.aspose.cells.Range-) | Agrega una referencia de objeto de rango a las celdas |
| [applyColumnStyle(int column, Style style, StyleFlag flag)](#applyColumnStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Aplica formatos a una columna completa. |
| [applyRowStyle(int row, Style style, StyleFlag flag)](#applyRowStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Aplica formatos a una fila completa. |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Aplica formatos a una hoja de cálculo completa. |
| [checkCell(int row, int column)](#checkCell-int-int-) | Obtiene el elemento [Cell](../../com.aspose.cells/cell) o null en el índice de fila y columna de celda especificados. |
| [checkColumn(int columnIndex)](#checkColumn-int-) | Obtiene el elemento [Column](../../com.aspose.cells/column) o null en el índice de columna especificado. |
| [checkRow(int row)](#checkRow-int-) | Obtiene el elemento [Row](../../com.aspose.cells/row) o null en el índice de fila de celda especificado. |
| [clear()](#clear--) | Borra todos los datos de la hoja de cálculo. |
| [clearContents(CellArea range)](#clearContents-com.aspose.cells.CellArea-) | Borra el contenido de un rango. |
| [clearContents(int startRow, int startColumn, int endRow, int endColumn)](#clearContents-int-int-int-int-) | Borra el contenido de un rango. |
| [clearFormats(CellArea range)](#clearFormats-com.aspose.cells.CellArea-) | Borra el formato de un rango. |
| [clearFormats(int startRow, int startColumn, int endRow, int endColumn)](#clearFormats-int-int-int-int-) | Borra el formato de un rango. |
| [clearMergedCells()](#clearMergedCells--) | Borra todos los rangos combinados. |
| [clearRange(CellArea range)](#clearRange-com.aspose.cells.CellArea-) | Borra el contenido y el formato de un rango. |
| [clearRange(int startRow, int startColumn, int endRow, int endColumn)](#clearRange-int-int-int-int-) | Borra el contenido y el formato de un rango. |
| [convertStringToNumericValue()](#convertStringToNumericValue--) | Convierte todos los datos de cadena en la hoja de cálculo a valor numérico si es posible. |
| [copyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex)](#copyColumn-com.aspose.cells.Cells-int-int-) | Copia datos y formatos de una columna completa. |
| [copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)](#copyColumns-com.aspose.cells.Cells-int-int-int-) | Copia los datos y formatos de columnas completas. |
| [copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber, PasteOptions pasteOptions)](#copyColumns-com.aspose.cells.Cells-int-int-int-com.aspose.cells.PasteOptions-) | Copia datos y formatos de una columna completa. |
| [copyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, int destinationColumnIndex, int destinationTotalColumns)](#copyColumns-com.aspose.cells.Cells-int-int-int-int-) | Copia los datos y formatos de todas las columnas. |
| [copyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex)](#copyRow-com.aspose.cells.Cells-int-int-) | Copia los datos y formatos de una fila completa. |
| [copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)](#copyRows-com.aspose.cells.Cells-int-int-int-) | Copia los datos y formatos de algunas filas completas. |
| [copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions)](#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-) | Copia los datos y formatos de algunas filas completas. |
| [copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)](#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-com.aspose.cells.PasteOptions-) | Copia los datos y formatos de algunas filas completas. |
| [createRange(int firstIndex, int number, boolean isVertical)](#createRange-int-int-boolean-) | Crea un objeto [Range](../../com.aspose.cells/range) a partir de filas de celdas o columnas de celdas. |
| [createRange(int firstRow, int firstColumn, int totalRows, int totalColumns)](#createRange-int-int-int-int-) | Crea un objeto [Range](../../com.aspose.cells/range) a partir de un rango de celdas. |
| [createRange(String address)](#createRange-java.lang.String-) | Crea un objeto [Range](../../com.aspose.cells/range) a partir de una dirección del rango. |
| [createRange(String upperLeftCell, String lowerRightCell)](#createRange-java.lang.String-java.lang.String-) | Crea un objeto [Range](../../com.aspose.cells/range) a partir de un rango de celdas. |
| [deleteBlankColumns()](#deleteBlankColumns--) | Elimina todas las columnas en blanco que no contienen datos. |
| [deleteBlankColumns(DeleteOptions options)](#deleteBlankColumns-com.aspose.cells.DeleteOptions-) | Elimina todas las columnas en blanco que no contienen datos. |
| [deleteBlankRows()](#deleteBlankRows--) | Elimina todas las filas en blanco que no contienen datos ni otros objetos. |
| [deleteBlankRows(DeleteOptions options)](#deleteBlankRows-com.aspose.cells.DeleteOptions-) | Elimina todas las filas en blanco que no contienen datos o algunos objetos especiales como comentarios visibles o tablas dinámicas. |
| [deleteColumn(int columnIndex)](#deleteColumn-int-) | Elimina una columna. |
| [deleteColumn(int columnIndex, boolean updateReference)](#deleteColumn-int-boolean-) | Elimina una columna. |
| [deleteColumns(int columnIndex, int totalColumns, boolean updateReference)](#deleteColumns-int-int-boolean-) | Elimina varias columnas. |
| [deleteColumns(int columnIndex, int totalColumns, DeleteOptions options)](#deleteColumns-int-int-com.aspose.cells.DeleteOptions-) | Elimina varias columnas. |
| [deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)](#deleteRange-int-int-int-int-int-) | Elimina un rango de celdas y desplaza las celdas según la opción de desplazamiento. |
| [deleteRow(int rowIndex)](#deleteRow-int-) | Elimina una fila. |
| [deleteRow(int rowIndex, boolean updateReference)](#deleteRow-int-boolean-) | Elimina una fila. |
| [deleteRows(int rowIndex, int totalRows)](#deleteRows-int-int-) | Elimina varias filas. |
| [deleteRows(int rowIndex, int totalRows, boolean updateReference)](#deleteRows-int-int-boolean-) | Elimina varias filas en la hoja de cálculo. |
| [deleteRows(int rowIndex, int totalRows, DeleteOptions options)](#deleteRows-int-int-com.aspose.cells.DeleteOptions-) | Elimina varias filas en la hoja de cálculo. |
| [dispose()](#dispose--) | Ejecuta tareas definidas por la aplicación asociadas con la liberación, el lanzamiento o el restablecimiento de recursos no administrados. |
| [endCellInColumn(int columnIndex)](#endCellInColumn-int-) | Obtiene la última celda de esta columna. |
| [endCellInColumn(int startRow, int endRow, int startColumn, int endColumn)](#endCellInColumn-int-int-int-int-) | Obtiene la última celda con el índice de columna máximo en este rango. |
| [endCellInRow(int rowIndex)](#endCellInRow-int-) | Obtiene la última celda de esta fila. |
| [endCellInRow(int startRow, int endRow, int startColumn, int endColumn)](#endCellInRow-int-int-int-int-) | Obtiene la última celda con el índice de fila máximo en este rango. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)](#exportArray-int-int-int-int-) | Exporta los datos de la colección [Cells](../../com.aspose.cells/cells) a un objeto de matriz bidimensional. |
| [exportTypeArray(int firstRow, int firstColumn, int totalRows, int totalColumns)](#exportTypeArray-int-int-int-int-) | Exporta el tipo de valor de celda de la colección [Cells](../../com.aspose.cells/cells) a un objeto de matriz bidimensional. |
| [find(Object what, Cell previousCell)](#find-java.lang.Object-com.aspose.cells.Cell-) | Encuentra la celda que contiene el objeto de entrada. |
| [find(Object what, Cell previousCell, FindOptions findOptions)](#find-java.lang.Object-com.aspose.cells.Cell-com.aspose.cells.FindOptions-) | Encuentra la celda que contiene el objeto de entrada. |
| [get(int row, int column)](#get-int-int-) | Obtiene el elemento [Cell](../../com.aspose.cells/cell) en el índice de fila y columna de celda especificados. |
| [get(String cellName)](#get-java.lang.String-) | Obtiene el elemento [Cell](../../com.aspose.cells/cell) con el nombre de celda especificado. |
| [getCellDisplayStyle(int row, int column)](#getCellDisplayStyle-int-int-) | Obtén el estilo de visualización de la celda dada. |
| [getCellDisplayStyle(int row, int column, int adjacentBorders)](#getCellDisplayStyle-int-int-int-) | Obtén el estilo de visualización de la celda dada. |
| [getCellStyle(int row, int column)](#getCellStyle-int-int-) | Obtenga el estilo de la celda dada. |
| [getCellsWithPlaceInCellPicture()](#getCellsWithPlaceInCellPicture--) | Obtiene todas las celdas que contienen una imagen incrustada. |
| [getClass()](#getClass--) |  |
| [getColumnOriginalWidthPoint(int column)](#getColumnOriginalWidthPoint-int-) | Obtiene la altura original de la columna en unidades de punto si la columna está oculta. |
| [getColumnWidth(int column)](#getColumnWidth-int-) | Obtiene el ancho (en unidades de caracteres) de la columna especificada en vista normal. |
| [getColumnWidth(int column, boolean isOriginal, int unitType)](#getColumnWidth-int-boolean-int-) | Obtiene el ancho de la columna. |
| [getColumnWidthInch(int column)](#getColumnWidthInch-int-) | Obtiene el ancho de la columna especificada en vista normal, en unidades de pulgadas. |
| [getColumnWidthPixel(int column)](#getColumnWidthPixel-int-) | Obtiene el ancho de la columna especificada en vista normal, en unidades de píxel. |
| [getColumnWidthPixel(int column, boolean original)](#getColumnWidthPixel-int-boolean-) | Obtiene el ancho de la columna especificada en vista normal, en unidades de píxel. |
| [getColumns()](#getColumns--) | Obtiene la colección de objetos [Column](../../com.aspose.cells/column) que representan las columnas individuales en esta hoja de cálculo. |
| [getCount()](#getCount--) | Obtiene el recuento total de objetos Cell instanciados. |
| [getCountLarge()](#getCountLarge--) | Obtiene el recuento total de objetos Cell instanciados. |
| [getDependents(boolean isAll, int row, int column)](#getDependents-boolean-int-int-) | Obtenga todas las celdas que hacen referencia a la celda específica. |
| [getDependentsInCalculation(int row, int column, boolean recursive)](#getDependentsInCalculation-int-int-boolean-) | Obtiene todas las celdas cuyo resultado calculado depende de la celda específica. |
| [getFirstCell()](#getFirstCell--) | Obtiene la primera celda en esta hoja de cálculo. |
| [getFirstDataRow(int column)](#getFirstDataRow-int-) | Obtiene el índice de la primera fila de la celda que contiene datos en la columna especificada. |
| [getGroupedColumnOutlineLevel(int columnIndex)](#getGroupedColumnOutlineLevel-int-) | Obtiene el nivel de esquema (basado en cero) de la columna. |
| [getGroupedRowOutlineLevel(int rowIndex)](#getGroupedRowOutlineLevel-int-) | Obtiene el nivel de esquema (basado en cero) de la fila. |
| [getLastCell()](#getLastCell--) | Obtiene la última celda en esta hoja de cálculo. |
| [getLastDataRow(int column)](#getLastDataRow-int-) | Obtiene el índice de la última fila de la celda que contiene datos en la columna especificada. |
| [getMaxColumn()](#getMaxColumn--) | Índice máximo de columna de aquellas celdas que han sido instanciadas en la colección (no incluye la columna donde el estilo está definido para toda la columna pero no se ha instanciado ninguna celda en ella). |
| [getMaxDataColumn()](#getMaxDataColumn--) | Índice máximo de columna de la celda que contiene datos. |
| [getMaxDataRow()](#getMaxDataRow--) | Índice máximo de fila de la celda que contiene datos. |
| [getMaxDisplayRange()](#getMaxDisplayRange--) | Obtiene el rango máximo que incluye datos, celdas combinadas y formas. |
| [getMaxGroupedColumnOutlineLevel()](#getMaxGroupedColumnOutlineLevel--) | Obtiene el nivel máximo de esquema de columna agrupada (basado en cero). |
| [getMaxGroupedRowOutlineLevel()](#getMaxGroupedRowOutlineLevel--) | Obtiene el nivel máximo de esquema de fila agrupada (basado en cero). |
| [getMaxRow()](#getMaxRow--) | Índice máximo de fila de la celda que contiene datos o estilo. |
| [getMemorySetting()](#getMemorySetting--) | Obtiene la opción de uso de memoria para estas celdas. |
| [getMergedAreas()](#getMergedAreas--) | Obtiene todas las celdas combinadas. |
| [getMergedCells()](#getMergedCells--) | Obtiene la colección de celdas combinadas. |
| [getMinColumn()](#getMinColumn--) | Índice de columna mínimo de esas celdas que han sido instanciadas en la colección (no incluye la columna donde el estilo está definido para toda la columna pero no se ha instanciado ninguna celda en ella). |
| [getMinDataColumn()](#getMinDataColumn--) | Índice de columna mínimo de la celda que contiene datos. |
| [getMinDataRow()](#getMinDataRow--) | Índice de fila mínimo de la celda que contiene datos. |
| [getMinRow()](#getMinRow--) | Índice de fila mínimo de la celda que contiene datos o estilo. |
| [getMultiThreadReading()](#getMultiThreadReading--) | Obtiene si el modelo de datos de las celdas debe soportar la lectura Multi-Thread. |
| [getOdsCellFields()](#getOdsCellFields--) | Obtiene la lista de campos de ods. |
| [getPreserveString()](#getPreserveString--) | Obtiene un valor que indica si todos los valores de la hoja de cálculo se conservan como cadenas. |
| [getRanges()](#getRanges--) | Obtiene la colección de objetos [Range](../../com.aspose.cells/range) creados en tiempo de ejecución. |
| [getRowEnumerator()](#getRowEnumerator--) | Obtiene el enumerador de filas. |
| [getRowHeight(int row)](#getRowHeight-int-) | Obtiene la altura de una fila especificada, en unidades de puntos. |
| [getRowHeight(int row, boolean isOriginal, int unitType)](#getRowHeight-int-boolean-int-) | Obtiene la altura de la fila. |
| [getRowHeightInch(int row)](#getRowHeightInch-int-) | Obtiene la altura de una fila especificada en unidades de pulgadas. |
| [getRowHeightPixel(int row)](#getRowHeightPixel-int-) | Obtiene la altura de una fila especificada en unidades de píxeles. |
| [getRowOriginalHeightPoint(int row)](#getRowOriginalHeightPoint-int-) | Obtiene la altura original de la fila en unidades de punto si la fila está oculta. |
| [getRows()](#getRows--) | Obtiene la colección de objetos [Row](../../com.aspose.cells/row) que representan las filas individuales en esta hoja de cálculo. |
| [getStandardHeight()](#getStandardHeight--) | Obtiene la altura de fila predeterminada en esta hoja de cálculo, en unidades de puntos. |
| [getStandardHeightInch()](#getStandardHeightInch--) | Obtiene la altura de fila predeterminada en esta hoja de cálculo, en unidades de pulgadas. |
| [getStandardHeightPixels()](#getStandardHeightPixels--) | Obtiene la altura de fila predeterminada en esta hoja de cálculo, en unidades de píxeles. |
| [getStandardWidth()](#getStandardWidth--) | Obtiene el ancho de columna predeterminado en la hoja de cálculo, en unidades de caracteres. |
| [getStandardWidthInch()](#getStandardWidthInch--) | Obtiene el ancho de columna predeterminado en la hoja de cálculo, en unidades de pulgadas. |
| [getStandardWidthPixels()](#getStandardWidthPixels--) | Obtiene el ancho de columna predeterminado en la hoja de cálculo, en unidades de píxeles. |
| [getStyle()](#getStyle--) | Obtiene el estilo predeterminado de la hoja de cálculo. |
| [getViewColumnWidthPixel(int column)](#getViewColumnWidthPixel-int-) | Obtenga el ancho en diferentes tipos de vista. |
| [getViewRowHeight(int row)](#getViewRowHeight-int-) | Obtiene la altura de una fila especificada. |
| [getViewRowHeightInch(int row)](#getViewRowHeightInch-int-) | Obtiene la altura de una fila especificada en unidades de pulgadas. |
| [groupColumns(int firstIndex, int lastIndex)](#groupColumns-int-int-) | Agrupa columnas. |
| [groupColumns(int firstIndex, int lastIndex, boolean isHidden)](#groupColumns-int-int-boolean-) | Agrupa columnas. |
| [groupRows(int firstIndex, int lastIndex)](#groupRows-int-int-) | Agrupa filas. |
| [groupRows(int firstIndex, int lastIndex, boolean isHidden)](#groupRows-int-int-boolean-) | Agrupa filas. |
| [hashCode()](#hashCode--) |  |
| [hideColumn(int column)](#hideColumn-int-) | Oculta una columna. |
| [hideColumns(int column, int totalColumns)](#hideColumns-int-int-) | Oculta varias columnas. |
| [hideGroupDetail(boolean isVertical, int index)](#hideGroupDetail-boolean-int-) | Contrae las filas/columnas agrupadas. |
| [hideRow(int row)](#hideRow-int-) | Oculta una fila. |
| [hideRows(int row, int totalRows)](#hideRows-int-int-) | Oculta varias filas. |
| [importArray(double[] doubleArray, int firstRow, int firstColumn, boolean isVertical)](#importArray-double---int-int-boolean-) | Importa una matriz de double a una hoja de cálculo. |
| [importArray(double[][] doubleArray, int firstRow, int firstColumn)](#importArray-double-----int-int-) | Importa una matriz bidimensional de double a una hoja de cálculo. |
| [importArray(int[] intArray, int firstRow, int firstColumn, boolean isVertical)](#importArray-int---int-int-boolean-) | Importa una matriz de integer a una hoja de cálculo. |
| [importArray(int[][] intArray, int firstRow, int firstColumn)](#importArray-int-----int-int-) | Importa una matriz bidimensional de integer a una hoja de cálculo. |
| [importArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)](#importArray-java.lang.String---int-int-boolean-) | Importa una matriz de string a una hoja de cálculo. |
| [importArray(String[][] stringArray, int firstRow, int firstColumn)](#importArray-java.lang.String-----int-int-) | Importa una matriz bidimensional de string a una hoja de cálculo. |
| [importArrayList(ArrayList arrayList, int firstRow, int firstColumn, boolean isVertical)](#importArrayList-java.util.ArrayList-int-int-boolean-) | Importa un arraylist de datos a una hoja de cálculo. |
| [importCSV(InputStream stream, TxtLoadOptions options, int firstRow, int firstColumn)](#importCSV-java.io.InputStream-com.aspose.cells.TxtLoadOptions-int-int-) | Importa un archivo CSV a las celdas. |
| [importCSV(InputStream stream, String splitter, boolean convertNumericData, int firstRow, int firstColumn)](#importCSV-java.io.InputStream-java.lang.String-boolean-int-int-) | Importa un archivo CSV a las celdas. |
| [importCSV(String fileName, TxtLoadOptions options, int firstRow, int firstColumn)](#importCSV-java.lang.String-com.aspose.cells.TxtLoadOptions-int-int-) | Importa un archivo CSV a las celdas. |
| [importCSV(String fileName, String splitter, boolean convertNumericData, int firstRow, int firstColumn)](#importCSV-java.lang.String-java.lang.String-boolean-int-int-) | Importa un archivo CSV a las celdas. |
| [importCustomObjects(Collection list, int firstRow, int firstColumn, ImportTableOptions options)](#importCustomObjects-java.util.Collection-int-int-com.aspose.cells.ImportTableOptions-) | Importa objetos personalizados. |
| [importCustomObjects(Collection list, String[] propertyNames, boolean isPropertyNameShown, int firstRow, int firstColumn, int rowNumber, boolean insertRows, String dateFormatString, boolean convertStringToNumber)](#importCustomObjects-java.util.Collection-java.lang.String---boolean-int-int-int-boolean-java.lang.String-boolean-) | Importa objetos personalizados. |
| [importData(ICellsDataTable table, int firstRow, int firstColumn, ImportTableOptions options)](#importData-com.aspose.cells.ICellsDataTable-int-int-com.aspose.cells.ImportTableOptions-) | Importa datos de una tabla de datos personalizada. |
| [importFormulaArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)](#importFormulaArray-java.lang.String---int-int-boolean-) | Importa una matriz de fórmulas a una hoja de cálculo. |
| [importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical)](#importObjectArray-java.lang.Object---int-int-boolean-) | Importa una matriz de datos a una hoja de cálculo. |
| [importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical, int skip)](#importObjectArray-java.lang.Object---int-int-boolean-int-) | Importa una matriz de datos a una hoja de cálculo. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-int-int-boolean-) | Importa datos de un objeto ResultSet a la hoja de cálculo. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)](#importResultSet-java.sql.ResultSet-int-int-boolean-java.lang.String-boolean-) | Importa datos de un objeto ResultSet a la hoja de cálculo. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, ImportTableOptions options)](#importResultSet-java.sql.ResultSet-int-int-com.aspose.cells.ImportTableOptions-) | Importa datos de un objeto ResultSet a la hoja de cálculo. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-) | Importa datos de un objeto ResultSet a la hoja de cálculo. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)](#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-java.lang.String-boolean-) | Importa datos de un objeto ResultSet a la hoja de cálculo. |
| [importResultSet(ResultSet rs, String startCell, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-java.lang.String-boolean-) | Importa datos de un objeto ResultSet a la hoja de cálculo. |
| [importResultSet(ResultSet rs, String startCell, ImportTableOptions options)](#importResultSet-java.sql.ResultSet-java.lang.String-com.aspose.cells.ImportTableOptions-) | Importa datos de un objeto ResultSet a la hoja de cálculo. |
| [importResultSet(ResultSet rs, String startCell, int rowNum, int columnNum, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-java.lang.String-int-int-boolean-) | Importa datos de un objeto ResultSet a la hoja de cálculo. |
| [importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn)](#importTwoDimensionArray-java.lang.Object-----int-int-) | Importa una matriz bidimensional de datos a una hoja de cálculo. |
| [importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn, boolean convertStringToNumber)](#importTwoDimensionArray-java.lang.Object-----int-int-boolean-) | Importa una matriz bidimensional de datos a una hoja de cálculo. |
| [importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, boolean convertStringToNumber)](#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-boolean-) | Importa una matriz bidimensional de datos a una hoja de cálculo. |
| [importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, TxtLoadOptions opts)](#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-com.aspose.cells.TxtLoadOptions-) | Importa una matriz bidimensional de datos a una hoja de cálculo. |
| [insertColumn(int columnIndex)](#insertColumn-int-) | Inserta una nueva columna en la hoja de cálculo. |
| [insertColumn(int columnIndex, boolean updateReference)](#insertColumn-int-boolean-) | Inserta una nueva columna en la hoja de cálculo. |
| [insertColumns(int columnIndex, int totalColumns)](#insertColumns-int-int-) | Inserta varias columnas en la hoja de cálculo. |
| [insertColumns(int columnIndex, int totalColumns, boolean updateReference)](#insertColumns-int-int-boolean-) | Inserta varias columnas en la hoja de cálculo. |
| [insertColumns(int columnIndex, int totalColumns, InsertOptions options)](#insertColumns-int-int-com.aspose.cells.InsertOptions-) | Inserta varias columnas en la hoja de cálculo. |
| [insertCutCells(Range cutRange, int row, int column, int shiftType)](#insertCutCells-com.aspose.cells.Range-int-int-int-) | Insertar rango recortado. |
| [insertRange(CellArea area, int shiftType)](#insertRange-com.aspose.cells.CellArea-int-) | Inserta un rango de celdas y desplaza las celdas según la opción de desplazamiento. |
| [insertRange(CellArea area, int shiftNumber, int shiftType)](#insertRange-com.aspose.cells.CellArea-int-int-) | Inserta un rango de celdas y desplaza las celdas según la opción de desplazamiento. |
| [insertRange(CellArea area, int shiftNumber, int shiftType, boolean updateReference)](#insertRange-com.aspose.cells.CellArea-int-int-boolean-) | Inserta un rango de celdas y desplaza las celdas según la opción de desplazamiento. |
| [insertRow(int rowIndex)](#insertRow-int-) | Inserta una nueva fila en la hoja de cálculo. |
| [insertRows(int rowIndex, int totalRows)](#insertRows-int-int-) | Inserta varias filas en la hoja de cálculo. |
| [insertRows(int rowIndex, int totalRows, boolean updateReference)](#insertRows-int-int-boolean-) | Inserta varias filas en la hoja de cálculo. |
| [insertRows(int rowIndex, int totalRows, InsertOptions options)](#insertRows-int-int-com.aspose.cells.InsertOptions-) | Inserta varias filas en la hoja de cálculo. |
| [isBlankColumn(int columnIndex)](#isBlankColumn-int-) | Comprueba si la columna dada está vacía (no contiene datos). |
| [isColumnHidden(int columnIndex)](#isColumnHidden-int-) | Comprueba si una columna en el índice dado está oculta. |
| [isDefaultColumnHidden()](#isDefaultColumnHidden--) |  |
| [isDefaultRowHeightMatched()](#isDefaultRowHeightMatched--) | Indica que la altura de la fila y la altura de fuente predeterminada coinciden |
| [isDefaultRowHidden()](#isDefaultRowHidden--) | Indica si la fila está oculta por defecto. |
| [isDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns)](#isDeletingRangeEnabled-int-int-int-int-) | Comprueba si el rango puede ser eliminado. |
| [isRowHidden(int rowIndex)](#isRowHidden-int-) | Comprueba si una fila en el índice dado está oculta. |
| [iterator()](#iterator--) | Obtiene el enumerador de celdas. |
| [linkToXmlMap(String mapName, int row, int column, String path)](#linkToXmlMap-java.lang.String-int-int-java.lang.String-) | Enlace a un mapa XML. |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#merge-int-int-int-int-) | Fusiona un rango especificado de celdas en una sola celda. |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean mergeConflict)](#merge-int-int-int-int-boolean-) | Fusiona un rango especificado de celdas en una sola celda. |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean checkConflict, boolean mergeConflict)](#merge-int-int-int-int-boolean-boolean-) | Fusiona un rango especificado de celdas en una sola celda. |
| [moveRange(CellArea sourceArea, int destRow, int destColumn)](#moveRange-com.aspose.cells.CellArea-int-int-) | Mueve el rango. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeDuplicates()](#removeDuplicates--) | Elimina filas duplicadas en la hoja. |
| [removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)](#removeDuplicates-int-int-int-int-) | Elimina valores duplicados en el rango. |
| [removeDuplicates(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders, int[] columnOffsets)](#removeDuplicates-int-int-int-int-boolean-int---) | Elimina datos duplicados del rango. |
| [removeFormulas()](#removeFormulas--) | Elimina todas las fórmulas y las reemplaza con el valor de la fórmula. |
| [retrieveSubtotalSetting(CellArea ca)](#retrieveSubtotalSetting-com.aspose.cells.CellArea-) | Recupera la configuración de subtotales del rango. |
| [setColumnWidth(int column, double width)](#setColumnWidth-int-double-) | Establece el ancho de la columna especificada en vista normal. |
| [setColumnWidthInch(int column, double inches)](#setColumnWidthInch-int-double-) | Establece el ancho de la columna en unidades de pulgadas en vista normal. |
| [setColumnWidthPixel(int column, int pixels)](#setColumnWidthPixel-int-int-) | Establece el ancho de la columna en unidades de píxeles en vista normal. |
| [setDefaultColumnHidden(boolean value)](#setDefaultColumnHidden-boolean-) |  |
| [setDefaultRowHeightMatched(boolean value)](#setDefaultRowHeightMatched-boolean-) | Indica que la altura de la fila y la altura de fuente predeterminada coinciden |
| [setDefaultRowHidden(boolean value)](#setDefaultRowHidden-boolean-) | Indica si la fila está oculta por defecto. |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Establece la opción de uso de memoria para estas celdas. |
| [setMultiThreadReading(boolean value)](#setMultiThreadReading-boolean-) | Establece si el modelo de datos de celdas debe soportar lectura multihilo. |
| [setPreserveString(boolean value)](#setPreserveString-boolean-) | Establece un valor que indica si todos los valores de la hoja de cálculo se conservan como cadenas. |
| [setRowHeight(int row, double height)](#setRowHeight-int-double-) | Establece la altura de la fila especificada. |
| [setRowHeightInch(int row, double inches)](#setRowHeightInch-int-double-) | Establece la altura de la fila en unidades de pulgadas. |
| [setRowHeightPixel(int row, int pixels)](#setRowHeightPixel-int-int-) | Establece la altura de la fila en unidades de píxeles. |
| [setStandardHeight(double value)](#setStandardHeight-double-) | Establece la altura predeterminada de la fila en esta hoja de cálculo, en unidades de puntos. |
| [setStandardHeightInch(double value)](#setStandardHeightInch-double-) | Establece la altura predeterminada de la fila en esta hoja de cálculo, en unidades de pulgadas. |
| [setStandardHeightPixels(int value)](#setStandardHeightPixels-int-) | Establece la altura predeterminada de la fila en esta hoja de cálculo, en unidades de píxeles. |
| [setStandardWidth(double value)](#setStandardWidth-double-) | Establece el ancho predeterminado de la columna en la hoja de cálculo, en unidades de caracteres. |
| [setStandardWidthInch(double value)](#setStandardWidthInch-double-) | Establece el ancho predeterminado de la columna en la hoja de cálculo, en unidades de pulgadas. |
| [setStandardWidthPixels(int value)](#setStandardWidthPixels-int-) | Establece el ancho predeterminado de la columna en la hoja de cálculo, en unidades de píxeles. |
| [setStyle(Style value)](#setStyle-com.aspose.cells.Style-) | Establece el estilo predeterminado de la hoja de cálculo. |
| [setViewColumnWidthPixel(int column, int pixels)](#setViewColumnWidthPixel-int-int-) | Establece el ancho de la columna en diferentes vistas. |
| [showGroupDetail(boolean isVertical, int index)](#showGroupDetail-boolean-int-) | Expande las filas/columnas agrupadas. |
| [subtotal(CellArea ca, int groupBy, int function, int[] totalList)](#subtotal-com.aspose.cells.CellArea-int-int-int---) | Crea subtotales para el rango. |
| [subtotal(CellArea ca, int groupBy, int function, int[] totalList, boolean replace, boolean pageBreaks, boolean summaryBelowData)](#subtotal-com.aspose.cells.CellArea-int-int-int---boolean-boolean-boolean-) | Crea subtotales para el rango. |
| [textToColumns(int row, int column, int totalRows, TxtLoadOptions options)](#textToColumns-int-int-int-com.aspose.cells.TxtLoadOptions-) | Divide el contenido en la columna especificada en múltiples columnas.. |
| [toString()](#toString--) |  |
| [unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#unMerge-int-int-int-int-) | Descombina un rango especificado de celdas combinadas. |
| [ungroupColumns(int firstIndex, int lastIndex)](#ungroupColumns-int-int-) | Desagrupa columnas. |
| [ungroupRows(int firstIndex, int lastIndex)](#ungroupRows-int-int-) | Desagrupa filas. |
| [ungroupRows(int firstIndex, int lastIndex, boolean isAll)](#ungroupRows-int-int-boolean-) | Desagrupa filas. |
| [unhideColumn(int column, double width)](#unhideColumn-int-double-) | Desoculta una columna |
| [unhideColumns(int column, int totalColumns, double width)](#unhideColumns-int-int-double-) | Desoculta varias columnas. |
| [unhideRow(int row, double height)](#unhideRow-int-double-) | Desoculta una fila. |
| [unhideRows(int row, int totalRows, double height)](#unhideRows-int-int-double-) | Desoculta las filas ocultas. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addRange(Range rangeObject) {#addRange-com.aspose.cells.Range-}
```
public void addRange(Range rangeObject)
```


Agrega una referencia de objeto de rango a las celdas

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rangeObject | [Range](../../com.aspose.cells/range) | El objeto de rango se contendrá en las celdas |

### applyColumnStyle(int column, Style style, StyleFlag flag) {#applyColumnStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyColumnStyle(int column, Style style, StyleFlag flag)
```


Aplica formatos a una columna completa.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | El índice de columna. |
| style | [Style](../../com.aspose.cells/style) | El objeto de estilo que se aplicará. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Banderas que indican las propiedades de formato aplicadas. |

### applyRowStyle(int row, Style style, StyleFlag flag) {#applyRowStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyRowStyle(int row, Style style, StyleFlag flag)
```


Aplica formatos a una fila completa.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | El índice de fila. |
| style | [Style](../../com.aspose.cells/style) | El objeto de estilo que se aplicará. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Banderas que indican las propiedades de formato aplicadas. |

### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Aplica formatos a una hoja de cálculo completa.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | El objeto de estilo que se aplicará. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Banderas que indican las propiedades de formato aplicadas. |

### checkCell(int row, int column) {#checkCell-int-int-}
```
public Cell checkCell(int row, int column)
```


Obtiene el elemento [Cell](../../com.aspose.cells/cell) o null en el índice de fila y columna de celda especificados.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila |
| columna | int | Índice de columna |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Return Cell object if a Cell object exists. Return null if the cell does not exist.
### checkColumn(int columnIndex) {#checkColumn-int-}
```
public Column checkColumn(int columnIndex)
```


Obtiene el elemento [Column](../../com.aspose.cells/column) o null en el índice de columna especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | int | El índice de columna. |

**Returns:**
[Column](../../com.aspose.cells/column) - The Column object.
### checkRow(int row) {#checkRow-int-}
```
public Row checkRow(int row)
```


Obtiene el elemento [Row](../../com.aspose.cells/row) o null en el índice de fila de celda especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila |

**Returns:**
[Row](../../com.aspose.cells/row) - Returns [Row](../../com.aspose.cells/row) object If the row object does exist, otherwise returns null.
### clear() {#clear--}
```
public void clear()
```


Borra todos los datos de la hoja de cálculo.

### clearContents(CellArea range) {#clearContents-com.aspose.cells.CellArea-}
```
public void clearContents(CellArea range)
```


Borra el contenido de un rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| range | [CellArea](../../com.aspose.cells/cellarea) | Rango a borrar. |

### clearContents(int startRow, int startColumn, int endRow, int endColumn) {#clearContents-int-int-int-int-}
```
public void clearContents(int startRow, int startColumn, int endRow, int endColumn)
```


Borra el contenido de un rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | int | Índice de fila inicial. |
| startColumn | int | Índice de columna inicial. |
| endRow | int | Índice de fila final. |
| endColumn | int | Índice de columna final. |

### clearFormats(CellArea range) {#clearFormats-com.aspose.cells.CellArea-}
```
public void clearFormats(CellArea range)
```


Borra el formato de un rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| range | [CellArea](../../com.aspose.cells/cellarea) | Rango a borrar. |

### clearFormats(int startRow, int startColumn, int endRow, int endColumn) {#clearFormats-int-int-int-int-}
```
public void clearFormats(int startRow, int startColumn, int endRow, int endColumn)
```


Borra el formato de un rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | int | Índice de fila inicial. |
| startColumn | int | Índice de columna inicial. |
| endRow | int | Índice de fila final. |
| endColumn | int | Índice de columna final. |

### clearMergedCells() {#clearMergedCells--}
```
public void clearMergedCells()
```


Borra todos los rangos combinados.

### clearRange(CellArea range) {#clearRange-com.aspose.cells.CellArea-}
```
public void clearRange(CellArea range)
```


Borra el contenido y el formato de un rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| range | [CellArea](../../com.aspose.cells/cellarea) | Rango a borrar. |

### clearRange(int startRow, int startColumn, int endRow, int endColumn) {#clearRange-int-int-int-int-}
```
public void clearRange(int startRow, int startColumn, int endRow, int endColumn)
```


Borra el contenido y el formato de un rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | int | Índice de fila inicial. |
| startColumn | int | Índice de columna inicial. |
| endRow | int | Índice de fila final. |
| endColumn | int | Índice de columna final. |

### convertStringToNumericValue() {#convertStringToNumericValue--}
```
public void convertStringToNumericValue()
```


Convierte todos los datos de cadena en la hoja de cálculo a valor numérico si es posible.

### copyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex) {#copyColumn-com.aspose.cells.Cells-int-int-}
```
public void copyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex)
```


Copia datos y formatos de una columna completa.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | El objeto Source Cells contiene datos y formatos para copiar. |
| sourceColumnIndex | int | Índice de columna de origen. |
| destinationColumnIndex | int | Índice de columna de destino. |

### copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber) {#copyColumns-com.aspose.cells.Cells-int-int-int-}
```
public void copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)
```


Copia los datos y formatos de columnas completas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | El objeto Source Cells contiene datos y formatos para copiar. |
| sourceColumnIndex | int | Índice de columna de origen. |
| destinationColumnIndex | int | Índice de columna de destino. |
| columnNumber | int | El número de columna copiada. |

### copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber, PasteOptions pasteOptions) {#copyColumns-com.aspose.cells.Cells-int-int-int-com.aspose.cells.PasteOptions-}
```
public void copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber, PasteOptions pasteOptions)
```


Copia datos y formatos de una columna completa.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | El objeto Source Cells contiene datos y formatos para copiar. |
| sourceColumnIndex | int | Índice de columna de origen. |
| destinationColumnIndex | int | Índice de columna de destino. |
| columnNumber | int | El número de columna copiada. |
| pasteOptions | [PasteOptions](../../com.aspose.cells/pasteoptions) | las opciones de pegado. |

### copyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, int destinationColumnIndex, int destinationTotalColumns) {#copyColumns-com.aspose.cells.Cells-int-int-int-int-}
```
public void copyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, int destinationColumnIndex, int destinationTotalColumns)
```


Copia los datos y formatos de todas las columnas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | El objeto Source Cells contiene datos y formatos para copiar. |
| sourceColumnIndex | int | Índice de columna de origen. |
| sourceTotalColumns | int | El número de columnas de origen. |
| destinationColumnIndex | int | Índice de columna de destino. |
| destinationTotalColumns | int | El número de columnas de destino. |

### copyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex) {#copyRow-com.aspose.cells.Cells-int-int-}
```
public void copyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex)
```


Copia los datos y formatos de una fila completa.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | El objeto Source Cells contiene datos y formatos para copiar. |
| sourceRowIndex | int | Índice de fila de origen. |
| destinationRowIndex | int | Índice de fila de destino. |

### copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber) {#copyRows-com.aspose.cells.Cells-int-int-int-}
```
public void copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```


Copia los datos y formatos de algunas filas completas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | El objeto Source Cells contiene datos y formatos para copiar. |
| sourceRowIndex | int | Índice de fila de origen. |
| destinationRowIndex | int | Índice de fila de destino. |
| rowNumber | int | El número de fila copiada. |

### copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions) {#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-}
```
public void copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions)
```


Copia los datos y formatos de algunas filas completas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | El objeto Source Cells contiene datos y formatos para copiar. |
| sourceRowIndex | int | Índice de fila de origen. |
| destinationRowIndex | int | Índice de fila de destino. |
| rowNumber | int | El número de fila copiada. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Las opciones de copia. |

### copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions) {#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-com.aspose.cells.PasteOptions-}
```
public void copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)
```


Copia los datos y formatos de algunas filas completas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceCells0 | [Cells](../../com.aspose.cells/cells) | El objeto Source Cells contiene datos y formatos para copiar. |
| sourceRowIndex | int | Índice de fila de origen. |
| destinationRowIndex | int | Índice de fila de destino. |
| rowNumber | int | El número de fila copiada. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Las opciones de copia. |
| pasteOptions | [PasteOptions](../../com.aspose.cells/pasteoptions) | las opciones de pegado. |

### createRange(int firstIndex, int number, boolean isVertical) {#createRange-int-int-boolean-}
```
public Range createRange(int firstIndex, int number, boolean isVertical)
```


Crea un objeto [Range](../../com.aspose.cells/range) a partir de filas de celdas o columnas de celdas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstIndex | int | Índice de la primera fila o índice de la primera columna, basado en cero. |
| número | int | Número total de filas o columnas, basado en uno. |
| isVertical | boolean | Verdadero - Rango creado a partir de columnas de celdas. Falso - Rango creado a partir de filas de celdas. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object.
### createRange(int firstRow, int firstColumn, int totalRows, int totalColumns) {#createRange-int-int-int-int-}
```
public Range createRange(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Crea un objeto [Range](../../com.aspose.cells/range) a partir de un rango de celdas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | int | Primera fila de este rango |
| firstColumn | int | Primera columna de este rango |
| totalRows | int | Número de filas |
| totalColumns | int | Número de columnas |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### createRange(String address) {#createRange-java.lang.String-}
```
public Range createRange(String address)
```


Crea un objeto [Range](../../com.aspose.cells/range) a partir de una dirección del rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dirección | java.lang.String | La dirección del rango. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### createRange(String upperLeftCell, String lowerRightCell) {#createRange-java.lang.String-java.lang.String-}
```
public Range createRange(String upperLeftCell, String lowerRightCell)
```


Crea un objeto [Range](../../com.aspose.cells/range) a partir de un rango de celdas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| upperLeftCell | java.lang.String | Nombre de la celda superior izquierda. |
| lowerRightCell | java.lang.String | Nombre de la celda inferior derecha. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### deleteBlankColumns() {#deleteBlankColumns--}
```
public void deleteBlankColumns()
```


Elimina todas las columnas en blanco que no contienen datos.

### deleteBlankColumns(DeleteOptions options) {#deleteBlankColumns-com.aspose.cells.DeleteOptions-}
```
public void deleteBlankColumns(DeleteOptions options)
```


Elimina todas las columnas en blanco que no contienen datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | Las opciones de eliminación de rango. |

### deleteBlankRows() {#deleteBlankRows--}
```
public void deleteBlankRows()
```


Elimina todas las filas en blanco que no contienen datos ni otros objetos.

### deleteBlankRows(DeleteOptions options) {#deleteBlankRows-com.aspose.cells.DeleteOptions-}
```
public void deleteBlankRows(DeleteOptions options)
```


Elimina todas las filas en blanco que no contienen datos o algunos objetos especiales como comentarios visibles o tablas dinámicas.

**Remarks**

Para las filas en blanco que se eliminarán, no solo se requiere que [Row.isBlank()](../../com.aspose.cells/row\#isBlank--) sea verdadero, sino que también no debe haber ningún comentario visible definido para cualquier celda en esas filas, y ninguna tabla dinámica cuyo rango intersecte con ellas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | Las opciones de eliminación de rango. |

### deleteColumn(int columnIndex) {#deleteColumn-int-}
```
public void deleteColumn(int columnIndex)
```


Elimina una columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | int | Índice de la columna a eliminar. |

### deleteColumn(int columnIndex, boolean updateReference) {#deleteColumn-int-boolean-}
```
public void deleteColumn(int columnIndex, boolean updateReference)
```


Elimina una columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | int | Índice de la columna a eliminar. |
| updateReference | boolean | Indica si se actualizan referencias en otras hojas de cálculo. |

### deleteColumns(int columnIndex, int totalColumns, boolean updateReference) {#deleteColumns-int-int-boolean-}
```
public void deleteColumns(int columnIndex, int totalColumns, boolean updateReference)
```


Elimina varias columnas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | int | Índice de la primera columna a eliminar. |
| totalColumns | int | Cantidad de columnas a eliminar. |
| updateReference | boolean | Indica si se actualizan referencias en otras hojas de cálculo. |

### deleteColumns(int columnIndex, int totalColumns, DeleteOptions options) {#deleteColumns-int-int-com.aspose.cells.DeleteOptions-}
```
public void deleteColumns(int columnIndex, int totalColumns, DeleteOptions options)
```


Elimina varias columnas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | int | Índice de la primera columna a eliminar. |
| totalColumns | int | Cantidad de columnas a eliminar. |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | Opciones para la operación de eliminación |

### deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType) {#deleteRange-int-int-int-int-int-}
```
public void deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)
```


Elimina un rango de celdas y desplaza las celdas según la opción de desplazamiento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | int | Índice de fila inicial. |
| startColumn | int | Índice de columna inicial. |
| endRow | int | Índice de fila final. |
| endColumn | int | Índice de columna final. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Opción de desplazar celdas. |

### deleteRow(int rowIndex) {#deleteRow-int-}
```
public void deleteRow(int rowIndex)
```


Elimina una fila.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | int | Índice de la fila a eliminar. |

### deleteRow(int rowIndex, boolean updateReference) {#deleteRow-int-boolean-}
```
public void deleteRow(int rowIndex, boolean updateReference)
```


Elimina una fila.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | int | Índice de la fila a eliminar. |
| updateReference | boolean | Indica si se actualizan referencias en otras hojas de cálculo. |

### deleteRows(int rowIndex, int totalRows) {#deleteRows-int-int-}
```
public boolean deleteRows(int rowIndex, int totalRows)
```


Elimina varias filas.

**Remarks**

Si el rango eliminado contiene la parte superior (no completa) de la tabla (ListObject), el rango no podrá ser eliminado y no se hará nada. Funciona de la misma manera que en MS Excel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | int | El índice de la primera fila a eliminar. |
| totalRows | int | Cantidad de filas a eliminar. |

**Returns:**
boolean
### deleteRows(int rowIndex, int totalRows, boolean updateReference) {#deleteRows-int-int-boolean-}
```
public boolean deleteRows(int rowIndex, int totalRows, boolean updateReference)
```


Elimina varias filas en la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | int | Índice de la primera fila a eliminar. |
| totalRows | int | Cantidad de filas a eliminar. |
| updateReference | boolean | Indica si se actualizan referencias en otras hojas de cálculo. |

**Returns:**
boolean -
### deleteRows(int rowIndex, int totalRows, DeleteOptions options) {#deleteRows-int-int-com.aspose.cells.DeleteOptions-}
```
public boolean deleteRows(int rowIndex, int totalRows, DeleteOptions options)
```


Elimina varias filas en la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | int | Índice de la primera fila a eliminar. |
| totalRows | int | Cantidad de filas a eliminar. |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | Opciones para la operación de eliminación |

**Returns:**
boolean -
### dispose() {#dispose--}
```
public void dispose()
```


Ejecuta tareas definidas por la aplicación asociadas con la liberación, el lanzamiento o el restablecimiento de recursos no administrados.

### endCellInColumn(int columnIndex) {#endCellInColumn-int-}
```
public Cell endCellInColumn(int columnIndex)
```


Obtiene la última celda de esta columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | int | Índice de columna. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### endCellInColumn(int startRow, int endRow, int startColumn, int endColumn) {#endCellInColumn-int-int-int-int-}
```
public Cell endCellInColumn(int startRow, int endRow, int startColumn, int endColumn)
```


Obtiene la última celda con el índice de columna máximo en este rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | int | Índice de fila inicial. |
| endRow | int | Índice de fila final. |
| startColumn | int | Índice de columna inicial. |
| endColumn | int | Índice de columna final. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### endCellInRow(int rowIndex) {#endCellInRow-int-}
```
public Cell endCellInRow(int rowIndex)
```


Obtiene la última celda de esta fila.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | int | Índice de fila. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### endCellInRow(int startRow, int endRow, int startColumn, int endColumn) {#endCellInRow-int-int-int-int-}
```
public Cell endCellInRow(int startRow, int endRow, int startColumn, int endColumn)
```


Obtiene la última celda con el índice de fila máximo en este rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | int | Índice de fila inicial. |
| endRow | int | Índice de fila final. |
| startColumn | int | Índice de columna inicial. |
| endColumn | int | Índice de columna final. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns) {#exportArray-int-int-int-int-}
```
public Object[][] exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Exporta los datos de la colección [Cells](../../com.aspose.cells/cells) a un objeto de matriz bidimensional.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | int | El número de fila de la primera celda a exportar. |
| firstColumn | int | El número de columna de la primera celda a exportar |
| totalRows | int | Número de filas a exportar |
| totalColumns | int | Número de columnas a exportar |

**Returns:**
java.lang.Object[][] - Objeto de matriz de valores de celda exportados.
### exportTypeArray(int firstRow, int firstColumn, int totalRows, int totalColumns) {#exportTypeArray-int-int-int-int-}
```
public int[][] exportTypeArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Exporta el tipo de valor de celda de la colección [Cells](../../com.aspose.cells/cells) a un objeto de matriz bidimensional.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | int | El número de fila de la primera celda a exportar. |
| firstColumn | int | El número de columna de la primera celda a exportar |
| totalRows | int | Número de filas a exportar. |
| totalColumns | int | Número de columnas a exportar. |

**Returns:**
int[][] - [CellValueType](../../com.aspose.cells/cellvaluetype). Objeto de matriz exportado que representa los tipos de valor de celda.
### find(Object what, Cell previousCell) {#find-java.lang.Object-com.aspose.cells.Cell-}
```
public Cell find(Object what, Cell previousCell)
```


Encuentra la celda que contiene el objeto de entrada.

**Remarks**

Devuelve null (Nothing) si no se encuentra ninguna celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| qué | java.lang.Object | El objeto a buscar. El tipo debe ser int,double,DateTime,string,bool. |
| previousCell | [Cell](../../com.aspose.cells/cell) | Celda anterior con el mismo objeto. Este parámetro puede establecerse en null si se busca desde el inicio. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### find(Object what, Cell previousCell, FindOptions findOptions) {#find-java.lang.Object-com.aspose.cells.Cell-com.aspose.cells.FindOptions-}
```
public Cell find(Object what, Cell previousCell, FindOptions findOptions)
```


Encuentra la celda que contiene el objeto de entrada.

**Remarks**

Devuelve null (Nothing) si no se encuentra ninguna celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| qué | java.lang.Object | El objeto a buscar. El tipo debe ser int,double,DateTime,string,bool. |
| previousCell | [Cell](../../com.aspose.cells/cell) | Celda anterior con el mismo objeto. Este parámetro puede establecerse en null si se busca desde el inicio. |
| findOptions | [FindOptions](../../com.aspose.cells/findoptions) | Opciones de búsqueda |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### get(int row, int column) {#get-int-int-}
```
public Cell get(int row, int column)
```


Obtiene el elemento [Cell](../../com.aspose.cells/cell) en el índice de fila y columna de celda especificados.

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
         Cell cell = cells.get(0, 0);	//Gets the cell at "A1"
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila. |
| columna | int | Índice de columna. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - The [Cell](../../com.aspose.cells/cell) object.
### get(String cellName) {#get-java.lang.String-}
```
public Cell get(String cellName)
```


Obtiene el elemento [Cell](../../com.aspose.cells/cell) con el nombre de celda especificado.

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
         Cell cell = cells.get("A1");	//Gets the cell at "A1"
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellName | java.lang.String | Nombre de la celda, incluyendo su letra de columna y número de fila, por ejemplo A5. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - A [Cell](../../com.aspose.cells/cell) object
### getCellDisplayStyle(int row, int column) {#getCellDisplayStyle-int-int-}
```
public Style getCellDisplayStyle(int row, int column)
```


Obtén el estilo de visualización de la celda dada.

**Remarks**

Lo mismo con [Cell.getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--), y lo mismo al usar [BorderType.SIDE\_BORDERS](../../com.aspose.cells/bordertype\#SIDE-BORDERS) para [getCellDisplayStyle(int,int,int)](../../com.aspose.cells/cells\#getCellDisplayStyle-int-int-int-).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | índice de fila de la celda dada |
| columna | int | columna de la celda dada |

**Returns:**
[Style](../../com.aspose.cells/style) - the display style of given cell.
### getCellDisplayStyle(int row, int column, int adjacentBorders) {#getCellDisplayStyle-int-int-int-}
```
public Style getCellDisplayStyle(int row, int column, int adjacentBorders)
```


Obtén el estilo de visualización de la celda dada.

**Remarks**

Si la celda también está afectada por otras configuraciones como formato condicional, objetos de lista, etc., entonces el estilo de visualización puede ser diferente de [getCellStyle(int,int)](../../com.aspose.cells/cells\#getCellStyle-int-int-). Y debido a que esas configuraciones también pueden aplicarse a celdas vacías (no existentes), usar este método puede evitar la instanciación de esas celdas vacías, por lo que el rendimiento será mejor que obtener la instancia Cell de Cells y luego llamar a [Cell.getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | índice de fila de la celda dada |
| columna | int | columna de la celda dada |
| adjacentBorders | int | [BorderType](../../com.aspose.cells/bordertype). Indica qué bordes deben revisarse y ajustarse según los bordes de las celdas adyacentes. Consulte la descripción del mismo parámetro de [Cell.getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-). |

**Returns:**
[Style](../../com.aspose.cells/style) - the display style of given cell.
### getCellStyle(int row, int column) {#getCellStyle-int-int-}
```
public Style getCellStyle(int row, int column)
```


Obtenga el estilo de la celda dada.

**Remarks**

El estilo devuelto es solo el establecido para la celda o heredado de la fila/columna de la celda, no incluye las propiedades aplicadas por otras configuraciones como formatos condicionales.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | índice de fila |
| columna | int | columna |

**Returns:**
[Style](../../com.aspose.cells/style) - the style of given cell.
### getCellsWithPlaceInCellPicture() {#getCellsWithPlaceInCellPicture--}
```
public Iterator getCellsWithPlaceInCellPicture()
```


Obtiene todas las celdas que contienen una imagen incrustada.

**Remarks**

Si no hay ninguna imagen configurada como "Place in Cell" en esta hoja de cálculo, se devolverá null.

**Returns:**
java.util.Iterator - Enumerador para enumerar todos los objetos Cell que contienen una imagen incrustada
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


Obtiene la altura original de la columna en unidades de punto si la columna está oculta.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método Cells.GetColumnWidth(int ,bool , CellsUnitType ). Este método será eliminado 12 meses después desde abril de 2024. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | El índice de fila. |

**Returns:**
double - Ancho de la columna en vista normal.
### getColumnWidth(int column) {#getColumnWidth-int-}
```
public double getColumnWidth(int column)
```


Obtiene el ancho (en unidades de caracteres) de la columna especificada en vista normal.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | Índice de columna |

**Returns:**
double - Ancho de la columna. Para una hoja de cálculo, el ancho de columna se mide como el número de caracteres del ancho máximo de dígitos de los números 0~9 tal como se renderizan en la fuente del estilo normal.
### getColumnWidth(int column, boolean isOriginal, int unitType) {#getColumnWidth-int-boolean-int-}
```
public double getColumnWidth(int column, boolean isOriginal, int unitType)
```


Obtiene el ancho de la columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | El índice de columna. |
| isOriginal | boolean | Indica si se obtiene el ancho original. |
| unitType | int | [CellsUnitType](../../com.aspose.cells/cellsunittype). |

**Returns:**
double -
### getColumnWidthInch(int column) {#getColumnWidthInch-int-}
```
public double getColumnWidthInch(int column)
```


Obtiene el ancho de la columna especificada en vista normal, en unidades de pulgadas.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método Cells.GetColumnWidth(int ,bool , CellsUnitType ). Este método será eliminado 12 meses después desde abril de 2024. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | Índice de columna |

**Returns:**
double - Ancho de la columna en vista normal.
### getColumnWidthPixel(int column) {#getColumnWidthPixel-int-}
```
public int getColumnWidthPixel(int column)
```


Obtiene el ancho de la columna especificada en vista normal, en unidades de píxel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | Índice de columna |

**Returns:**
int - Ancho de la columna en vista normal.
### getColumnWidthPixel(int column, boolean original) {#getColumnWidthPixel-int-boolean-}
```
public int getColumnWidthPixel(int column, boolean original)
```


Obtiene el ancho de la columna especificada en vista normal, en unidades de píxel.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método Cells.GetColumnWidth(int ,bool , CellsUnitType ). Este método será eliminado 12 meses después desde abril de 2024. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | Índice de columna |
| original | boolean | Indica si se devuelve el ancho original incluso cuando la columna está oculta |

**Returns:**
int - Ancho de la columna en vista normal.
### getColumns() {#getColumns--}
```
public ColumnCollection getColumns()
```


Obtiene la colección de objetos [Column](../../com.aspose.cells/column) que representan las columnas individuales en esta hoja de cálculo.

**Returns:**
[ColumnCollection](../../com.aspose.cells/columncollection)
### getCount() {#getCount--}
```
public int getCount()
```


Obtiene el recuento total de objetos Cell instanciados.

**Returns:**
int
### getCountLarge() {#getCountLarge--}
```
public long getCountLarge()
```


Obtiene el recuento total de objetos Cell instanciados.

**Returns:**
long
### getDependents(boolean isAll, int row, int column) {#getDependents-boolean-int-int-}
```
public Cell[] getDependents(boolean isAll, int row, int column)
```


Obtenga todas las celdas que hacen referencia a la celda específica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isAll | boolean | Indica si se verifica otras hojas de cálculo |
| fila | int | El índice de fila. |
| columna | int | El índice de columna. |

**Returns:**
com.aspose.cells.Cell[] -
### getDependentsInCalculation(int row, int column, boolean recursive) {#getDependentsInCalculation-int-int-boolean-}
```
public Iterator getDependentsInCalculation(int row, int column, boolean recursive)
```


Obtiene todas las celdas cuyo resultado calculado depende de la celda específica.

**Remarks**

Para usar este método, asegúrese de que el libro de trabajo se haya configurado con el valor true para [FormulaSettings.getEnableCalculationChain()](../../com.aspose.cells/formulasettings\#getEnableCalculationChain--) y se haya calculado completamente con esta configuración. Si no hay ninguna referencia de fórmula a esta celda, se devolverá null. Para más detalles y un ejemplo, consulte [Cell.getDependentsInCalculation(boolean)](../../com.aspose.cells/cell\#getDependentsInCalculation-boolean-)

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila de la celda específica |
| columna | int | Índice de columna de la celda específica. |
| recursive | boolean | Indica si devuelve los dependientes que no hacen referencia directamente a la celda específica, sino a otras hojas de esa celda. |

**Returns:**
java.util.Iterator - Enumerador para enumerar todos los dependientes (objetos Cell)
### getFirstCell() {#getFirstCell--}
```
public Cell getFirstCell()
```


Obtiene la primera celda en esta hoja de cálculo.

**Remarks**

Devuelve null si no hay datos en la hoja de cálculo.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getFirstDataRow(int column) {#getFirstDataRow-int-}
```
public int getFirstDataRow(int column)
```


Obtiene el índice de la primera fila de la celda que contiene datos en la columna especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | Índice de columna. |

**Returns:**
int - índice de la primera fila.
### getGroupedColumnOutlineLevel(int columnIndex) {#getGroupedColumnOutlineLevel-int-}
```
public int getGroupedColumnOutlineLevel(int columnIndex)
```


Obtiene el nivel de esquema (basado en cero) de la columna.

**Remarks**

Si la columna no está agrupada, devuelve cero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | int | El índice de columna |

**Returns:**
int - Nivel de contorno de la columna
### getGroupedRowOutlineLevel(int rowIndex) {#getGroupedRowOutlineLevel-int-}
```
public int getGroupedRowOutlineLevel(int rowIndex)
```


Obtiene el nivel de esquema (basado en cero) de la fila.

**Remarks**

Si la fila no está agrupada, devuelve cero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | int | El índice de fila. |

**Returns:**
int - Nivel de contorno (basado en cero) de la fila.
### getLastCell() {#getLastCell--}
```
public Cell getLastCell()
```


Obtiene la última celda en esta hoja de cálculo.

**Remarks**

Devuelve null si no hay datos en la hoja de cálculo.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getLastDataRow(int column) {#getLastDataRow-int-}
```
public int getLastDataRow(int column)
```


Obtiene el índice de la última fila de la celda que contiene datos en la columna especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | Índice de columna. |

**Returns:**
int - índice de la última fila.
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


Índice máximo de columna de aquellas celdas que han sido instanciadas en la colección (no incluye la columna donde el estilo está definido para toda la columna pero no se ha instanciado ninguna celda en ella).

**Remarks**

Devuelve -1 si no se ha instanciado ninguna celda.

**Returns:**
int
### getMaxDataColumn() {#getMaxDataColumn--}
```
public int getMaxDataColumn()
```


Índice máximo de columna de la celda que contiene datos.

**Remarks**

\-1 se devolverá si no hay ninguna celda que contenga datos. Esta propiedad necesita iterar y comprobar todas las celdas en una hoja de cálculo de forma dinámica, por lo que es un proceso que consume tiempo y no debe invocarse repetidamente, como usarla directamente como condición en un bucle.

**Returns:**
int
### getMaxDataRow() {#getMaxDataRow--}
```
public int getMaxDataRow()
```


Índice máximo de fila de la celda que contiene datos.

**Remarks**

Devuelve -1 si no hay ninguna celda que contenga datos. Esta propiedad necesita iterar y comprobar celdas y filas de forma dinámica, por lo que es un proceso que consume tiempo y no debe invocarse repetidamente, como usarla directamente como condición en un bucle.

**Returns:**
int
### getMaxDisplayRange() {#getMaxDisplayRange--}
```
public Range getMaxDisplayRange()
```


Obtiene el rango máximo que incluye datos, celdas combinadas y formas.

**Remarks**

Devuelve null si la hoja de cálculo está vacía desde Aspose.Cells 21.5.2.

**Returns:**
[Range](../../com.aspose.cells/range)
### getMaxGroupedColumnOutlineLevel() {#getMaxGroupedColumnOutlineLevel--}
```
public int getMaxGroupedColumnOutlineLevel()
```


Obtiene el nivel máximo de esquema de columna agrupada (basado en cero).

**Returns:**
int - Nivel máximo de contorno de columna agrupada (basado en cero)
### getMaxGroupedRowOutlineLevel() {#getMaxGroupedRowOutlineLevel--}
```
public int getMaxGroupedRowOutlineLevel()
```


Obtiene el nivel máximo de esquema de fila agrupada (basado en cero).

**Returns:**
int - Nivel máximo de contorno de fila agrupada (basado en cero)
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


Índice máximo de fila de la celda que contiene datos o estilo.

**Remarks**

Devuelve -1 si no hay ninguna celda que contenga datos o estilo en la hoja de cálculo. Esta propiedad necesita iterar y comprobar celdas y filas de forma dinámica, por lo que es un proceso que consume tiempo y no debe invocarse repetidamente, como usarla directamente como condición en un bucle.

**Returns:**
int
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


Obtiene la opción de uso de memoria para estas celdas.

Ver [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Límites notables y operaciones recomendadas para algunos modos:

| Modo | Observaciones | Compatible |
| ------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
| [MemorySetting.MEMORY\_PREFERENCE](../../com.aspose.cells/memorysetting\#MEMORY-PREFERENCE) | Cells data will be maintained in compact format to decrease the memory cost. On other hand, the compact data also may cause higher time cost, especially when updating the cells data, or accessing cells/rows randomly | v8.0.0 |
|  | [MemorySetting.FILE\_CACHE](../../com.aspose.cells/memorysetting\#FILE-CACHE) | Cuando se usa este modo para cualquier hoja de cálculo en un libro, se debe llamar a [Workbook.dispose()](../../com.aspose.cells/workbook\#dispose--) al final del trabajo para liberar todos los recursos, como los archivos temporales. |
 
Acceder a celdas de forma aleatoria producirá un bajo rendimiento porque los datos deben leerse/actualizarse de forma aleatoria y repetida (por lo que el puntero en el archivo se cambiará en consecuencia y se requerirán operaciones de E/S repetidamente). Si es posible, acceda siempre a los datos de forma secuencial (fila por fila).
 
Cuando se modifica el dato de una fila/celda, los datos de otras celdas/filas también pueden verse afectados (por ejemplo, los datos pueden desplazarse/moverse a otros lugares para asignar suficiente espacio al dato modificado). Por lo tanto, cada cambio de cualquier dato requiere la sincronización de otros objetos existentes (como objetos Row o Cell). Así, para obtener un mejor rendimiento, no mantenga múltiples Rows/Cells al mismo tiempo. Procesarlos uno por uno reducirá la sincronización de datos y mejorará un poco el rendimiento. | v25.7     |

**Returns:**
int
### getMergedAreas() {#getMergedAreas--}
```
public CellArea[] getMergedAreas()
```


Obtiene todas las celdas combinadas.

**Returns:**
com.aspose.cells.CellArea[]
### getMergedCells() {#getMergedCells--}
```
public ArrayList getMergedCells()
```


Obtiene la colección de celdas combinadas.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método Cells.GetMergedAreas(). Este método será eliminado 12 meses después, desde noviembre de 2023. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
java.util.ArrayList
### getMinColumn() {#getMinColumn--}
```
public int getMinColumn()
```


Índice de columna mínimo de esas celdas que han sido instanciadas en la colección (no incluye la columna donde el estilo está definido para toda la columna pero no se ha instanciado ninguna celda en ella).

**Remarks**

Esta propiedad necesita iterar y comprobar celdas y filas de forma dinámica, por lo que es un proceso que consume tiempo y no debe invocarse repetidamente, como usarla directamente como condición en un bucle.

**Returns:**
int
### getMinDataColumn() {#getMinDataColumn--}
```
public int getMinDataColumn()
```


Índice de columna mínimo de la celda que contiene datos.

**Remarks**

\-1 se devolverá si no hay ninguna celda que contenga datos. Esta propiedad necesita iterar y comprobar todas las celdas en una hoja de cálculo de forma dinámica, por lo que es un proceso que consume tiempo y no debe invocarse repetidamente, como usarla directamente como condición en un bucle.

**Returns:**
int
### getMinDataRow() {#getMinDataRow--}
```
public int getMinDataRow()
```


Índice de fila mínimo de la celda que contiene datos.

**Remarks**

Devuelve -1 si no hay ninguna celda que contenga datos. Esta propiedad necesita iterar y comprobar celdas y filas de forma dinámica, por lo que es un proceso que consume tiempo y no debe invocarse repetidamente, como usarla directamente como condición en un bucle.

**Returns:**
int
### getMinRow() {#getMinRow--}
```
public int getMinRow()
```


Índice de fila mínimo de la celda que contiene datos o estilo.

**Remarks**

Esta propiedad necesita iterar y comprobar celdas y filas de forma dinámica, por lo que es un proceso que consume tiempo y no debe invocarse repetidamente, como usarla directamente como condición en un bucle.

**Returns:**
int
### getMultiThreadReading() {#getMultiThreadReading--}
```
public boolean getMultiThreadReading()
```


Obtiene si el modelo de datos de celdas debe soportar la lectura Multi-Thread. El valor predeterminado de esta propiedad es false.

**Remarks**

Si hay varios hilos leyendo objetos Row/Cell en esta colección de forma concurrente, esta propiedad debe establecerse en true; de lo contrario, pueden producirse resultados inesperados. Soportar la lectura Multi-Thread puede degradar el rendimiento al acceder a objetos Row/Cell de esta colección. Tenga en cuenta que algunas funciones no pueden soportar la lectura Multi-Thread, como el formato de valores (por ejemplo, [Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--), [Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), etc.). Por lo tanto, incluso con esta propiedad establecida en true, esas API aún pueden dar resultados inesperados al leer en modo Multi-Thread.

**Returns:**
boolean
### getOdsCellFields() {#getOdsCellFields--}
```
public OdsCellFieldCollection getOdsCellFields()
```


Obtiene la lista de campos de ods.

**Returns:**
[OdsCellFieldCollection](../../com.aspose.cells/odscellfieldcollection)
### getPreserveString() {#getPreserveString--}
```
public boolean getPreserveString()
```


Obtiene un valor que indica si todos los valores de la hoja de cálculo se conservan como cadenas. El valor predeterminado es false.

**Returns:**
boolean
### getRanges() {#getRanges--}
```
public RangeCollection getRanges()
```


Obtiene la colección de objetos [Range](../../com.aspose.cells/range) creados en tiempo de ejecución.

**Returns:**
[RangeCollection](../../com.aspose.cells/rangecollection)
### getRowEnumerator() {#getRowEnumerator--}
```
public Iterator getRowEnumerator()
```


Obtiene el enumerador de filas.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método RowCollection.GetEnumerator(). Este método será eliminado 12 meses después, a partir de mayo de 2023. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
java.util.Iterator - El enumerador de filas.
### getRowHeight(int row) {#getRowHeight-int-}
```
public double getRowHeight(int row)
```


Obtiene la altura de una fila especificada, en unidades de puntos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila |

**Returns:**
double - Altura de la fila
### getRowHeight(int row, boolean isOriginal, int unitType) {#getRowHeight-int-boolean-int-}
```
public double getRowHeight(int row, boolean isOriginal, int unitType)
```


Obtiene la altura de la fila.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | El índice de fila. |
| isOriginal | boolean | Indica si devuelve la altura original de la fila o 0 para una fila oculta. |
| unitType | int | [CellsUnitType](../../com.aspose.cells/cellsunittype). Tipo de unidad del valor de altura devuelto |

**Returns:**
double - Altura de la fila
### getRowHeightInch(int row) {#getRowHeightInch-int-}
```
public double getRowHeightInch(int row)
```


Obtiene la altura de una fila especificada en unidades de pulgadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila |

**Returns:**
double - Altura de la fila
### getRowHeightPixel(int row) {#getRowHeightPixel-int-}
```
public int getRowHeightPixel(int row)
```


Obtiene la altura de una fila especificada en unidades de píxeles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila |

**Returns:**
int - Altura de la fila
### getRowOriginalHeightPoint(int row) {#getRowOriginalHeightPoint-int-}
```
public double getRowOriginalHeightPoint(int row)
```


Obtiene la altura original de la fila en unidades de punto si la fila está oculta.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método Cells.GetRowHeight(int,bool,CellsUnitType). Este método será eliminado 12 meses después, a partir de abril de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | El índice de fila. |

**Returns:**
double -
### getRows() {#getRows--}
```
public RowCollection getRows()
```


Obtiene la colección de objetos [Row](../../com.aspose.cells/row) que representan las filas individuales en esta hoja de cálculo.

**Returns:**
[RowCollection](../../com.aspose.cells/rowcollection)
### getStandardHeight() {#getStandardHeight--}
```
public double getStandardHeight()
```


Obtiene la altura de fila predeterminada en esta hoja de cálculo, en unidades de puntos.

**Returns:**
double
### getStandardHeightInch() {#getStandardHeightInch--}
```
public double getStandardHeightInch()
```


Obtiene la altura de fila predeterminada en esta hoja de cálculo, en unidades de pulgadas.

**Returns:**
double
### getStandardHeightPixels() {#getStandardHeightPixels--}
```
public int getStandardHeightPixels()
```


Obtiene la altura de fila predeterminada en esta hoja de cálculo, en unidades de píxeles.

**Returns:**
int
### getStandardWidth() {#getStandardWidth--}
```
public double getStandardWidth()
```


Obtiene el ancho de columna predeterminado en la hoja de cálculo, en unidades de caracteres.

**Returns:**
double
### getStandardWidthInch() {#getStandardWidthInch--}
```
public double getStandardWidthInch()
```


Obtiene el ancho de columna predeterminado en la hoja de cálculo, en unidades de pulgadas.

**Returns:**
double
### getStandardWidthPixels() {#getStandardWidthPixels--}
```
public int getStandardWidthPixels()
```


Obtiene el ancho de columna predeterminado en la hoja de cálculo, en unidades de píxeles.

**Returns:**
int
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Obtiene el estilo predeterminado de la hoja de cálculo.

**Returns:**
[Style](../../com.aspose.cells/style)
### getViewColumnWidthPixel(int column) {#getViewColumnWidthPixel-int-}
```
public int getViewColumnWidthPixel(int column)
```


Obtenga el ancho en diferentes tipos de vista.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | El índice de columna. |

**Returns:**
int - el ancho de la columna en unidades de píxeles
### getViewRowHeight(int row) {#getViewRowHeight-int-}
```
public double getViewRowHeight(int row)
```


Obtiene la altura de una fila especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila. |

**Returns:**
double - Altura de la fila.
### getViewRowHeightInch(int row) {#getViewRowHeightInch-int-}
```
public double getViewRowHeightInch(int row)
```


Obtiene la altura de una fila especificada en unidades de pulgadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila |

**Returns:**
double - Altura de la fila
### groupColumns(int firstIndex, int lastIndex) {#groupColumns-int-int-}
```
public void groupColumns(int firstIndex, int lastIndex)
```


Agrupa columnas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstIndex | int | El índice de la primera columna a agrupar. |
| lastIndex | int | El índice de la última columna a agrupar. |

### groupColumns(int firstIndex, int lastIndex, boolean isHidden) {#groupColumns-int-int-boolean-}
```
public void groupColumns(int firstIndex, int lastIndex, boolean isHidden)
```


Agrupa columnas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstIndex | int | El índice de la primera columna a agrupar. |
| lastIndex | int | El índice de la última columna a agrupar. |
| isHidden | boolean | Especifica si las columnas agrupadas están ocultas. |

### groupRows(int firstIndex, int lastIndex) {#groupRows-int-int-}
```
public void groupRows(int firstIndex, int lastIndex)
```


Agrupa filas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstIndex | int | El índice de la primera fila a agrupar. |
| lastIndex | int | El índice de la última fila a agrupar. |

### groupRows(int firstIndex, int lastIndex, boolean isHidden) {#groupRows-int-int-boolean-}
```
public void groupRows(int firstIndex, int lastIndex, boolean isHidden)
```


Agrupa filas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstIndex | int | El índice de la primera fila a agrupar. |
| lastIndex | int | El índice de la última fila a agrupar. |
| isHidden | boolean | Especifica si las filas agrupadas están ocultas. |

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


Oculta una columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | Índice de columna. |

### hideColumns(int column, int totalColumns) {#hideColumns-int-int-}
```
public void hideColumns(int column, int totalColumns)
```


Oculta varias columnas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | Índice de columna. |
| totalColumns | int | Número de columna. |

### hideGroupDetail(boolean isVertical, int index) {#hideGroupDetail-boolean-int-}
```
public void hideGroupDetail(boolean isVertical, int index)
```


Contrae las filas/columnas agrupadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isVertical | boolean | True, colapsar las filas agrupadas. |
| índice | int | El índice de fila/columna |

### hideRow(int row) {#hideRow-int-}
```
public void hideRow(int row)
```


Oculta una fila.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila. |

### hideRows(int row, int totalRows) {#hideRows-int-int-}
```
public void hideRows(int row, int totalRows)
```


Oculta varias filas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | El índice de fila. |
| totalRows | int | El número de fila. |

### importArray(double[] doubleArray, int firstRow, int firstColumn, boolean isVertical) {#importArray-double---int-int-boolean-}
```
public void importArray(double[] doubleArray, int firstRow, int firstColumn, boolean isVertical)
```


Importa una matriz de double a una hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| doubleArray | double[] | Array de double. |
| firstRow | int | El número de fila de la primera celda en la que importar. |
| firstColumn | int | El número de columna de la primera celda en la que importar. |
| isVertical | boolean | Especifica importar datos verticalmente u horizontalmente. |

### importArray(double[][] doubleArray, int firstRow, int firstColumn) {#importArray-double-----int-int-}
```
public void importArray(double[][] doubleArray, int firstRow, int firstColumn)
```


Importa una matriz bidimensional de double a una hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| doubleArray | double[][] | Array de double bidimensional. |
| firstRow | int | El número de fila de la primera celda en la que importar. |
| firstColumn | int | El número de columna de la primera celda en la que importar. |

### importArray(int[] intArray, int firstRow, int firstColumn, boolean isVertical) {#importArray-int---int-int-boolean-}
```
public void importArray(int[] intArray, int firstRow, int firstColumn, boolean isVertical)
```


Importa una matriz de integer a una hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| intArray | int[] | Array de entero. |
| firstRow | int | El número de fila de la primera celda en la que importar. |
| firstColumn | int | El número de columna de la primera celda en la que importar. |
| isVertical | boolean | Especifica importar datos verticalmente u horizontalmente. |

### importArray(int[][] intArray, int firstRow, int firstColumn) {#importArray-int-----int-int-}
```
public void importArray(int[][] intArray, int firstRow, int firstColumn)
```


Importa una matriz bidimensional de integer a una hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| intArray | int[][] | Array de entero bidimensional. |
| firstRow | int | El número de fila de la primera celda en la que importar. |
| firstColumn | int | El número de columna de la primera celda en la que importar. |

### importArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical) {#importArray-java.lang.String---int-int-boolean-}
```
public void importArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)
```


Importa una matriz de string a una hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stringArray | java.lang.String[] | Array de cadena. |
| firstRow | int | El número de fila de la primera celda en la que importar. |
| firstColumn | int | El número de columna de la primera celda en la que importar. |
| isVertical | boolean | Especifica importar datos verticalmente u horizontalmente. |

### importArray(String[][] stringArray, int firstRow, int firstColumn) {#importArray-java.lang.String-----int-int-}
```
public void importArray(String[][] stringArray, int firstRow, int firstColumn)
```


Importa una matriz bidimensional de string a una hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stringArray | java.lang.String[][] | Array de cadena bidimensional. |
| firstRow | int | El número de fila de la primera celda en la que importar. |
| firstColumn | int | El número de columna de la primera celda en la que importar. |

### importArrayList(ArrayList arrayList, int firstRow, int firstColumn, boolean isVertical) {#importArrayList-java.util.ArrayList-int-int-boolean-}
```
public void importArrayList(ArrayList arrayList, int firstRow, int firstColumn, boolean isVertical)
```


Importa un arraylist de datos a una hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arrayList | java.util.ArrayList | Datos arraylist. |
| firstRow | int | El número de fila de la primera celda en la que importar. |
| firstColumn | int | El número de columna de la primera celda en la que importar. |
| isVertical | boolean | Especifica importar datos verticalmente u horizontalmente. |

### importCSV(InputStream stream, TxtLoadOptions options, int firstRow, int firstColumn) {#importCSV-java.io.InputStream-com.aspose.cells.TxtLoadOptions-int-int-}
```
public void importCSV(InputStream stream, TxtLoadOptions options, int firstRow, int firstColumn)
```


Importa un archivo CSV a las celdas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.InputStream | El flujo del archivo CSV. |
| options | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | Las opciones de carga para leer el archivo de texto |
| firstRow | int | El número de fila de la primera celda en la que importar. |
| firstColumn | int | El número de columna de la primera celda en la que importar. |

### importCSV(InputStream stream, String splitter, boolean convertNumericData, int firstRow, int firstColumn) {#importCSV-java.io.InputStream-java.lang.String-boolean-int-int-}
```
public void importCSV(InputStream stream, String splitter, boolean convertNumericData, int firstRow, int firstColumn)
```


Importa un archivo CSV a las celdas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.InputStream | El flujo del archivo CSV. |
| splitter | java.lang.String | El divisor |
| convertNumericData | boolean | Si la cadena en el archivo de texto se convierte en datos numéricos. |
| firstRow | int | El número de fila de la primera celda en la que importar. |
| firstColumn | int | El número de columna de la primera celda en la que importar. |

### importCSV(String fileName, TxtLoadOptions options, int firstRow, int firstColumn) {#importCSV-java.lang.String-com.aspose.cells.TxtLoadOptions-int-int-}
```
public void importCSV(String fileName, TxtLoadOptions options, int firstRow, int firstColumn)
```


Importa un archivo CSV a las celdas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | java.lang.String | El nombre del archivo CSV. |
| options | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | Las opciones de carga para leer el archivo de texto |
| firstRow | int | El número de fila de la primera celda en la que importar. |
| firstColumn | int | El número de columna de la primera celda en la que importar. |

### importCSV(String fileName, String splitter, boolean convertNumericData, int firstRow, int firstColumn) {#importCSV-java.lang.String-java.lang.String-boolean-int-int-}
```
public void importCSV(String fileName, String splitter, boolean convertNumericData, int firstRow, int firstColumn)
```


Importa un archivo CSV a las celdas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | java.lang.String | El nombre del archivo CSV. |
| splitter | java.lang.String | El divisor |
| convertNumericData | boolean | Si la cadena en el archivo de texto se convierte en datos numéricos. |
| firstRow | int | El número de fila de la primera celda en la que importar. |
| firstColumn | int | El número de columna de la primera celda en la que importar. |

### importCustomObjects(Collection list, int firstRow, int firstColumn, ImportTableOptions options) {#importCustomObjects-java.util.Collection-int-int-com.aspose.cells.ImportTableOptions-}
```
public int importCustomObjects(Collection list, int firstRow, int firstColumn, ImportTableOptions options)
```


Importa objetos personalizados.

**Remarks**

Los objetos personalizados deben ser del mismo tipo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| list | java.util.Collection | El objeto personalizado |
| firstRow | int | El número de fila de la primera celda en la que importar. |
| firstColumn | int | El número de columna de la primera celda en la que importar. |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | Las opciones de importación. |

**Returns:**
int - Número total de filas importadas.
### importCustomObjects(Collection list, String[] propertyNames, boolean isPropertyNameShown, int firstRow, int firstColumn, int rowNumber, boolean insertRows, String dateFormatString, boolean convertStringToNumber) {#importCustomObjects-java.util.Collection-java.lang.String---boolean-int-int-int-boolean-java.lang.String-boolean-}
```
public int importCustomObjects(Collection list, String[] propertyNames, boolean isPropertyNameShown, int firstRow, int firstColumn, int rowNumber, boolean insertRows, String dateFormatString, boolean convertStringToNumber)
```


Importa objetos personalizados.

**Remarks**

Los objetos personalizados deben ser del mismo tipo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| list | java.util.Collection | El objeto personalizado |
| propertyNames | java.lang.String[] | Los nombres de las propiedades. Si es nulo, importaremos todas las propiedades del objeto. |
| isPropertyNameShown | boolean | Indica si el nombre de la propiedad se importará en la primera fila. |
| firstRow | int | El número de fila de la primera celda en la que importar. |
| firstColumn | int | El número de columna de la primera celda en la que importar. |
| rowNumber | int | Número de filas a importar. |
| insertRows | boolean | Indica si se añaden filas extra para ajustar los datos. |
| dateFormatString | java.lang.String | Cadena de formato de fecha para celdas. |
| convertStringToNumber | boolean | Indica si este método intentará convertir la cadena a número. |

**Returns:**
int - Número total de filas importadas.
### importData(ICellsDataTable table, int firstRow, int firstColumn, ImportTableOptions options) {#importData-com.aspose.cells.ICellsDataTable-int-int-com.aspose.cells.ImportTableOptions-}
```
public int importData(ICellsDataTable table, int firstRow, int firstColumn, ImportTableOptions options)
```


Importa datos de una tabla de datos personalizada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| table | [ICellsDataTable](../../com.aspose.cells/icellsdatatable) | La tabla de datos personalizada. |
| firstRow | int | Índice de la primera fila. |
| firstColumn | int | Índice de la primera columna. |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | Las opciones de importación |

**Returns:**
int -
### importFormulaArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical) {#importFormulaArray-java.lang.String---int-int-boolean-}
```
public void importFormulaArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)
```


Importa una matriz de fórmulas a una hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stringArray | java.lang.String[] | Matriz de fórmulas. |
| firstRow | int | El número de fila de la primera celda en la que importar. |
| firstColumn | int | El número de columna de la primera celda en la que importar. |
| isVertical | boolean | Especifica importar datos verticalmente u horizontalmente. |

### importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical) {#importObjectArray-java.lang.Object---int-int-boolean-}
```
public void importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical)
```


Importa una matriz de datos a una hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| objArray | java.lang.Object[] | Matriz de datos. |
| firstRow | int | El número de fila de la primera celda en la que importar. |
| firstColumn | int | El número de columna de la primera celda en la que importar. |
| isVertical | boolean | Especifica importar datos verticalmente u horizontalmente. |

### importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical, int skip) {#importObjectArray-java.lang.Object---int-int-boolean-int-}
```
public void importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical, int skip)
```


Importa una matriz de datos a una hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| objArray | java.lang.Object[] | Matriz de datos. |
| firstRow | int | El número de fila de la primera celda en la que importar. |
| firstColumn | int | El número de columna de la primera celda en la que importar. |
| isVertical | boolean | Especifica importar datos verticalmente u horizontalmente. |
| skip | int | Se omitió el número de filas o columnas. |

### importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-int-int-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown)
```


Importa datos de un objeto ResultSet a la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rs | java.sql.ResultSet | el objeto ResultSet del cual importar. |
| rowIndex | int | índice de fila inicial en la hoja de cálculo. |
| columnIndex | int | índice de columna inicial en la hoja de cálculo. |
| isFieldNameShown | boolean | Indica si el nombre de campo del resultset se importará a la primera fila. |

**Returns:**
int - cuántas filas se importaron realmente.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber) {#importResultSet-java.sql.ResultSet-int-int-boolean-java.lang.String-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)
```


Importa datos de un objeto ResultSet a la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rs | java.sql.ResultSet | el objeto ResultSet del cual importar. |
| rowIndex | int | índice de fila inicial en la hoja de cálculo. |
| columnIndex | int | índice de columna inicial en la hoja de cálculo. |
| isFieldNameShown | boolean | Indica si el nombre de campo del resultset se importará a la primera fila. |
| customDateFormatString | java.lang.String | Cadena de formato de fecha para celdas que contienen valores de fecha. |
| convertStringToNumber | boolean | Indica si este método intentará convertir la cadena a número. |

**Returns:**
int - cuántas filas se importaron realmente.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, ImportTableOptions options) {#importResultSet-java.sql.ResultSet-int-int-com.aspose.cells.ImportTableOptions-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, ImportTableOptions options)
```


Importa datos de un objeto ResultSet a la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rs | java.sql.ResultSet | el objeto ResultSet del cual importar. |
| rowIndex | int | índice de fila inicial en la hoja de cálculo. |
| columnIndex | int | índice de columna inicial en la hoja de cálculo. |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | Las opciones de importación |

**Returns:**
int - cuántas filas se importaron realmente.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown)
```


Importa datos de un objeto ResultSet a la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rs | java.sql.ResultSet | el objeto ResultSet del cual importar. |
| rowIndex | int | índice de fila inicial en la hoja de cálculo. |
| columnIndex | int | índice de columna inicial en la hoja de cálculo. |
| rowNum | int | número de filas a importar. -1 para importar todos los registros del resultset dado. |
| columnNum | int | número de columnas a importar. -1 para importar todas las columnas del resultset dado. |
| isFieldNameShown | boolean | Indica si el nombre de campo del resultset se importará a la primera fila. |

**Returns:**
int - cuántas filas se importaron realmente.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber) {#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-java.lang.String-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)
```


Importa datos de un objeto ResultSet a la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rs | java.sql.ResultSet | el objeto ResultSet del cual importar. |
| rowIndex | int | índice de fila inicial en la hoja de cálculo. |
| columnIndex | int | índice de columna inicial en la hoja de cálculo. |
| rowNum | int | número de filas a importar. -1 para importar todos los registros del resultset dado. |
| columnNum | int | número de columnas a importar. -1 para importar todas las columnas del resultset dado. |
| isFieldNameShown | boolean | Indica si el nombre de campo del resultset se importará a la primera fila. |
| customDateFormatString | java.lang.String | Cadena de formato de fecha para celdas que contienen valores de fecha. |
| convertStringToNumber | boolean | Indica si este método intentará convertir la cadena a número. |

**Returns:**
int - cuántas filas se importaron realmente.
### importResultSet(ResultSet rs, String startCell, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-java.lang.String-boolean-}
```
public int importResultSet(ResultSet rs, String startCell, boolean isFieldNameShown)
```


Importa datos de un objeto ResultSet a la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rs | java.sql.ResultSet | el objeto ResultSet del cual importar. |
| startCell | java.lang.String | nombre de la celda inicial para insertar el resultset, como "A1". |
| isFieldNameShown | boolean | Indica si el nombre de campo del resultset se importará a la primera fila. |

**Returns:**
int - cuántas filas se importaron realmente.
### importResultSet(ResultSet rs, String startCell, ImportTableOptions options) {#importResultSet-java.sql.ResultSet-java.lang.String-com.aspose.cells.ImportTableOptions-}
```
public int importResultSet(ResultSet rs, String startCell, ImportTableOptions options)
```


Importa datos de un objeto ResultSet a la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rs | java.sql.ResultSet | el objeto ResultSet del cual importar. |
| startCell | java.lang.String | nombre de la celda inicial para insertar el resultset, como "A1". |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | Las opciones de importación |

**Returns:**
int - cuántas filas se importaron realmente.
### importResultSet(ResultSet rs, String startCell, int rowNum, int columnNum, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-java.lang.String-int-int-boolean-}
```
public int importResultSet(ResultSet rs, String startCell, int rowNum, int columnNum, boolean isFieldNameShown)
```


Importa datos de un objeto ResultSet a la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rs | java.sql.ResultSet | el objeto ResultSet del cual importar. |
| startCell | java.lang.String | nombre de la celda inicial para insertar el resultset, como "A1". |
| rowNum | int | número de filas a importar. -1 para importar todos los registros del resultset dado. |
| columnNum | int | número de columnas a importar. -1 para importar todas las columnas del resultset dado. |
| isFieldNameShown | boolean | Indica si el nombre de campo del resultset se importará a la primera fila. |

**Returns:**
int - cuántas filas se importaron realmente.
### importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn) {#importTwoDimensionArray-java.lang.Object-----int-int-}
```
public void importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn)
```


Importa una matriz bidimensional de datos a una hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| objArray | java.lang.Object[][] | Matriz de datos bidimensional. |
| firstRow | int | El número de fila de la primera celda en la que importar. |
| firstColumn | int | El número de columna de la primera celda en la que importar. |

### importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn, boolean convertStringToNumber) {#importTwoDimensionArray-java.lang.Object-----int-int-boolean-}
```
public void importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn, boolean convertStringToNumber)
```


Importa una matriz bidimensional de datos a una hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| objArray | java.lang.Object[][] | Matriz de datos bidimensional. |
| firstRow | int | El número de fila de la primera celda en la que importar. |
| firstColumn | int | El número de columna de la primera celda en la que importar. |
| convertStringToNumber | boolean | Indica si este método intentará convertir la cadena a número. |

### importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, boolean convertStringToNumber) {#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-boolean-}
```
public void importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, boolean convertStringToNumber)
```


Importa una matriz bidimensional de datos a una hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| objArray | java.lang.Object[][] | Matriz de datos bidimensional. |
| estilos | java.lang.Object[][] | Estilo de datos bidimensional. |
| firstRow | int | El número de fila de la primera celda en la que importar. |
| firstColumn | int | El número de columna de la primera celda en la que importar. |
| convertStringToNumber | boolean | Indica si este método intentará convertir la cadena a número. |

### importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, TxtLoadOptions opts) {#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-com.aspose.cells.TxtLoadOptions-}
```
public void importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, TxtLoadOptions opts)
```


Importa una matriz bidimensional de datos a una hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| objArray | java.lang.Object[][] | Matriz de datos bidimensional. |
| estilos | java.lang.Object[][] | Estilo de datos bidimensional. |
| firstRow | int | El número de fila de la primera celda en la que importar. |
| firstColumn | int | El número de columna de la primera celda en la que importar. |
| opts | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | Opciones para convertir valores de cadena |

### insertColumn(int columnIndex) {#insertColumn-int-}
```
public void insertColumn(int columnIndex)
```


Inserta una nueva columna en la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | int | Índice de columna. |

### insertColumn(int columnIndex, boolean updateReference) {#insertColumn-int-boolean-}
```
public void insertColumn(int columnIndex, boolean updateReference)
```


Inserta una nueva columna en la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | int | Índice de columna. |
| updateReference | boolean | Indica si las referencias en otras hojas de cálculo se actualizarán. |

### insertColumns(int columnIndex, int totalColumns) {#insertColumns-int-int-}
```
public void insertColumns(int columnIndex, int totalColumns)
```


Inserta varias columnas en la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | int | Índice de columna. |
| totalColumns | int | El número de columnas. |

### insertColumns(int columnIndex, int totalColumns, boolean updateReference) {#insertColumns-int-int-boolean-}
```
public void insertColumns(int columnIndex, int totalColumns, boolean updateReference)
```


Inserta varias columnas en la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | int | Índice de columna. |
| totalColumns | int | El número de columnas. |
| updateReference | boolean | Indica si las referencias en otras hojas de cálculo se actualizarán. |

### insertColumns(int columnIndex, int totalColumns, InsertOptions options) {#insertColumns-int-int-com.aspose.cells.InsertOptions-}
```
public void insertColumns(int columnIndex, int totalColumns, InsertOptions options)
```


Inserta varias columnas en la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | int | Índice de columna. |
| totalColumns | int | El número de columnas. |
| options | [InsertOptions](../../com.aspose.cells/insertoptions) | Las opciones para la operación de inserción. |

### insertCutCells(Range cutRange, int row, int column, int shiftType) {#insertCutCells-com.aspose.cells.Range-int-int-int-}
```
public void insertCutCells(Range cutRange, int row, int column, int shiftType)
```


Insertar rango recortado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cutRange | [Range](../../com.aspose.cells/range) | El rango de corte. |
| fila | int | La fila. |
| columna | int | La columna. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Indica cómo desplazar otros objetos del rango objetivo al insertar el rango recortado. |

### insertRange(CellArea area, int shiftType) {#insertRange-com.aspose.cells.CellArea-int-}
```
public void insertRange(CellArea area, int shiftType)
```


Inserta un rango de celdas y desplaza las celdas según la opción de desplazamiento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| area | [CellArea](../../com.aspose.cells/cellarea) | Desplazar área. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Opción de desplazar celdas. |

### insertRange(CellArea area, int shiftNumber, int shiftType) {#insertRange-com.aspose.cells.CellArea-int-int-}
```
public void insertRange(CellArea area, int shiftNumber, int shiftType)
```


Inserta un rango de celdas y desplaza las celdas según la opción de desplazamiento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| area | [CellArea](../../com.aspose.cells/cellarea) | Desplazar área. |
| shiftNumber | int | Número de filas o columnas a insertar. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Opción de desplazar celdas. |

### insertRange(CellArea area, int shiftNumber, int shiftType, boolean updateReference) {#insertRange-com.aspose.cells.CellArea-int-int-boolean-}
```
public void insertRange(CellArea area, int shiftNumber, int shiftType, boolean updateReference)
```


Inserta un rango de celdas y desplaza las celdas según la opción de desplazamiento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| area | [CellArea](../../com.aspose.cells/cellarea) | Desplazar área. |
| shiftNumber | int | Número de filas o columnas a insertar. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Opción de desplazar celdas. |
| updateReference | boolean | Indica si se actualizan referencias en otras hojas de cálculo. |

### insertRow(int rowIndex) {#insertRow-int-}
```
public void insertRow(int rowIndex)
```


Inserta una nueva fila en la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | int | Índice de fila. |

### insertRows(int rowIndex, int totalRows) {#insertRows-int-int-}
```
public void insertRows(int rowIndex, int totalRows)
```


Inserta varias filas en la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | int | Índice de fila. |
| totalRows | int | Número de filas a insertar. |

### insertRows(int rowIndex, int totalRows, boolean updateReference) {#insertRows-int-int-boolean-}
```
public void insertRows(int rowIndex, int totalRows, boolean updateReference)
```


Inserta varias filas en la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | int | Índice de fila. |
| totalRows | int | Número de filas a insertar. |
| updateReference | boolean | Indica si las referencias en otras hojas de cálculo se actualizarán. |

### insertRows(int rowIndex, int totalRows, InsertOptions options) {#insertRows-int-int-com.aspose.cells.InsertOptions-}
```
public void insertRows(int rowIndex, int totalRows, InsertOptions options)
```


Inserta varias filas en la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | int | Índice de fila. |
| totalRows | int | Número de filas a insertar. |
| options | [InsertOptions](../../com.aspose.cells/insertoptions) | Opciones para la operación de inserción. |

### isBlankColumn(int columnIndex) {#isBlankColumn-int-}
```
public boolean isBlankColumn(int columnIndex)
```


Comprueba si la columna dada está vacía (no contiene datos).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | int | el índice de columna |

**Returns:**
booleano - verdadero si la columna dada no contiene datos
### isColumnHidden(int columnIndex) {#isColumnHidden-int-}
```
public boolean isColumnHidden(int columnIndex)
```


Comprueba si una columna en el índice dado está oculta.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | int | índice de columna |

**Returns:**
booleano - verdadero si la columna está oculta.
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


Indica que la altura de la fila y la altura de fuente predeterminada coinciden

**Returns:**
boolean
### isDefaultRowHidden() {#isDefaultRowHidden--}
```
public boolean isDefaultRowHidden()
```


Indica si la fila está oculta por defecto.

**Returns:**
boolean
### isDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns) {#isDeletingRangeEnabled-int-int-int-int-}
```
public boolean isDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns)
```


Comprueba si el rango puede ser eliminado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | int | El índice de fila inicial del rango. |
| startColumn | int | El índice de columna inicial del rango. |
| totalRows | int | El número de filas en el rango. |
| totalColumns | int | El número de columnas en el rango. |

**Returns:**
boolean -
### isRowHidden(int rowIndex) {#isRowHidden-int-}
```
public boolean isRowHidden(int rowIndex)
```


Comprueba si una fila en el índice dado está oculta.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | int | índice de fila |

**Returns:**
booleano - verdadero si la fila está oculta
### iterator() {#iterator--}
```
public Iterator iterator()
```


Obtiene el enumerador de celdas.

**Remarks**

Al recorrer los elementos mediante el Enumerator devuelto, la colección de celdas no debe modificarse (por ejemplo, operaciones que provoquen la creación de una nueva Cell/Row o la eliminación de una Cell/Row existente). De lo contrario, el enumerador podría no ser capaz de recorrer todas las celdas correctamente (algunos elementos podrían recorrerse repetidamente o omitirse).

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
java.util.Iterator - El enumerador de celdas
### linkToXmlMap(String mapName, int row, int column, String path) {#linkToXmlMap-java.lang.String-int-int-java.lang.String-}
```
public void linkToXmlMap(String mapName, int row, int column, String path)
```


Enlace a un mapa XML.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| mapName | java.lang.String | nombre del mapa xml |
| fila | int | fila de la celda de destino |
| columna | int | columna de la celda de destino |
| ruta | java.lang.String | ruta del elemento xml en el mapa xml |

### merge(int firstRow, int firstColumn, int totalRows, int totalColumns) {#merge-int-int-int-int-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Fusiona un rango especificado de celdas en una sola celda.

**Remarks**

Referencia la celda combinada mediante la dirección de la celda superior izquierda del rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | int | Primera fila de este rango (basado en cero) |
| firstColumn | int | Primera columna de este rango (basado en cero) |
| totalRows | int | Número de filas (basado en uno) |
| totalColumns | int | Número de columnas (basado en uno) |

### merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean mergeConflict) {#merge-int-int-int-int-boolean-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean mergeConflict)
```


Fusiona un rango especificado de celdas en una sola celda.

**Remarks**

Referencia la celda combinada mediante la dirección de la celda superior izquierda en el rango. Si mergeConflict es verdadero y el rango combinado entra en conflicto con otras celdas combinadas, las otras celdas combinadas se eliminarán automáticamente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | int | Primera fila de este rango (basado en cero) |
| firstColumn | int | Primera columna de este rango (basado en cero) |
| totalRows | int | Número de filas (basado en uno) |
| totalColumns | int | Número de columnas (basado en uno) |
| mergeConflict | boolean | Rangos combinados con conflicto de combinación. |

### merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean checkConflict, boolean mergeConflict) {#merge-int-int-int-int-boolean-boolean-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean checkConflict, boolean mergeConflict)
```


Fusiona un rango especificado de celdas en una sola celda.

**Remarks**

Referencia la celda combinada mediante la dirección de la celda superior izquierda en el rango. Si mergeConflict es verdadero y el rango combinado entra en conflicto con otras celdas combinadas, las otras celdas combinadas se eliminarán automáticamente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | int | Primera fila de este rango (basado en cero) |
| firstColumn | int | Primera columna de este rango (basado en cero) |
| totalRows | int | Número de filas (basado en uno) |
| totalColumns | int | Número de columnas (basado en uno) |
| checkConflict | boolean | Indica si se verifica que las celdas combinadas intersectan otras celdas combinadas. |
| mergeConflict | boolean | Rangos combinados con conflicto de combinación. |

### moveRange(CellArea sourceArea, int destRow, int destColumn) {#moveRange-com.aspose.cells.CellArea-int-int-}
```
public void moveRange(CellArea sourceArea, int destRow, int destColumn)
```


Mueve el rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceArea | [CellArea](../../com.aspose.cells/cellarea) | El rango que debe moverse. |
| destRow | int | La fila de destino. |
| destColumn | int | La columna de destino. |

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


Elimina filas duplicadas en la hoja.

### removeDuplicates(int startRow, int startColumn, int endRow, int endColumn) {#removeDuplicates-int-int-int-int-}
```
public void removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)
```


Elimina valores duplicados en el rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | int | La fila inicial. |
| startColumn | int | La columna inicial |
| endRow | int | El índice de fila final. |
| endColumn | int | El índice de columna final. |

### removeDuplicates(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders, int[] columnOffsets) {#removeDuplicates-int-int-int-int-boolean-int---}
```
public void removeDuplicates(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders, int[] columnOffsets)
```


Elimina datos duplicados del rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | int | La fila inicial. |
| startColumn | int | La columna inicial |
| endRow | int | El índice de fila final. |
| endColumn | int | El índice de columna final. |
| hasHeaders | boolean | Indica si el rango contiene encabezados. |
| columnOffsets | int[] | Los desplazamientos de columna. |

### removeFormulas() {#removeFormulas--}
```
public void removeFormulas()
```


Elimina todas las fórmulas y las reemplaza con el valor de la fórmula.

### retrieveSubtotalSetting(CellArea ca) {#retrieveSubtotalSetting-com.aspose.cells.CellArea-}
```
public SubtotalSetting retrieveSubtotalSetting(CellArea ca)
```


Recupera la configuración de subtotales del rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | El rango |

**Returns:**
[SubtotalSetting](../../com.aspose.cells/subtotalsetting) - 
### setColumnWidth(int column, double width) {#setColumnWidth-int-double-}
```
public void setColumnWidth(int column, double width)
```


Establece el ancho de la columna especificada en vista normal.

**Remarks**

Para la hoja de cálculo, el ancho de columna se mide como el número de caracteres del ancho máximo de dígitos de los números 0~9 tal como se renderizan en la fuente del estilo normal.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | Índice de columna. |
| ancho | double | Ancho de columna en unidades de caracteres. El ancho de columna debe estar entre 0 y 255. |

### setColumnWidthInch(int column, double inches) {#setColumnWidthInch-int-double-}
```
public void setColumnWidthInch(int column, double inches)
```


Establece el ancho de la columna en unidades de pulgadas en vista normal.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | Índice de columna. |
| pulgadas | double | Número de pulgadas. |

### setColumnWidthPixel(int column, int pixels) {#setColumnWidthPixel-int-int-}
```
public void setColumnWidthPixel(int column, int pixels)
```


Establece el ancho de la columna en unidades de píxeles en vista normal.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | Índice de columna. |
| píxeles | int | Número de píxeles. |

### setDefaultColumnHidden(boolean value) {#setDefaultColumnHidden-boolean-}
```
public void setDefaultColumnHidden(boolean value)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setDefaultRowHeightMatched(boolean value) {#setDefaultRowHeightMatched-boolean-}
```
public void setDefaultRowHeightMatched(boolean value)
```


Indica que la altura de la fila y la altura de fuente predeterminada coinciden

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setDefaultRowHidden(boolean value) {#setDefaultRowHidden-boolean-}
```
public void setDefaultRowHidden(boolean value)
```


Indica si la fila está oculta por defecto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


Establece la opción de uso de memoria para estas celdas.

Ver [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Límites notables y operaciones recomendadas para algunos modos:

| Modo | Observaciones | Compatible |
| ------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
| [MemorySetting.MEMORY\_PREFERENCE](../../com.aspose.cells/memorysetting\#MEMORY-PREFERENCE) | Cells data will be maintained in compact format to decrease the memory cost. On other hand, the compact data also may cause higher time cost, especially when updating the cells data, or accessing cells/rows randomly | v8.0.0 |
|  | [MemorySetting.FILE\_CACHE](../../com.aspose.cells/memorysetting\#FILE-CACHE) | Cuando se usa este modo para cualquier hoja de cálculo en un libro, se debe llamar a [Workbook.dispose()](../../com.aspose.cells/workbook\#dispose--) al final del trabajo para liberar todos los recursos, como los archivos temporales. |
 
Acceder a celdas de forma aleatoria producirá un bajo rendimiento porque los datos deben leerse/actualizarse de forma aleatoria y repetida (por lo que el puntero en el archivo se cambiará en consecuencia y se requerirán operaciones de E/S repetidamente). Si es posible, acceda siempre a los datos de forma secuencial (fila por fila).
 
Cuando se modifica el dato de una fila/celda, los datos de otras celdas/filas también pueden verse afectados (por ejemplo, los datos pueden desplazarse/moverse a otros lugares para asignar suficiente espacio al dato modificado). Por lo tanto, cada cambio de cualquier dato requiere la sincronización de otros objetos existentes (como objetos Row o Cell). Así, para obtener un mejor rendimiento, no mantenga múltiples Rows/Cells al mismo tiempo. Procesarlos uno por uno reducirá la sincronización de datos y mejorará un poco el rendimiento. | v25.7     |

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMultiThreadReading(boolean value) {#setMultiThreadReading-boolean-}
```
public void setMultiThreadReading(boolean value)
```


Establece si el modelo de datos de las celdas debe soportar lectura Multi-Thread. El valor predeterminado de esta propiedad es false.

**Remarks**

Si hay varios hilos leyendo objetos Row/Cell en esta colección de forma concurrente, esta propiedad debe establecerse en true; de lo contrario, pueden producirse resultados inesperados. Soportar la lectura Multi-Thread puede degradar el rendimiento al acceder a objetos Row/Cell de esta colección. Tenga en cuenta que algunas funciones no pueden soportar la lectura Multi-Thread, como el formato de valores (por ejemplo, [Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--), [Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), etc.). Por lo tanto, incluso con esta propiedad establecida en true, esas API aún pueden dar resultados inesperados al leer en modo Multi-Thread.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setPreserveString(boolean value) {#setPreserveString-boolean-}
```
public void setPreserveString(boolean value)
```


Establece un valor que indica si todos los valores de la hoja de cálculo se conservan como cadenas. El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setRowHeight(int row, double height) {#setRowHeight-int-double-}
```
public void setRowHeight(int row, double height)
```


Establece la altura de la fila especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila. |
| altura | double | Altura de fila. En unidades de punto. Debe estar entre 0 y 409.5. |

### setRowHeightInch(int row, double inches) {#setRowHeightInch-int-double-}
```
public void setRowHeightInch(int row, double inches)
```


Establece la altura de la fila en unidades de pulgadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila. |
| pulgadas | double | Número de pulgadas. Debe estar entre 0 y 409.5/72. |

### setRowHeightPixel(int row, int pixels) {#setRowHeightPixel-int-int-}
```
public void setRowHeightPixel(int row, int pixels)
```


Establece la altura de la fila en unidades de píxeles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila. |
| píxeles | int | Número de píxeles. |

### setStandardHeight(double value) {#setStandardHeight-double-}
```
public void setStandardHeight(double value)
```


Establece la altura predeterminada de la fila en esta hoja de cálculo, en unidades de puntos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setStandardHeightInch(double value) {#setStandardHeightInch-double-}
```
public void setStandardHeightInch(double value)
```


Establece la altura predeterminada de la fila en esta hoja de cálculo, en unidades de pulgadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setStandardHeightPixels(int value) {#setStandardHeightPixels-int-}
```
public void setStandardHeightPixels(int value)
```


Establece la altura predeterminada de la fila en esta hoja de cálculo, en unidades de píxeles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setStandardWidth(double value) {#setStandardWidth-double-}
```
public void setStandardWidth(double value)
```


Establece el ancho predeterminado de la columna en la hoja de cálculo, en unidades de caracteres.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setStandardWidthInch(double value) {#setStandardWidthInch-double-}
```
public void setStandardWidthInch(double value)
```


Establece el ancho predeterminado de la columna en la hoja de cálculo, en unidades de pulgadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setStandardWidthPixels(int value) {#setStandardWidthPixels-int-}
```
public void setStandardWidthPixels(int value)
```


Establece el ancho predeterminado de la columna en la hoja de cálculo, en unidades de píxeles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setStyle(Style value) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style value)
```


Establece el estilo predeterminado de la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setViewColumnWidthPixel(int column, int pixels) {#setViewColumnWidthPixel-int-int-}
```
public void setViewColumnWidthPixel(int column, int pixels)
```


Establece el ancho de la columna en diferentes vistas.

**Remarks**

Si el tipo de vista actual es [ViewType.PAGE\_LAYOUT\_VIEW](../../com.aspose.cells/viewtype\#PAGE-LAYOUT-VIEW), el ancho de la columna es el mismo que el ancho impreso.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | El índice de columna. |
| píxeles | int | El ancho en unidades de píxeles. |

### showGroupDetail(boolean isVertical, int index) {#showGroupDetail-boolean-int-}
```
public void showGroupDetail(boolean isVertical, int index)
```


Expande las filas/columnas agrupadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isVertical | boolean | Verdadero, expande las filas agrupadas. |
| índice | int | El índice de fila/columna |

### subtotal(CellArea ca, int groupBy, int function, int[] totalList) {#subtotal-com.aspose.cells.CellArea-int-int-int---}
```
public void subtotal(CellArea ca, int groupBy, int function, int[] totalList)
```


Crea subtotales para el rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | El rango |
| groupBy | int | El campo por el cual agrupar, como un desplazamiento entero basado en cero |
| function | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). La función de subtotal. |
| totalList | int[] | Una matriz de desplazamientos de campo basados en cero, que indica los campos a los que se añaden los subtotales. |

### subtotal(CellArea ca, int groupBy, int function, int[] totalList, boolean replace, boolean pageBreaks, boolean summaryBelowData) {#subtotal-com.aspose.cells.CellArea-int-int-int---boolean-boolean-boolean-}
```
public void subtotal(CellArea ca, int groupBy, int function, int[] totalList, boolean replace, boolean pageBreaks, boolean summaryBelowData)
```


Crea subtotales para el rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | El rango |
| groupBy | int | El campo por el cual agrupar, como un desplazamiento entero basado en cero |
| function | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). La función de subtotal. |
| totalList | int[] | Una matriz de desplazamientos de campo basados en cero, que indica los campos a los que se añaden los subtotales. |
| replace | boolean | Indica si reemplaza los subtotales actuales |
| pageBreaks | boolean | Indica si se agrega un salto de página entre los grupos |
| summaryBelowData | boolean | Indica si se agrega un resumen debajo de los datos. |

### textToColumns(int row, int column, int totalRows, TxtLoadOptions options) {#textToColumns-int-int-int-com.aspose.cells.TxtLoadOptions-}
```
public int textToColumns(int row, int column, int totalRows, TxtLoadOptions options)
```


Divide el contenido en la columna especificada en múltiples columnas..

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | El índice de fila. |
| columna | int | El índice de columna. |
| totalRows | int | El número de filas. |
| options | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | Las opciones de división. |

**Returns:**
int - Recuento total de columnas de los valores divididos.
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


Descombina un rango especificado de celdas combinadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | int | Primera fila de este rango (basado en cero) |
| firstColumn | int | Primera columna de este rango (basado en cero) |
| totalRows | int | Número de filas (basado en uno) |
| totalColumns | int | Número de columnas (basado en uno) |

### ungroupColumns(int firstIndex, int lastIndex) {#ungroupColumns-int-int-}
```
public void ungroupColumns(int firstIndex, int lastIndex)
```


Desagrupa columnas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstIndex | int | El índice de la primera columna a desagrupar. |
| lastIndex | int | El índice de la última columna a desagrupar. |

### ungroupRows(int firstIndex, int lastIndex) {#ungroupRows-int-int-}
```
public void ungroupRows(int firstIndex, int lastIndex)
```


Desagrupa filas.

**Remarks**

Solo elimina la información del grupo externo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstIndex | int | El índice de la primera fila a desagrupar. |
| lastIndex | int | El índice de la última fila a desagrupar. |

### ungroupRows(int firstIndex, int lastIndex, boolean isAll) {#ungroupRows-int-int-boolean-}
```
public void ungroupRows(int firstIndex, int lastIndex, boolean isAll)
```


Desagrupa filas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstIndex | int | El índice de la primera fila a desagrupar. |
| lastIndex | int | El índice de la última fila a desagrupar. |
| isAll | boolean | Verdadero, elimina toda la información agrupada. De lo contrario, elimina la información del grupo externo. |

### unhideColumn(int column, double width) {#unhideColumn-int-double-}
```
public void unhideColumn(int column, double width)
```


Desoculta una columna

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | Índice de columna. |
| ancho | double | Ancho de columna. |

### unhideColumns(int column, int totalColumns, double width) {#unhideColumns-int-int-double-}
```
public void unhideColumns(int column, int totalColumns, double width)
```


Desoculta varias columnas.

**Remarks**

Solo aplica el ancho de columna a las columnas ocultas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | Índice de columna. |
| totalColumns | int | Número de columna |
| ancho | double | Ancho de columna. |

### unhideRow(int row, double height) {#unhideRow-int-double-}
```
public void unhideRow(int row, double height)
```


Desoculta una fila.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila. |
| altura | double | Altura de fila. La altura de la fila solo se cambiará cuando la fila esté oculta y el valor de altura proporcionado sea positivo. |

### unhideRows(int row, int totalRows, double height) {#unhideRows-int-int-double-}
```
public void unhideRows(int row, int totalRows, double height)
```


Desoculta las filas ocultas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | El índice de fila. |
| totalRows | int | El número de fila. |
| altura | double | Altura de fila. La altura de la fila solo se cambiará cuando la fila esté oculta y el valor de altura proporcionado sea positivo. |

### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

