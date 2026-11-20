---
title: "Cells"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula una raccolta di oggetti pertinenti alle celle, come   ...etc."
type: docs
url: /it/java/com.aspose.cells/cells/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Cells implements Iterable
```

Incapsula una raccolta di oggetti pertinenti alle celle, come [Cell](../../com.aspose.cells/cell), [Row](../../com.aspose.cells/row), ...etc.

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
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addRange(Range rangeObject)](#addRange-com.aspose.cells.Range-) | Aggiunge un riferimento a un oggetto intervallo alle celle |
| [applyColumnStyle(int column, Style style, StyleFlag flag)](#applyColumnStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Applica formati a un'intera colonna. |
| [applyRowStyle(int row, Style style, StyleFlag flag)](#applyRowStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Applica formati per un'intera riga. |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Applica formati a un intero foglio di lavoro. |
| [checkCell(int row, int column)](#checkCell-int-int-) | Restituisce l'elemento [Cell](../../com.aspose.cells/cell) o null all'indice di riga e colonna della cella specificati. |
| [checkColumn(int columnIndex)](#checkColumn-int-) | Restituisce l'elemento [Column](../../com.aspose.cells/column) o null all'indice di colonna specificato. |
| [checkRow(int row)](#checkRow-int-) | Restituisce l'elemento [Row](../../com.aspose.cells/row) o null all'indice di riga della cella specificato. |
| [clear()](#clear--) | Cancella tutti i dati del foglio di lavoro. |
| [clearContents(CellArea range)](#clearContents-com.aspose.cells.CellArea-) | Cancella il contenuto di un intervallo. |
| [clearContents(int startRow, int startColumn, int endRow, int endColumn)](#clearContents-int-int-int-int-) | Cancella il contenuto di un intervallo. |
| [clearFormats(CellArea range)](#clearFormats-com.aspose.cells.CellArea-) | Cancella la formattazione di un intervallo. |
| [clearFormats(int startRow, int startColumn, int endRow, int endColumn)](#clearFormats-int-int-int-int-) | Cancella la formattazione di un intervallo. |
| [clearMergedCells()](#clearMergedCells--) | Cancella tutti gli intervalli uniti. |
| [clearRange(CellArea range)](#clearRange-com.aspose.cells.CellArea-) | Cancella il contenuto e la formattazione di un intervallo. |
| [clearRange(int startRow, int startColumn, int endRow, int endColumn)](#clearRange-int-int-int-int-) | Cancella il contenuto e la formattazione di un intervallo. |
| [convertStringToNumericValue()](#convertStringToNumericValue--) | Converte tutti i dati stringa nel foglio di lavoro in valori numerici, se possibile. |
| [copyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex)](#copyColumn-com.aspose.cells.Cells-int-int-) | Copia dati e formati di un'intera colonna. |
| [copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)](#copyColumns-com.aspose.cells.Cells-int-int-int-) | Copia i dati e i formati di intere colonne. |
| [copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber, PasteOptions pasteOptions)](#copyColumns-com.aspose.cells.Cells-int-int-int-com.aspose.cells.PasteOptions-) | Copia dati e formati di un'intera colonna. |
| [copyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, int destinationColumnIndex, int destinationTotalColumns)](#copyColumns-com.aspose.cells.Cells-int-int-int-int-) | Copia i dati e i formati di tutte le colonne. |
| [copyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex)](#copyRow-com.aspose.cells.Cells-int-int-) | Copia i dati e i formati di un'intera riga. |
| [copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)](#copyRows-com.aspose.cells.Cells-int-int-int-) | Copia i dati e i formati di alcune intere righe. |
| [copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions)](#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-) | Copia i dati e i formati di alcune intere righe. |
| [copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)](#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-com.aspose.cells.PasteOptions-) | Copia i dati e i formati di alcune intere righe. |
| [createRange(int firstIndex, int number, boolean isVertical)](#createRange-int-int-boolean-) | Crea un oggetto [Range](../../com.aspose.cells/range) da righe di celle o colonne di celle. |
| [createRange(int firstRow, int firstColumn, int totalRows, int totalColumns)](#createRange-int-int-int-int-) | Crea un oggetto [Range](../../com.aspose.cells/range) da un intervallo di celle. |
| [createRange(String address)](#createRange-java.lang.String-) | Crea un oggetto [Range](../../com.aspose.cells/range) da un indirizzo dell'intervallo. |
| [createRange(String upperLeftCell, String lowerRightCell)](#createRange-java.lang.String-java.lang.String-) | Crea un oggetto [Range](../../com.aspose.cells/range) da un intervallo di celle. |
| [deleteBlankColumns()](#deleteBlankColumns--) | Elimina tutte le colonne vuote che non contengono alcun dato. |
| [deleteBlankColumns(DeleteOptions options)](#deleteBlankColumns-com.aspose.cells.DeleteOptions-) | Elimina tutte le colonne vuote che non contengono alcun dato. |
| [deleteBlankRows()](#deleteBlankRows--) | Elimina tutte le righe vuote che non contengono alcun dato o altro oggetto. |
| [deleteBlankRows(DeleteOptions options)](#deleteBlankRows-com.aspose.cells.DeleteOptions-) | Elimina tutte le righe vuote che non contengono alcun dato o alcuni oggetti speciali come commenti visibili, tabelle pivot. |
| [deleteColumn(int columnIndex)](#deleteColumn-int-) | Elimina una colonna. |
| [deleteColumn(int columnIndex, boolean updateReference)](#deleteColumn-int-boolean-) | Elimina una colonna. |
| [deleteColumns(int columnIndex, int totalColumns, boolean updateReference)](#deleteColumns-int-int-boolean-) | Elimina diverse colonne. |
| [deleteColumns(int columnIndex, int totalColumns, DeleteOptions options)](#deleteColumns-int-int-com.aspose.cells.DeleteOptions-) | Elimina diverse colonne. |
| [deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)](#deleteRange-int-int-int-int-int-) | Elimina un intervallo di celle e sposta le celle secondo l'opzione di spostamento. |
| [deleteRow(int rowIndex)](#deleteRow-int-) | Elimina una riga. |
| [deleteRow(int rowIndex, boolean updateReference)](#deleteRow-int-boolean-) | Elimina una riga. |
| [deleteRows(int rowIndex, int totalRows)](#deleteRows-int-int-) | Elimina più righe. |
| [deleteRows(int rowIndex, int totalRows, boolean updateReference)](#deleteRows-int-int-boolean-) | Elimina più righe nel foglio di lavoro. |
| [deleteRows(int rowIndex, int totalRows, DeleteOptions options)](#deleteRows-int-int-com.aspose.cells.DeleteOptions-) | Elimina più righe nel foglio di lavoro. |
| [dispose()](#dispose--) | Esegue attività definite dall'applicazione associate al rilascio, alla liberazione o al ripristino di risorse non gestite. |
| [endCellInColumn(int columnIndex)](#endCellInColumn-int-) | Ottiene l'ultima cella in questa colonna. |
| [endCellInColumn(int startRow, int endRow, int startColumn, int endColumn)](#endCellInColumn-int-int-int-int-) | Ottiene l'ultima cella con indice di colonna massimo in questo intervallo. |
| [endCellInRow(int rowIndex)](#endCellInRow-int-) | Ottiene l'ultima cella in questa riga. |
| [endCellInRow(int startRow, int endRow, int startColumn, int endColumn)](#endCellInRow-int-int-int-int-) | Ottiene l'ultima cella con indice di riga massimo in questo intervallo. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)](#exportArray-int-int-int-int-) | Esporta i dati nella collezione [Cells](../../com.aspose.cells/cells) in un oggetto array bidimensionale. |
| [exportTypeArray(int firstRow, int firstColumn, int totalRows, int totalColumns)](#exportTypeArray-int-int-int-int-) | Esporta il tipo di valore della cella nella collezione [Cells](../../com.aspose.cells/cells) in un oggetto array bidimensionale. |
| [find(Object what, Cell previousCell)](#find-java.lang.Object-com.aspose.cells.Cell-) | Trova la cella contenente l'oggetto di input. |
| [find(Object what, Cell previousCell, FindOptions findOptions)](#find-java.lang.Object-com.aspose.cells.Cell-com.aspose.cells.FindOptions-) | Trova la cella contenente l'oggetto di input. |
| [get(int row, int column)](#get-int-int-) | Ottiene l'elemento [Cell](../../com.aspose.cells/cell) all'indice di riga e colonna della cella specificati. |
| [get(String cellName)](#get-java.lang.String-) | Ottiene l'elemento [Cell](../../com.aspose.cells/cell) al nome della cella specificato. |
| [getCellDisplayStyle(int row, int column)](#getCellDisplayStyle-int-int-) | Ottieni lo stile di visualizzazione della cella fornita. |
| [getCellDisplayStyle(int row, int column, int adjacentBorders)](#getCellDisplayStyle-int-int-int-) | Ottieni lo stile di visualizzazione della cella fornita. |
| [getCellStyle(int row, int column)](#getCellStyle-int-int-) | Ottieni lo stile della cella fornita. |
| [getCellsWithPlaceInCellPicture()](#getCellsWithPlaceInCellPicture--) | Ottiene tutte le celle che contengono un'immagine incorporata. |
| [getClass()](#getClass--) |  |
| [getColumnOriginalWidthPoint(int column)](#getColumnOriginalWidthPoint-int-) | Ottiene l'altezza originale della colonna in unità di punto se la colonna è nascosta. |
| [getColumnWidth(int column)](#getColumnWidth-int-) | Ottiene la larghezza (in unità di caratteri) della colonna specificata nella visualizzazione normale. |
| [getColumnWidth(int column, boolean isOriginal, int unitType)](#getColumnWidth-int-boolean-int-) | Ottiene la larghezza della colonna. |
| [getColumnWidthInch(int column)](#getColumnWidthInch-int-) | Ottiene la larghezza della colonna specificata nella visualizzazione normale, in unità di pollici. |
| [getColumnWidthPixel(int column)](#getColumnWidthPixel-int-) | Ottiene la larghezza della colonna specificata nella visualizzazione normale, in unità di pixel. |
| [getColumnWidthPixel(int column, boolean original)](#getColumnWidthPixel-int-boolean-) | Ottiene la larghezza della colonna specificata nella visualizzazione normale, in unità di pixel. |
| [getColumns()](#getColumns--) | Ottiene la raccolta di oggetti [Column](../../com.aspose.cells/column) che rappresentano le singole colonne in questo foglio di lavoro. |
| [getCount()](#getCount--) | Ottiene il conteggio totale degli oggetti Cell istanziati. |
| [getCountLarge()](#getCountLarge--) | Ottiene il conteggio totale degli oggetti Cell istanziati. |
| [getDependents(boolean isAll, int row, int column)](#getDependents-boolean-int-int-) | Ottieni tutte le celle che fanno riferimento alla cella specifica. |
| [getDependentsInCalculation(int row, int column, boolean recursive)](#getDependentsInCalculation-int-int-boolean-) | Ottiene tutte le celle il cui risultato calcolato dipende dalla cella specifica. |
| [getFirstCell()](#getFirstCell--) | Ottiene la prima cella in questo foglio di lavoro. |
| [getFirstDataRow(int column)](#getFirstDataRow-int-) | Ottiene l'indice della prima riga della cella che contiene dati nella colonna specificata. |
| [getGroupedColumnOutlineLevel(int columnIndex)](#getGroupedColumnOutlineLevel-int-) | Ottiene il livello di contorno (basato su zero) della colonna. |
| [getGroupedRowOutlineLevel(int rowIndex)](#getGroupedRowOutlineLevel-int-) | Ottiene il livello di contorno (basato su zero) della riga. |
| [getLastCell()](#getLastCell--) | Ottiene l'ultima cella in questo foglio di lavoro. |
| [getLastDataRow(int column)](#getLastDataRow-int-) | Ottiene l'indice dell'ultima riga della cella che contiene dati nella colonna specificata. |
| [getMaxColumn()](#getMaxColumn--) | Indice massimo della colonna di quelle celle che sono state istanziate nella raccolta (non include la colonna in cui lo stile è definito per l'intera colonna ma nessuna cella è stata istanziata). |
| [getMaxDataColumn()](#getMaxDataColumn--) | Indice massimo della colonna della cella che contiene dati. |
| [getMaxDataRow()](#getMaxDataRow--) | Indice massimo della riga della cella che contiene dati. |
| [getMaxDisplayRange()](#getMaxDisplayRange--) | Ottiene l'intervallo massimo che include dati, celle unite e forme. |
| [getMaxGroupedColumnOutlineLevel()](#getMaxGroupedColumnOutlineLevel--) | Ottiene il livello di contorno della colonna raggruppata massima (basato su zero). |
| [getMaxGroupedRowOutlineLevel()](#getMaxGroupedRowOutlineLevel--) | Ottiene il livello di contorno della riga raggruppata massima (basato su zero). |
| [getMaxRow()](#getMaxRow--) | Indice massimo della riga della cella che contiene dati o stile. |
| [getMemorySetting()](#getMemorySetting--) | Ottiene l'opzione di utilizzo della memoria per queste celle. |
| [getMergedAreas()](#getMergedAreas--) | Ottiene tutte le celle unite. |
| [getMergedCells()](#getMergedCells--) | Ottiene la raccolta delle celle unite. |
| [getMinColumn()](#getMinColumn--) | Indice minimo di colonna di quelle celle che sono state istanziate nella raccolta (non include la colonna in cui lo stile è definito per l'intera colonna ma non è stata istanziata alcuna cella). |
| [getMinDataColumn()](#getMinDataColumn--) | Indice minimo di colonna della cella che contiene dati. |
| [getMinDataRow()](#getMinDataRow--) | Indice minimo di riga della cella che contiene dati. |
| [getMinRow()](#getMinRow--) | Indice minimo di riga della cella che contiene dati o stile. |
| [getMultiThreadReading()](#getMultiThreadReading--) | Ottiene se il modello dati delle celle deve supportare la lettura multi-thread. |
| [getOdsCellFields()](#getOdsCellFields--) | Ottiene l'elenco dei campi di ods. |
| [getPreserveString()](#getPreserveString--) | Ottiene un valore che indica se tutti i valori del foglio di lavoro sono conservati come stringhe. |
| [getRanges()](#getRanges--) | Ottiene la raccolta degli oggetti [Range](../../com.aspose.cells/range) creati a runtime. |
| [getRowEnumerator()](#getRowEnumerator--) | Ottiene l'enumeratore delle righe. |
| [getRowHeight(int row)](#getRowHeight-int-) | Ottiene l'altezza di una riga specificata, in unità di punti. |
| [getRowHeight(int row, boolean isOriginal, int unitType)](#getRowHeight-int-boolean-int-) | Ottiene l'altezza della riga. |
| [getRowHeightInch(int row)](#getRowHeightInch-int-) | Ottiene l'altezza di una riga specificata in unità di pollici. |
| [getRowHeightPixel(int row)](#getRowHeightPixel-int-) | Ottiene l'altezza di una riga specificata in unità di pixel. |
| [getRowOriginalHeightPoint(int row)](#getRowOriginalHeightPoint-int-) | Ottiene l'altezza originale della riga in unità di punti se la riga è nascosta |
| [getRows()](#getRows--) | Ottiene la raccolta degli oggetti [Row](../../com.aspose.cells/row) che rappresentano le singole righe in questo foglio di lavoro. |
| [getStandardHeight()](#getStandardHeight--) | Ottiene l'altezza predefinita delle righe in questo foglio di lavoro, in unità di punti. |
| [getStandardHeightInch()](#getStandardHeightInch--) | Ottiene l'altezza predefintta delle righe in questo foglio di lavoro, in unità di pollici. |
| [getStandardHeightPixels()](#getStandardHeightPixels--) | Ottiene l'altezza predefinita delle righe in questo foglio di lavoro, in unità di pixel. |
| [getStandardWidth()](#getStandardWidth--) | Ottiene la larghezza predefinita delle colonne nel foglio di lavoro, in unità di caratteri. |
| [getStandardWidthInch()](#getStandardWidthInch--) | Ottiene la larghezza predefinita delle colonne nel foglio di lavoro, in unità di pollici. |
| [getStandardWidthPixels()](#getStandardWidthPixels--) | Ottiene la larghezza predefinita delle colonne nel foglio di lavoro, in unità di pixel. |
| [getStyle()](#getStyle--) | Ottiene lo stile predefinito del foglio di lavoro. |
| [getViewColumnWidthPixel(int column)](#getViewColumnWidthPixel-int-) | Ottieni la larghezza in diversi tipi di visualizzazione. |
| [getViewRowHeight(int row)](#getViewRowHeight-int-) | Ottiene l'altezza di una riga specificata. |
| [getViewRowHeightInch(int row)](#getViewRowHeightInch-int-) | Ottiene l'altezza di una riga specificata in unità di pollici. |
| [groupColumns(int firstIndex, int lastIndex)](#groupColumns-int-int-) | Raggruppa le colonne. |
| [groupColumns(int firstIndex, int lastIndex, boolean isHidden)](#groupColumns-int-int-boolean-) | Raggruppa le colonne. |
| [groupRows(int firstIndex, int lastIndex)](#groupRows-int-int-) | Raggruppa le righe. |
| [groupRows(int firstIndex, int lastIndex, boolean isHidden)](#groupRows-int-int-boolean-) | Raggruppa le righe. |
| [hashCode()](#hashCode--) |  |
| [hideColumn(int column)](#hideColumn-int-) | Nasconde una colonna. |
| [hideColumns(int column, int totalColumns)](#hideColumns-int-int-) | Nascondi più colonne. |
| [hideGroupDetail(boolean isVertical, int index)](#hideGroupDetail-boolean-int-) | Comprimi le righe/colonne raggruppate. |
| [hideRow(int row)](#hideRow-int-) | Nasconde una riga. |
| [hideRows(int row, int totalRows)](#hideRows-int-int-) | Nasconde più righe. |
| [importArray(double[] doubleArray, int firstRow, int firstColumn, boolean isVertical)](#importArray-double---int-int-boolean-) | Importa un array di double in un foglio di lavoro. |
| [importArray(double[][] doubleArray, int firstRow, int firstColumn)](#importArray-double-----int-int-) | Importa un array bidimensionale di double in un foglio di lavoro. |
| [importArray(int[] intArray, int firstRow, int firstColumn, boolean isVertical)](#importArray-int---int-int-boolean-) | Importa un array di integer in un foglio di lavoro. |
| [importArray(int[][] intArray, int firstRow, int firstColumn)](#importArray-int-----int-int-) | Importa un array bidimensionale di integer in un foglio di lavoro. |
| [importArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)](#importArray-java.lang.String---int-int-boolean-) | Importa un array di string in un foglio di lavoro. |
| [importArray(String[][] stringArray, int firstRow, int firstColumn)](#importArray-java.lang.String-----int-int-) | Importa un array bidimensionale di string in un foglio di lavoro. |
| [importArrayList(ArrayList arrayList, int firstRow, int firstColumn, boolean isVertical)](#importArrayList-java.util.ArrayList-int-int-boolean-) | Importa un arraylist di dati in un foglio di lavoro. |
| [importCSV(InputStream stream, TxtLoadOptions options, int firstRow, int firstColumn)](#importCSV-java.io.InputStream-com.aspose.cells.TxtLoadOptions-int-int-) | Importa un file CSV nelle celle. |
| [importCSV(InputStream stream, String splitter, boolean convertNumericData, int firstRow, int firstColumn)](#importCSV-java.io.InputStream-java.lang.String-boolean-int-int-) | Importa un file CSV nelle celle. |
| [importCSV(String fileName, TxtLoadOptions options, int firstRow, int firstColumn)](#importCSV-java.lang.String-com.aspose.cells.TxtLoadOptions-int-int-) | Importa un file CSV nelle celle. |
| [importCSV(String fileName, String splitter, boolean convertNumericData, int firstRow, int firstColumn)](#importCSV-java.lang.String-java.lang.String-boolean-int-int-) | Importa un file CSV nelle celle. |
| [importCustomObjects(Collection list, int firstRow, int firstColumn, ImportTableOptions options)](#importCustomObjects-java.util.Collection-int-int-com.aspose.cells.ImportTableOptions-) | Importa oggetti personalizzati. |
| [importCustomObjects(Collection list, String[] propertyNames, boolean isPropertyNameShown, int firstRow, int firstColumn, int rowNumber, boolean insertRows, String dateFormatString, boolean convertStringToNumber)](#importCustomObjects-java.util.Collection-java.lang.String---boolean-int-int-int-boolean-java.lang.String-boolean-) | Importa oggetti personalizzati. |
| [importData(ICellsDataTable table, int firstRow, int firstColumn, ImportTableOptions options)](#importData-com.aspose.cells.ICellsDataTable-int-int-com.aspose.cells.ImportTableOptions-) | Importa dati da una tabella dati personalizzata. |
| [importFormulaArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)](#importFormulaArray-java.lang.String---int-int-boolean-) | Importa un array di formula in un foglio di lavoro. |
| [importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical)](#importObjectArray-java.lang.Object---int-int-boolean-) | Importa un array di dati in un foglio di lavoro. |
| [importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical, int skip)](#importObjectArray-java.lang.Object---int-int-boolean-int-) | Importa un array di dati in un foglio di lavoro. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-int-int-boolean-) | Importa dati da un oggetto ResultSet nel foglio di lavoro. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)](#importResultSet-java.sql.ResultSet-int-int-boolean-java.lang.String-boolean-) | Importa dati da un oggetto ResultSet nel foglio di lavoro. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, ImportTableOptions options)](#importResultSet-java.sql.ResultSet-int-int-com.aspose.cells.ImportTableOptions-) | Importa dati da un oggetto ResultSet nel foglio di lavoro. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-) | Importa dati da un oggetto ResultSet nel foglio di lavoro. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)](#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-java.lang.String-boolean-) | Importa dati da un oggetto ResultSet nel foglio di lavoro. |
| [importResultSet(ResultSet rs, String startCell, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-java.lang.String-boolean-) | Importa dati da un oggetto ResultSet nel foglio di lavoro. |
| [importResultSet(ResultSet rs, String startCell, ImportTableOptions options)](#importResultSet-java.sql.ResultSet-java.lang.String-com.aspose.cells.ImportTableOptions-) | Importa dati da un oggetto ResultSet nel foglio di lavoro. |
| [importResultSet(ResultSet rs, String startCell, int rowNum, int columnNum, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-java.lang.String-int-int-boolean-) | Importa dati da un oggetto ResultSet nel foglio di lavoro. |
| [importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn)](#importTwoDimensionArray-java.lang.Object-----int-int-) | Importa un array bidimensionale di dati in un foglio di lavoro. |
| [importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn, boolean convertStringToNumber)](#importTwoDimensionArray-java.lang.Object-----int-int-boolean-) | Importa un array bidimensionale di dati in un foglio di lavoro. |
| [importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, boolean convertStringToNumber)](#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-boolean-) | Importa un array bidimensionale di dati in un foglio di lavoro. |
| [importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, TxtLoadOptions opts)](#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-com.aspose.cells.TxtLoadOptions-) | Importa un array bidimensionale di dati in un foglio di lavoro. |
| [insertColumn(int columnIndex)](#insertColumn-int-) | Inserisce una nuova colonna nel foglio di lavoro. |
| [insertColumn(int columnIndex, boolean updateReference)](#insertColumn-int-boolean-) | Inserisce una nuova colonna nel foglio di lavoro. |
| [insertColumns(int columnIndex, int totalColumns)](#insertColumns-int-int-) | Inserisce alcune colonne nel foglio di lavoro. |
| [insertColumns(int columnIndex, int totalColumns, boolean updateReference)](#insertColumns-int-int-boolean-) | Inserisce alcune colonne nel foglio di lavoro. |
| [insertColumns(int columnIndex, int totalColumns, InsertOptions options)](#insertColumns-int-int-com.aspose.cells.InsertOptions-) | Inserisce alcune colonne nel foglio di lavoro. |
| [insertCutCells(Range cutRange, int row, int column, int shiftType)](#insertCutCells-com.aspose.cells.Range-int-int-int-) | Inserisci intervallo tagliato. |
| [insertRange(CellArea area, int shiftType)](#insertRange-com.aspose.cells.CellArea-int-) | Inserisce un intervallo di celle e sposta le celle in base all'opzione di spostamento. |
| [insertRange(CellArea area, int shiftNumber, int shiftType)](#insertRange-com.aspose.cells.CellArea-int-int-) | Inserisce un intervallo di celle e sposta le celle in base all'opzione di spostamento. |
| [insertRange(CellArea area, int shiftNumber, int shiftType, boolean updateReference)](#insertRange-com.aspose.cells.CellArea-int-int-boolean-) | Inserisce un intervallo di celle e sposta le celle in base all'opzione di spostamento. |
| [insertRow(int rowIndex)](#insertRow-int-) | Inserisce una nuova riga nel foglio di lavoro. |
| [insertRows(int rowIndex, int totalRows)](#insertRows-int-int-) | Inserisce più righe nel foglio di lavoro. |
| [insertRows(int rowIndex, int totalRows, boolean updateReference)](#insertRows-int-int-boolean-) | Inserisce più righe nel foglio di lavoro. |
| [insertRows(int rowIndex, int totalRows, InsertOptions options)](#insertRows-int-int-com.aspose.cells.InsertOptions-) | Inserisce più righe nel foglio di lavoro. |
| [isBlankColumn(int columnIndex)](#isBlankColumn-int-) | Verifica se la colonna specificata è vuota (non contiene alcun dato). |
| [isColumnHidden(int columnIndex)](#isColumnHidden-int-) | Verifica se una colonna all'indice specificato è nascosta. |
| [isDefaultColumnHidden()](#isDefaultColumnHidden--) |  |
| [isDefaultRowHeightMatched()](#isDefaultRowHeightMatched--) | Indica che l'altezza della riga e l'altezza predefinita del carattere corrispondono. |
| [isDefaultRowHidden()](#isDefaultRowHidden--) | Indica se la riga è nascosta di default. |
| [isDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns)](#isDeletingRangeEnabled-int-int-int-int-) | Verifica se l'intervallo può essere eliminato. |
| [isRowHidden(int rowIndex)](#isRowHidden-int-) | Verifica se una riga all'indice specificato è nascosta. |
| [iterator()](#iterator--) | Ottiene l'enumeratore delle celle. |
| [linkToXmlMap(String mapName, int row, int column, String path)](#linkToXmlMap-java.lang.String-int-int-java.lang.String-) | Collegamento a una mappa XML. |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#merge-int-int-int-int-) | Unisce un intervallo specificato di celle in una singola cella. |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean mergeConflict)](#merge-int-int-int-int-boolean-) | Unisce un intervallo specificato di celle in una singola cella. |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean checkConflict, boolean mergeConflict)](#merge-int-int-int-int-boolean-boolean-) | Unisce un intervallo specificato di celle in una singola cella. |
| [moveRange(CellArea sourceArea, int destRow, int destColumn)](#moveRange-com.aspose.cells.CellArea-int-int-) | Sposta l'intervallo. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeDuplicates()](#removeDuplicates--) | Rimuove le righe duplicate nel foglio. |
| [removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)](#removeDuplicates-int-int-int-int-) | Rimuove i valori duplicati nell'intervallo. |
| [removeDuplicates(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders, int[] columnOffsets)](#removeDuplicates-int-int-int-int-boolean-int---) | Rimuove i dati duplicati dell'intervallo. |
| [removeFormulas()](#removeFormulas--) | Rimuove tutte le formule e le sostituisce con il valore della formula. |
| [retrieveSubtotalSetting(CellArea ca)](#retrieveSubtotalSetting-com.aspose.cells.CellArea-) | Recupera le impostazioni dei subtotali dell'intervallo. |
| [setColumnWidth(int column, double width)](#setColumnWidth-int-double-) | Imposta la larghezza della colonna specificata nella visualizzazione normale. |
| [setColumnWidthInch(int column, double inches)](#setColumnWidthInch-int-double-) | Imposta la larghezza della colonna in unità di pollici nella visualizzazione normale. |
| [setColumnWidthPixel(int column, int pixels)](#setColumnWidthPixel-int-int-) | Imposta la larghezza della colonna in unità di pixel nella visualizzazione normale. |
| [setDefaultColumnHidden(boolean value)](#setDefaultColumnHidden-boolean-) |  |
| [setDefaultRowHeightMatched(boolean value)](#setDefaultRowHeightMatched-boolean-) | Indica che l'altezza della riga e l'altezza predefinita del carattere corrispondono. |
| [setDefaultRowHidden(boolean value)](#setDefaultRowHidden-boolean-) | Indica se la riga è nascosta di default. |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Imposta l'opzione di utilizzo della memoria per queste celle. |
| [setMultiThreadReading(boolean value)](#setMultiThreadReading-boolean-) | Imposta se il modello di dati delle celle deve supportare la lettura multi-thread. |
| [setPreserveString(boolean value)](#setPreserveString-boolean-) | Imposta un valore che indica se tutti i valori del foglio di lavoro sono conservati come stringhe. |
| [setRowHeight(int row, double height)](#setRowHeight-int-double-) | Imposta l'altezza della riga specificata. |
| [setRowHeightInch(int row, double inches)](#setRowHeightInch-int-double-) | Imposta l'altezza della riga in unità di pollici. |
| [setRowHeightPixel(int row, int pixels)](#setRowHeightPixel-int-int-) | Imposta l'altezza della riga in unità di pixel. |
| [setStandardHeight(double value)](#setStandardHeight-double-) | Imposta l'altezza predefinita della riga in questo foglio di lavoro, in unità di punti. |
| [setStandardHeightInch(double value)](#setStandardHeightInch-double-) | Imposta l'altezza predefinita della riga in questo foglio di lavoro, in unità di pollici. |
| [setStandardHeightPixels(int value)](#setStandardHeightPixels-int-) | Imposta l'altezza predefinita della riga in questo foglio di lavoro, in unità di pixel. |
| [setStandardWidth(double value)](#setStandardWidth-double-) | Imposta la larghezza predefinita della colonna nel foglio di lavoro, in unità di caratteri. |
| [setStandardWidthInch(double value)](#setStandardWidthInch-double-) | Imposta la larghezza predefinita della colonna nel foglio di lavoro, in unità di pollici. |
| [setStandardWidthPixels(int value)](#setStandardWidthPixels-int-) | Imposta la larghezza predefinita della colonna nel foglio di lavoro, in unità di pixel. |
| [setStyle(Style value)](#setStyle-com.aspose.cells.Style-) | Imposta lo stile predefinito del foglio di lavoro. |
| [setViewColumnWidthPixel(int column, int pixels)](#setViewColumnWidthPixel-int-int-) | Imposta la larghezza della colonna in diverse visualizzazioni. |
| [showGroupDetail(boolean isVertical, int index)](#showGroupDetail-boolean-int-) | Espande le righe/colonne raggruppate. |
| [subtotal(CellArea ca, int groupBy, int function, int[] totalList)](#subtotal-com.aspose.cells.CellArea-int-int-int---) | Crea subtotali per l'intervallo. |
| [subtotal(CellArea ca, int groupBy, int function, int[] totalList, boolean replace, boolean pageBreaks, boolean summaryBelowData)](#subtotal-com.aspose.cells.CellArea-int-int-int---boolean-boolean-boolean-) | Crea subtotali per l'intervallo. |
| [textToColumns(int row, int column, int totalRows, TxtLoadOptions options)](#textToColumns-int-int-int-com.aspose.cells.TxtLoadOptions-) | Divide il contenuto nella colonna specificata in più colonne.. |
| [toString()](#toString--) |  |
| [unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#unMerge-int-int-int-int-) | Separa un intervallo specificato di celle unite. |
| [ungroupColumns(int firstIndex, int lastIndex)](#ungroupColumns-int-int-) | Separa le colonne. |
| [ungroupRows(int firstIndex, int lastIndex)](#ungroupRows-int-int-) | Separa le righe. |
| [ungroupRows(int firstIndex, int lastIndex, boolean isAll)](#ungroupRows-int-int-boolean-) | Separa le righe. |
| [unhideColumn(int column, double width)](#unhideColumn-int-double-) | Rivela una colonna |
| [unhideColumns(int column, int totalColumns, double width)](#unhideColumns-int-int-double-) | Rivela più colonne. |
| [unhideRow(int row, double height)](#unhideRow-int-double-) | Rivela una riga. |
| [unhideRows(int row, int totalRows, double height)](#unhideRows-int-int-double-) | Rivela le righe nascoste. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addRange(Range rangeObject) {#addRange-com.aspose.cells.Range-}
```
public void addRange(Range rangeObject)
```


Aggiunge un riferimento a un oggetto intervallo alle celle

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rangeObject | [Range](../../com.aspose.cells/range) | L'oggetto intervallo sarà contenuto nelle celle |

### applyColumnStyle(int column, Style style, StyleFlag flag) {#applyColumnStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyColumnStyle(int column, Style style, StyleFlag flag)
```


Applica formati a un'intera colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | L'indice della colonna. |
| style | [Style](../../com.aspose.cells/style) | L'oggetto stile che verrà applicato. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Flag che indicano le proprietà di formattazione applicate. |

### applyRowStyle(int row, Style style, StyleFlag flag) {#applyRowStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyRowStyle(int row, Style style, StyleFlag flag)
```


Applica formati per un'intera riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | L'indice della riga. |
| style | [Style](../../com.aspose.cells/style) | L'oggetto stile che verrà applicato. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Flag che indicano le proprietà di formattazione applicate. |

### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Applica formati a un intero foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | L'oggetto stile che verrà applicato. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Flag che indicano le proprietà di formattazione applicate. |

### checkCell(int row, int column) {#checkCell-int-int-}
```
public Cell checkCell(int row, int column)
```


Restituisce l'elemento [Cell](../../com.aspose.cells/cell) o null all'indice di riga e colonna della cella specificati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice della riga |
| colonna | int | Indice della colonna |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Return Cell object if a Cell object exists. Return null if the cell does not exist.
### checkColumn(int columnIndex) {#checkColumn-int-}
```
public Column checkColumn(int columnIndex)
```


Restituisce l'elemento [Column](../../com.aspose.cells/column) o null all'indice di colonna specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | int | L'indice della colonna. |

**Returns:**
[Column](../../com.aspose.cells/column) - The Column object.
### checkRow(int row) {#checkRow-int-}
```
public Row checkRow(int row)
```


Restituisce l'elemento [Row](../../com.aspose.cells/row) o null all'indice di riga della cella specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice della riga |

**Returns:**
[Row](../../com.aspose.cells/row) - Returns [Row](../../com.aspose.cells/row) object If the row object does exist, otherwise returns null.
### clear() {#clear--}
```
public void clear()
```


Cancella tutti i dati del foglio di lavoro.

### clearContents(CellArea range) {#clearContents-com.aspose.cells.CellArea-}
```
public void clearContents(CellArea range)
```


Cancella il contenuto di un intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| range | [CellArea](../../com.aspose.cells/cellarea) | Intervallo da cancellare. |

### clearContents(int startRow, int startColumn, int endRow, int endColumn) {#clearContents-int-int-int-int-}
```
public void clearContents(int startRow, int startColumn, int endRow, int endColumn)
```


Cancella il contenuto di un intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | int | Indice della riga di inizio. |
| startColumn | int | Indice della colonna di inizio. |
| endRow | int | Indice della riga finale. |
| endColumn | int | Indice della colonna finale. |

### clearFormats(CellArea range) {#clearFormats-com.aspose.cells.CellArea-}
```
public void clearFormats(CellArea range)
```


Cancella la formattazione di un intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| range | [CellArea](../../com.aspose.cells/cellarea) | Intervallo da cancellare. |

### clearFormats(int startRow, int startColumn, int endRow, int endColumn) {#clearFormats-int-int-int-int-}
```
public void clearFormats(int startRow, int startColumn, int endRow, int endColumn)
```


Cancella la formattazione di un intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | int | Indice della riga di inizio. |
| startColumn | int | Indice della colonna di inizio. |
| endRow | int | Indice della riga finale. |
| endColumn | int | Indice della colonna finale. |

### clearMergedCells() {#clearMergedCells--}
```
public void clearMergedCells()
```


Cancella tutti gli intervalli uniti.

### clearRange(CellArea range) {#clearRange-com.aspose.cells.CellArea-}
```
public void clearRange(CellArea range)
```


Cancella il contenuto e la formattazione di un intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| range | [CellArea](../../com.aspose.cells/cellarea) | Intervallo da cancellare. |

### clearRange(int startRow, int startColumn, int endRow, int endColumn) {#clearRange-int-int-int-int-}
```
public void clearRange(int startRow, int startColumn, int endRow, int endColumn)
```


Cancella il contenuto e la formattazione di un intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | int | Indice della riga di inizio. |
| startColumn | int | Indice della colonna di inizio. |
| endRow | int | Indice della riga finale. |
| endColumn | int | Indice della colonna finale. |

### convertStringToNumericValue() {#convertStringToNumericValue--}
```
public void convertStringToNumericValue()
```


Converte tutti i dati stringa nel foglio di lavoro in valori numerici, se possibile.

### copyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex) {#copyColumn-com.aspose.cells.Cells-int-int-}
```
public void copyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex)
```


Copia dati e formati di un'intera colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | L'oggetto Source Cells contiene dati e formati da copiare. |
| sourceColumnIndex | int | Indice della colonna di origine. |
| destinationColumnIndex | int | Indice della colonna di destinazione. |

### copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber) {#copyColumns-com.aspose.cells.Cells-int-int-int-}
```
public void copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)
```


Copia i dati e i formati di intere colonne.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | L'oggetto Source Cells contiene dati e formati da copiare. |
| sourceColumnIndex | int | Indice della colonna di origine. |
| destinationColumnIndex | int | Indice della colonna di destinazione. |
| columnNumber | int | Il numero della colonna copiata. |

### copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber, PasteOptions pasteOptions) {#copyColumns-com.aspose.cells.Cells-int-int-int-com.aspose.cells.PasteOptions-}
```
public void copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber, PasteOptions pasteOptions)
```


Copia dati e formati di un'intera colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | L'oggetto Source Cells contiene dati e formati da copiare. |
| sourceColumnIndex | int | Indice della colonna di origine. |
| destinationColumnIndex | int | Indice della colonna di destinazione. |
| columnNumber | int | Il numero della colonna copiata. |
| pasteOptions | [PasteOptions](../../com.aspose.cells/pasteoptions) | le opzioni di incolla. |

### copyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, int destinationColumnIndex, int destinationTotalColumns) {#copyColumns-com.aspose.cells.Cells-int-int-int-int-}
```
public void copyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, int destinationColumnIndex, int destinationTotalColumns)
```


Copia i dati e i formati di tutte le colonne.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | L'oggetto Source Cells contiene dati e formati da copiare. |
| sourceColumnIndex | int | Indice della colonna di origine. |
| sourceTotalColumns | int | Il numero delle colonne di origine. |
| destinationColumnIndex | int | Indice della colonna di destinazione. |
| destinationTotalColumns | int | Il numero delle colonne di destinazione. |

### copyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex) {#copyRow-com.aspose.cells.Cells-int-int-}
```
public void copyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex)
```


Copia i dati e i formati di un'intera riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | L'oggetto Source Cells contiene dati e formati da copiare. |
| sourceRowIndex | int | Indice della riga di origine. |
| destinationRowIndex | int | Indice della riga di destinazione. |

### copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber) {#copyRows-com.aspose.cells.Cells-int-int-int-}
```
public void copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```


Copia i dati e i formati di alcune intere righe.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | L'oggetto Source Cells contiene dati e formati da copiare. |
| sourceRowIndex | int | Indice della riga di origine. |
| destinationRowIndex | int | Indice della riga di destinazione. |
| rowNumber | int | Il numero della riga copiata. |

### copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions) {#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-}
```
public void copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions)
```


Copia i dati e i formati di alcune intere righe.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | L'oggetto Source Cells contiene dati e formati da copiare. |
| sourceRowIndex | int | Indice della riga di origine. |
| destinationRowIndex | int | Indice della riga di destinazione. |
| rowNumber | int | Il numero della riga copiata. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Le opzioni di copia. |

### copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions) {#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-com.aspose.cells.PasteOptions-}
```
public void copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)
```


Copia i dati e i formati di alcune intere righe.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceCells0 | [Cells](../../com.aspose.cells/cells) | L'oggetto Source Cells contiene dati e formati da copiare. |
| sourceRowIndex | int | Indice della riga di origine. |
| destinationRowIndex | int | Indice della riga di destinazione. |
| rowNumber | int | Il numero della riga copiata. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Le opzioni di copia. |
| pasteOptions | [PasteOptions](../../com.aspose.cells/pasteoptions) | le opzioni di incolla. |

### createRange(int firstIndex, int number, boolean isVertical) {#createRange-int-int-boolean-}
```
public Range createRange(int firstIndex, int number, boolean isVertical)
```


Crea un oggetto [Range](../../com.aspose.cells/range) da righe di celle o colonne di celle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstIndex | int | Indice della prima riga o indice della prima colonna, basato su zero. |
| numero | int | Numero totale di righe o colonne, basato su uno. |
| isVertical | boolean | Vero - Intervallo creato dalle colonne delle celle. Falso - Intervallo creato dalle righe delle celle. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object.
### createRange(int firstRow, int firstColumn, int totalRows, int totalColumns) {#createRange-int-int-int-int-}
```
public Range createRange(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Crea un oggetto [Range](../../com.aspose.cells/range) da un intervallo di celle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstRow | int | Prima riga di questo intervallo |
| firstColumn | int | Prima colonna di questo intervallo |
| totalRows | int | Numero di righe |
| totalColumns | int | Numero di colonne |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### createRange(String address) {#createRange-java.lang.String-}
```
public Range createRange(String address)
```


Crea un oggetto [Range](../../com.aspose.cells/range) da un indirizzo dell'intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indirizzo | java.lang.String | L'indirizzo dell'intervallo. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### createRange(String upperLeftCell, String lowerRightCell) {#createRange-java.lang.String-java.lang.String-}
```
public Range createRange(String upperLeftCell, String lowerRightCell)
```


Crea un oggetto [Range](../../com.aspose.cells/range) da un intervallo di celle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| upperLeftCell | java.lang.String | Nome della cella in alto a sinistra. |
| lowerRightCell | java.lang.String | Nome della cella in basso a destra. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### deleteBlankColumns() {#deleteBlankColumns--}
```
public void deleteBlankColumns()
```


Elimina tutte le colonne vuote che non contengono alcun dato.

### deleteBlankColumns(DeleteOptions options) {#deleteBlankColumns-com.aspose.cells.DeleteOptions-}
```
public void deleteBlankColumns(DeleteOptions options)
```


Elimina tutte le colonne vuote che non contengono alcun dato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | Le opzioni per l'eliminazione dell'intervallo. |

### deleteBlankRows() {#deleteBlankRows--}
```
public void deleteBlankRows()
```


Elimina tutte le righe vuote che non contengono alcun dato o altro oggetto.

### deleteBlankRows(DeleteOptions options) {#deleteBlankRows-com.aspose.cells.DeleteOptions-}
```
public void deleteBlankRows(DeleteOptions options)
```


Elimina tutte le righe vuote che non contengono alcun dato o alcuni oggetti speciali come commenti visibili, tabelle pivot.

**Remarks**

Per le righe vuote che verranno eliminate, non è sufficiente che [Row.isBlank()](../../com.aspose.cells/row\#isBlank--) sia vero, ma è anche necessario che non vi siano commenti visibili definiti per alcuna cella in quelle righe, e nessuna tabella pivot il cui intervallo intersechi esse.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | Le opzioni per l'eliminazione dell'intervallo. |

### deleteColumn(int columnIndex) {#deleteColumn-int-}
```
public void deleteColumn(int columnIndex)
```


Elimina una colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | int | Indice della colonna da eliminare. |

### deleteColumn(int columnIndex, boolean updateReference) {#deleteColumn-int-boolean-}
```
public void deleteColumn(int columnIndex, boolean updateReference)
```


Elimina una colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | int | Indice della colonna da eliminare. |
| updateReference | boolean | Indica se aggiornare i riferimenti in altri fogli di lavoro. |

### deleteColumns(int columnIndex, int totalColumns, boolean updateReference) {#deleteColumns-int-int-boolean-}
```
public void deleteColumns(int columnIndex, int totalColumns, boolean updateReference)
```


Elimina diverse colonne.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | int | Indice della prima colonna da eliminare. |
| totalColumns | int | Numero di colonne da eliminare. |
| updateReference | boolean | Indica se aggiornare i riferimenti in altri fogli di lavoro. |

### deleteColumns(int columnIndex, int totalColumns, DeleteOptions options) {#deleteColumns-int-int-com.aspose.cells.DeleteOptions-}
```
public void deleteColumns(int columnIndex, int totalColumns, DeleteOptions options)
```


Elimina diverse colonne.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | int | Indice della prima colonna da eliminare. |
| totalColumns | int | Numero di colonne da eliminare. |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | Opzioni per l'operazione di eliminazione |

### deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType) {#deleteRange-int-int-int-int-int-}
```
public void deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)
```


Elimina un intervallo di celle e sposta le celle secondo l'opzione di spostamento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | int | Indice della riga di inizio. |
| startColumn | int | Indice della colonna di inizio. |
| endRow | int | Indice della riga finale. |
| endColumn | int | Indice della colonna finale. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Opzione di spostamento delle celle. |

### deleteRow(int rowIndex) {#deleteRow-int-}
```
public void deleteRow(int rowIndex)
```


Elimina una riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int | Indice della riga da eliminare. |

### deleteRow(int rowIndex, boolean updateReference) {#deleteRow-int-boolean-}
```
public void deleteRow(int rowIndex, boolean updateReference)
```


Elimina una riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int | Indice della riga da eliminare. |
| updateReference | boolean | Indica se aggiornare i riferimenti in altri fogli di lavoro. |

### deleteRows(int rowIndex, int totalRows) {#deleteRows-int-int-}
```
public boolean deleteRows(int rowIndex, int totalRows)
```


Elimina più righe.

**Remarks**

Se l'intervallo eliminato contiene la parte superiore (non l'intera) della tabella (ListObject), l'intervallo non può essere eliminato e non verrà eseguita alcuna operazione. Funziona allo stesso modo di MS Excel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int | L'indice della prima riga da eliminare. |
| totalRows | int | Numero di righe da eliminare. |

**Returns:**
boolean
### deleteRows(int rowIndex, int totalRows, boolean updateReference) {#deleteRows-int-int-boolean-}
```
public boolean deleteRows(int rowIndex, int totalRows, boolean updateReference)
```


Elimina più righe nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int | Indice della prima riga da eliminare. |
| totalRows | int | Numero di righe da eliminare. |
| updateReference | boolean | Indica se aggiornare i riferimenti in altri fogli di lavoro. |

**Returns:**
boolean -
### deleteRows(int rowIndex, int totalRows, DeleteOptions options) {#deleteRows-int-int-com.aspose.cells.DeleteOptions-}
```
public boolean deleteRows(int rowIndex, int totalRows, DeleteOptions options)
```


Elimina più righe nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int | Indice della prima riga da eliminare. |
| totalRows | int | Numero di righe da eliminare. |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | Opzioni per l'operazione di eliminazione |

**Returns:**
boolean -
### dispose() {#dispose--}
```
public void dispose()
```


Esegue attività definite dall'applicazione associate al rilascio, alla liberazione o al ripristino di risorse non gestite.

### endCellInColumn(int columnIndex) {#endCellInColumn-int-}
```
public Cell endCellInColumn(int columnIndex)
```


Ottiene l'ultima cella in questa colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | int | Indice di colonna. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### endCellInColumn(int startRow, int endRow, int startColumn, int endColumn) {#endCellInColumn-int-int-int-int-}
```
public Cell endCellInColumn(int startRow, int endRow, int startColumn, int endColumn)
```


Ottiene l'ultima cella con indice di colonna massimo in questo intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | int | Indice della riga di inizio. |
| endRow | int | Indice della riga finale. |
| startColumn | int | Indice della colonna di inizio. |
| endColumn | int | Indice della colonna finale. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### endCellInRow(int rowIndex) {#endCellInRow-int-}
```
public Cell endCellInRow(int rowIndex)
```


Ottiene l'ultima cella in questa riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int | Indice di riga. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### endCellInRow(int startRow, int endRow, int startColumn, int endColumn) {#endCellInRow-int-int-int-int-}
```
public Cell endCellInRow(int startRow, int endRow, int startColumn, int endColumn)
```


Ottiene l'ultima cella con indice di riga massimo in questo intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | int | Indice della riga di inizio. |
| endRow | int | Indice della riga finale. |
| startColumn | int | Indice della colonna di inizio. |
| endColumn | int | Indice della colonna finale. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns) {#exportArray-int-int-int-int-}
```
public Object[][] exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Esporta i dati nella collezione [Cells](../../com.aspose.cells/cells) in un oggetto array bidimensionale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstRow | int | Il numero di riga della prima cella da esportare. |
| firstColumn | int | Il numero di colonna della prima cella da esportare. |
| totalRows | int | Numero di righe da esportare |
| totalColumns | int | Numero di colonne da esportare |

**Returns:**
java.lang.Object[][] - Oggetto array dei valori delle celle esportate.
### exportTypeArray(int firstRow, int firstColumn, int totalRows, int totalColumns) {#exportTypeArray-int-int-int-int-}
```
public int[][] exportTypeArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Esporta il tipo di valore della cella nella collezione [Cells](../../com.aspose.cells/cells) in un oggetto array bidimensionale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstRow | int | Il numero di riga della prima cella da esportare. |
| firstColumn | int | Il numero di colonna della prima cella da esportare. |
| totalRows | int | Numero di righe da esportare. |
| totalColumns | int | Numero di colonne da esportare. |

**Returns:**
int[][] - [CellValueType](../../com.aspose.cells/cellvaluetype). Oggetto array esportato che rappresenta i tipi di valore delle celle.
### find(Object what, Cell previousCell) {#find-java.lang.Object-com.aspose.cells.Cell-}
```
public Cell find(Object what, Cell previousCell)
```


Trova la cella contenente l'oggetto di input.

**Remarks**

Restituisce null (Nothing) se non viene trovata alcuna cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cosa | java.lang.Object | L'oggetto da cercare. Il tipo dovrebbe essere int,double,DateTime,string,bool. |
| previousCell | [Cell](../../com.aspose.cells/cell) | Cella precedente con lo stesso oggetto. Questo parametro può essere impostato a null se la ricerca inizia dall'inizio. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### find(Object what, Cell previousCell, FindOptions findOptions) {#find-java.lang.Object-com.aspose.cells.Cell-com.aspose.cells.FindOptions-}
```
public Cell find(Object what, Cell previousCell, FindOptions findOptions)
```


Trova la cella contenente l'oggetto di input.

**Remarks**

Restituisce null (Nothing) se non viene trovata alcuna cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cosa | java.lang.Object | L'oggetto da cercare. Il tipo dovrebbe essere int,double,DateTime,string,bool. |
| previousCell | [Cell](../../com.aspose.cells/cell) | Cella precedente con lo stesso oggetto. Questo parametro può essere impostato a null se la ricerca inizia dall'inizio. |
| findOptions | [FindOptions](../../com.aspose.cells/findoptions) | Opzioni di ricerca |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### get(int row, int column) {#get-int-int-}
```
public Cell get(int row, int column)
```


Ottiene l'elemento [Cell](../../com.aspose.cells/cell) all'indice di riga e colonna della cella specificati.

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
         Cell cell = cells.get(0, 0);	//Gets the cell at "A1"
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice di riga. |
| colonna | int | Indice di colonna. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - The [Cell](../../com.aspose.cells/cell) object.
### get(String cellName) {#get-java.lang.String-}
```
public Cell get(String cellName)
```


Ottiene l'elemento [Cell](../../com.aspose.cells/cell) al nome della cella specificato.

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
         Cell cell = cells.get("A1");	//Gets the cell at "A1"
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellName | java.lang.String | Nome della cella, includendo la lettera della colonna e il numero della riga, ad esempio A5. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - A [Cell](../../com.aspose.cells/cell) object
### getCellDisplayStyle(int row, int column) {#getCellDisplayStyle-int-int-}
```
public Style getCellDisplayStyle(int row, int column)
```


Ottieni lo stile di visualizzazione della cella fornita.

**Remarks**

Stesso di [Cell.getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--), e lo stesso usando [BorderType.SIDE\_BORDERS](../../com.aspose.cells/bordertype\#SIDE-BORDERS) per [getCellDisplayStyle(int,int,int)](../../com.aspose.cells/cells\#getCellDisplayStyle-int-int-int-).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | indice di riga della cella specificata |
| colonna | int | colonna della cella specificata |

**Returns:**
[Style](../../com.aspose.cells/style) - the display style of given cell.
### getCellDisplayStyle(int row, int column, int adjacentBorders) {#getCellDisplayStyle-int-int-int-}
```
public Style getCellDisplayStyle(int row, int column, int adjacentBorders)
```


Ottieni lo stile di visualizzazione della cella fornita.

**Remarks**

Se la cella è anche influenzata da altre impostazioni come la formattazione condizionale, oggetti elenco, ecc., lo stile di visualizzazione potrebbe differire da [getCellStyle(int,int)](../../com.aspose.cells/cells\#getCellStyle-int-int-). E poiché tali impostazioni possono essere applicate anche a celle vuote (non esistenti), l'uso di questo metodo può evitare l'instanziazione di quelle celle vuote, quindi le prestazioni saranno migliori rispetto all'ottenere l'istanza Cell da Cells e poi chiamare [Cell.getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | indice di riga della cella specificata |
| colonna | int | colonna della cella specificata |
| adjacentBorders | int | [BorderType](../../com.aspose.cells/bordertype). Indica quali bordi devono essere controllati e regolati in base ai bordi delle celle adiacenti. Si prega di consultare la descrizione per lo stesso parametro di [Cell.getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-). |

**Returns:**
[Style](../../com.aspose.cells/style) - the display style of given cell.
### getCellStyle(int row, int column) {#getCellStyle-int-int-}
```
public Style getCellStyle(int row, int column)
```


Ottieni lo stile della cella fornita.

**Remarks**

Lo stile restituito è solo quello impostato per la cella o ereditato dalla riga/colonna della cella, non include le proprietà applicate da altre impostazioni come le formattazioni condizionali.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | indice di riga |
| colonna | int | colonna |

**Returns:**
[Style](../../com.aspose.cells/style) - the style of given cell.
### getCellsWithPlaceInCellPicture() {#getCellsWithPlaceInCellPicture--}
```
public Iterator getCellsWithPlaceInCellPicture()
```


Ottiene tutte le celle che contengono un'immagine incorporata.

**Remarks**

Se non esiste alcuna immagine impostata come "Place in Cell" in questo foglio di lavoro, verrà restituito null.

**Returns:**
java.util.Iterator - Enumeratore per enumerare tutti gli oggetti Cell che contengono immagini incorporate
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


Ottiene l'altezza originale della colonna in unità di punto se la colonna è nascosta.

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo Cells.GetColumnWidth(int ,bool , CellsUnitType ). Questo metodo sarà rimosso 12 mesi dopo, a partire da aprile 2024. Aspose si scusa per eventuali disagi che potreste aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | L'indice della riga. |

**Returns:**
double - Larghezza della colonna nella visualizzazione normale.
### getColumnWidth(int column) {#getColumnWidth-int-}
```
public double getColumnWidth(int column)
```


Ottiene la larghezza (in unità di caratteri) della colonna specificata nella visualizzazione normale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | Indice della colonna |

**Returns:**
double - Larghezza della colonna. Per i fogli di calcolo, la larghezza della colonna è misurata come il numero di caratteri della larghezza massima delle cifre dei numeri 0~9 così come renderizzati nel carattere dello stile normale.
### getColumnWidth(int column, boolean isOriginal, int unitType) {#getColumnWidth-int-boolean-int-}
```
public double getColumnWidth(int column, boolean isOriginal, int unitType)
```


Ottiene la larghezza della colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | L'indice della colonna. |
| isOriginal | boolean | Indica se ottenere la larghezza originale. |
| unitType | int | [CellsUnitType](../../com.aspose.cells/cellsunittype). |

**Returns:**
double -
### getColumnWidthInch(int column) {#getColumnWidthInch-int-}
```
public double getColumnWidthInch(int column)
```


Ottiene la larghezza della colonna specificata nella visualizzazione normale, in unità di pollici.

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo Cells.GetColumnWidth(int ,bool , CellsUnitType ). Questo metodo sarà rimosso 12 mesi dopo, a partire da aprile 2024. Aspose si scusa per eventuali disagi che potreste aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | Indice della colonna |

**Returns:**
double - Larghezza della colonna nella visualizzazione normale.
### getColumnWidthPixel(int column) {#getColumnWidthPixel-int-}
```
public int getColumnWidthPixel(int column)
```


Ottiene la larghezza della colonna specificata nella visualizzazione normale, in unità di pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | Indice della colonna |

**Returns:**
int - Larghezza della colonna nella visualizzazione normale.
### getColumnWidthPixel(int column, boolean original) {#getColumnWidthPixel-int-boolean-}
```
public int getColumnWidthPixel(int column, boolean original)
```


Ottiene la larghezza della colonna specificata nella visualizzazione normale, in unità di pixel.

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo Cells.GetColumnWidth(int ,bool , CellsUnitType ). Questo metodo sarà rimosso 12 mesi dopo, a partire da aprile 2024. Aspose si scusa per eventuali disagi che potreste aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | Indice della colonna |
| originale | boolean | Indica se restituire la larghezza originale anche quando la colonna è nascosta |

**Returns:**
int - Larghezza della colonna nella visualizzazione normale.
### getColumns() {#getColumns--}
```
public ColumnCollection getColumns()
```


Ottiene la raccolta di oggetti [Column](../../com.aspose.cells/column) che rappresentano le singole colonne in questo foglio di lavoro.

**Returns:**
[ColumnCollection](../../com.aspose.cells/columncollection)
### getCount() {#getCount--}
```
public int getCount()
```


Ottiene il conteggio totale degli oggetti Cell istanziati.

**Returns:**
int
### getCountLarge() {#getCountLarge--}
```
public long getCountLarge()
```


Ottiene il conteggio totale degli oggetti Cell istanziati.

**Returns:**
long
### getDependents(boolean isAll, int row, int column) {#getDependents-boolean-int-int-}
```
public Cell[] getDependents(boolean isAll, int row, int column)
```


Ottieni tutte le celle che fanno riferimento alla cella specifica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isAll | boolean | Indica se controllare altri fogli di lavoro |
| riga | int | L'indice della riga. |
| colonna | int | L'indice della colonna. |

**Returns:**
com.aspose.cells.Cell[] -
### getDependentsInCalculation(int row, int column, boolean recursive) {#getDependentsInCalculation-int-int-boolean-}
```
public Iterator getDependentsInCalculation(int row, int column, boolean recursive)
```


Ottiene tutte le celle il cui risultato calcolato dipende dalla cella specifica.

**Remarks**

Per utilizzare questo metodo, assicurarsi che la cartella di lavoro sia stata impostata con valore true per [FormulaSettings.getEnableCalculationChain()](../../com.aspose.cells/formulasettings\#getEnableCalculationChain--) e che sia stata completamente calcolata con questa impostazione. Se non esiste alcun riferimento di formula a questa cella, verrà restituito null. Per maggiori dettagli ed esempi, consultare [Cell.getDependentsInCalculation(boolean)](../../com.aspose.cells/cell\#getDependentsInCalculation-boolean-).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice di riga della cella specifica |
| colonna | int | Indice di colonna della cella specifica. |
| recursive | boolean | Restituisce i dipendenti che non fanno riferimento direttamente alla cella specifica ma fanno riferimento ad altri nodi foglia di quella cella. |

**Returns:**
java.util.Iterator - Enumeratore per elencare tutti i dipendenti (oggetti Cell)
### getFirstCell() {#getFirstCell--}
```
public Cell getFirstCell()
```


Ottiene la prima cella in questo foglio di lavoro.

**Remarks**

Restituisce null se non ci sono dati nel foglio di lavoro.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getFirstDataRow(int column) {#getFirstDataRow-int-}
```
public int getFirstDataRow(int column)
```


Ottiene l'indice della prima riga della cella che contiene dati nella colonna specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | Indice di colonna. |

**Returns:**
int - indice della prima riga.
### getGroupedColumnOutlineLevel(int columnIndex) {#getGroupedColumnOutlineLevel-int-}
```
public int getGroupedColumnOutlineLevel(int columnIndex)
```


Ottiene il livello di contorno (basato su zero) della colonna.

**Remarks**

Se la colonna non è raggruppata, restituisce zero.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | int | L'indice della colonna |

**Returns:**
int - Il livello di outline della colonna
### getGroupedRowOutlineLevel(int rowIndex) {#getGroupedRowOutlineLevel-int-}
```
public int getGroupedRowOutlineLevel(int rowIndex)
```


Ottiene il livello di contorno (basato su zero) della riga.

**Remarks**

Se la riga non è raggruppata, restituisce zero.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int | L'indice della riga. |

**Returns:**
int - Il livello di outline (basato su zero) della riga.
### getLastCell() {#getLastCell--}
```
public Cell getLastCell()
```


Ottiene l'ultima cella in questo foglio di lavoro.

**Remarks**

Restituisce null se non ci sono dati nel foglio di lavoro.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getLastDataRow(int column) {#getLastDataRow-int-}
```
public int getLastDataRow(int column)
```


Ottiene l'indice dell'ultima riga della cella che contiene dati nella colonna specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | Indice di colonna. |

**Returns:**
int - indice dell'ultima riga.
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


Indice massimo della colonna di quelle celle che sono state istanziate nella raccolta (non include la colonna in cui lo stile è definito per l'intera colonna ma nessuna cella è stata istanziata).

**Remarks**

Restituisce -1 se non è stata istanziata alcuna cella.

**Returns:**
int
### getMaxDataColumn() {#getMaxDataColumn--}
```
public int getMaxDataColumn()
```


Indice massimo della colonna della cella che contiene dati.

**Remarks**

\-1 verrà restituito se non esiste alcuna cella contenente dati. Questa proprietà deve iterare e controllare tutte le celle in un foglio di lavoro in modo dinamico, quindi è un processo che richiede tempo e non dovrebbe essere invocata ripetutamente, ad esempio usandola direttamente come condizione in un ciclo.

**Returns:**
int
### getMaxDataRow() {#getMaxDataRow--}
```
public int getMaxDataRow()
```


Indice massimo della riga della cella che contiene dati.

**Remarks**

Restituisce -1 se non esiste alcuna cella contenente dati. Questa proprietà deve iterare e controllare celle e righe in modo dinamico, quindi è un processo che richiede tempo e non dovrebbe essere invocata ripetutamente, ad esempio usandola direttamente come condizione in un ciclo.

**Returns:**
int
### getMaxDisplayRange() {#getMaxDisplayRange--}
```
public Range getMaxDisplayRange()
```


Ottiene l'intervallo massimo che include dati, celle unite e forme.

**Remarks**

Restituisce null se il foglio di lavoro è vuoto a partire da Aspose.Cells 21.5.2.

**Returns:**
[Range](../../com.aspose.cells/range)
### getMaxGroupedColumnOutlineLevel() {#getMaxGroupedColumnOutlineLevel--}
```
public int getMaxGroupedColumnOutlineLevel()
```


Ottiene il livello di contorno della colonna raggruppata massima (basato su zero).

**Returns:**
int - Il livello massimo di outline della colonna raggruppata (basato su zero)
### getMaxGroupedRowOutlineLevel() {#getMaxGroupedRowOutlineLevel--}
```
public int getMaxGroupedRowOutlineLevel()
```


Ottiene il livello di contorno della riga raggruppata massima (basato su zero).

**Returns:**
int - Il livello massimo di outline della riga raggruppata (basato su zero)
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


Indice massimo della riga della cella che contiene dati o stile.

**Remarks**

Restituisce -1 se non esiste alcuna cella contenente dati o stile nel foglio di lavoro. Questa proprietà deve iterare e controllare celle e righe in modo dinamico, quindi è un processo che richiede tempo e non dovrebbe essere invocata ripetutamente, ad esempio usandola direttamente come condizione in un ciclo.

**Returns:**
int
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


Ottiene l'opzione di utilizzo della memoria per queste celle.

Vedi [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Limiti notevoli e operazioni consigliate per alcune modalità:

| Modalità | Osservazioni | Supportato |
| ------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
| [MemorySetting.MEMORY\_PREFERENCE](../../com.aspose.cells/memorysetting\#MEMORY-PREFERENCE) | Cells data will be maintained in compact format to decrease the memory cost. On other hand, the compact data also may cause higher time cost, especially when updating the cells data, or accessing cells/rows randomly | v8.0.0 |
|  | [MemorySetting.FILE\_CACHE](../../com.aspose.cells/memorysetting\#FILE-CACHE) | Quando questa modalità è usata per qualsiasi foglio di lavoro in una cartella di lavoro, [Workbook.dispose()](../../com.aspose.cells/workbook\#dispose--) dovrebbe essere chiamato alla fine del lavoro per rilasciare tutte le risorse, come i file temporanei. |
 
L'accesso casuale alle celle comporta scarse prestazioni perché i dati devono essere letti/aggiornati in modo casuale e ripetuto (così il puntatore nel file verrà modificato di conseguenza e saranno necessarie operazioni di I/O ripetute). Se possibile, accedi sempre ai dati in modo sequenziale (riga per riga).
 
Quando i dati di una riga/cella vengono modificati, i dati di altre celle/righe possono essere influenzati (ad esempio i dati vengono spostati/trasferiti altrove per allocare spazio sufficiente per i dati modificati). Pertanto ogni modifica richiede la sincronizzazione con gli altri oggetti esistenti (come l'oggetto Row o Cell). Per ottenere migliori prestazioni, non mantenere più righe/celle contemporaneamente. Elaborarle una alla volta ridurrà la sincronizzazione dei dati, migliorando leggermente le prestazioni. | v25.7     |

**Returns:**
int
### getMergedAreas() {#getMergedAreas--}
```
public CellArea[] getMergedAreas()
```


Ottiene tutte le celle unite.

**Returns:**
com.aspose.cells.CellArea[]
### getMergedCells() {#getMergedCells--}
```
public ArrayList getMergedCells()
```


Ottiene la raccolta delle celle unite.

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, utilizza il metodo Cells.GetMergedAreas(). Questo metodo sarà rimosso tra 12 mesi a partire da novembre 2023. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
java.util.ArrayList
### getMinColumn() {#getMinColumn--}
```
public int getMinColumn()
```


Indice minimo di colonna di quelle celle che sono state istanziate nella raccolta (non include la colonna in cui lo stile è definito per l'intera colonna ma non è stata istanziata alcuna cella).

**Remarks**

Questa proprietà deve iterare e controllare celle e righe in modo dinamico, quindi è un processo che richiede tempo e non dovrebbe essere invocata ripetutamente, ad esempio usandola direttamente come condizione in un ciclo.

**Returns:**
int
### getMinDataColumn() {#getMinDataColumn--}
```
public int getMinDataColumn()
```


Indice minimo di colonna della cella che contiene dati.

**Remarks**

\-1 verrà restituito se non esiste alcuna cella contenente dati. Questa proprietà deve iterare e controllare tutte le celle in un foglio di lavoro in modo dinamico, quindi è un processo che richiede tempo e non dovrebbe essere invocata ripetutamente, ad esempio usandola direttamente come condizione in un ciclo.

**Returns:**
int
### getMinDataRow() {#getMinDataRow--}
```
public int getMinDataRow()
```


Indice minimo di riga della cella che contiene dati.

**Remarks**

Restituisce -1 se non esiste alcuna cella contenente dati. Questa proprietà deve iterare e controllare celle e righe in modo dinamico, quindi è un processo che richiede tempo e non dovrebbe essere invocata ripetutamente, ad esempio usandola direttamente come condizione in un ciclo.

**Returns:**
int
### getMinRow() {#getMinRow--}
```
public int getMinRow()
```


Indice minimo di riga della cella che contiene dati o stile.

**Remarks**

Questa proprietà deve iterare e controllare celle e righe in modo dinamico, quindi è un processo che richiede tempo e non dovrebbe essere invocata ripetutamente, ad esempio usandola direttamente come condizione in un ciclo.

**Returns:**
int
### getMultiThreadReading() {#getMultiThreadReading--}
```
public boolean getMultiThreadReading()
```


Restituisce se il modello dati delle celle deve supportare la lettura Multi-Thread. Il valore predefinito di questa proprietà è false.

**Remarks**

Se ci sono più thread che leggono oggetti Row/Cell in questa collezione contemporaneamente, questa proprietà dovrebbe essere impostata su true, altrimenti potrebbero verificarsi risultati inattesi. Supportare la lettura Multi-Thread può degradare le prestazioni per l'accesso agli oggetti Row/Cell da questa collezione. Si prega di notare che alcune funzionalità non possono supportare la lettura Multi-Thread, come la formattazione dei valori (tramite [Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--), [Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), ecc.). Quindi, anche con questa proprietà impostata su true, quelle API potrebbero comunque dare risultati inattesi per la lettura Multi-Thread.

**Returns:**
boolean
### getOdsCellFields() {#getOdsCellFields--}
```
public OdsCellFieldCollection getOdsCellFields()
```


Ottiene l'elenco dei campi di ods.

**Returns:**
[OdsCellFieldCollection](../../com.aspose.cells/odscellfieldcollection)
### getPreserveString() {#getPreserveString--}
```
public boolean getPreserveString()
```


Restituisce un valore che indica se tutti i valori del foglio di lavoro sono conservati come stringhe. Il valore predefinito è false.

**Returns:**
boolean
### getRanges() {#getRanges--}
```
public RangeCollection getRanges()
```


Ottiene la raccolta degli oggetti [Range](../../com.aspose.cells/range) creati a runtime.

**Returns:**
[RangeCollection](../../com.aspose.cells/rangecollection)
### getRowEnumerator() {#getRowEnumerator--}
```
public Iterator getRowEnumerator()
```


Ottiene l'enumeratore delle righe.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo RowCollection.GetEnumerator(). Questo metodo sarà rimosso 12 mesi dopo, a partire da maggio 2023. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Returns:**
java.util.Iterator - L'enumeratore delle righe.
### getRowHeight(int row) {#getRowHeight-int-}
```
public double getRowHeight(int row)
```


Ottiene l'altezza di una riga specificata, in unità di punti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice della riga |

**Returns:**
double - Altezza della riga
### getRowHeight(int row, boolean isOriginal, int unitType) {#getRowHeight-int-boolean-int-}
```
public double getRowHeight(int row, boolean isOriginal, int unitType)
```


Ottiene l'altezza della riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | L'indice della riga. |
| isOriginal | boolean | Indica se restituisce l'altezza originale della riga o 0 per una riga nascosta. |
| unitType | int | [CellsUnitType](../../com.aspose.cells/cellsunittype). Tipo di unità del valore di altezza restituito |

**Returns:**
double - Altezza della riga
### getRowHeightInch(int row) {#getRowHeightInch-int-}
```
public double getRowHeightInch(int row)
```


Ottiene l'altezza di una riga specificata in unità di pollici.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice della riga |

**Returns:**
double - Altezza della riga
### getRowHeightPixel(int row) {#getRowHeightPixel-int-}
```
public int getRowHeightPixel(int row)
```


Ottiene l'altezza di una riga specificata in unità di pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice della riga |

**Returns:**
int - Altezza della riga
### getRowOriginalHeightPoint(int row) {#getRowOriginalHeightPoint-int-}
```
public double getRowOriginalHeightPoint(int row)
```


Ottiene l'altezza originale della riga in unità di punti se la riga è nascosta

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo Cells.GetRowHeight(int,bool,CellsUnitType). Questo metodo sarà rimosso 12 mesi dopo, a partire da aprile 2024. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | L'indice della riga. |

**Returns:**
double -
### getRows() {#getRows--}
```
public RowCollection getRows()
```


Ottiene la raccolta degli oggetti [Row](../../com.aspose.cells/row) che rappresentano le singole righe in questo foglio di lavoro.

**Returns:**
[RowCollection](../../com.aspose.cells/rowcollection)
### getStandardHeight() {#getStandardHeight--}
```
public double getStandardHeight()
```


Ottiene l'altezza predefinita delle righe in questo foglio di lavoro, in unità di punti.

**Returns:**
double
### getStandardHeightInch() {#getStandardHeightInch--}
```
public double getStandardHeightInch()
```


Ottiene l'altezza predefintta delle righe in questo foglio di lavoro, in unità di pollici.

**Returns:**
double
### getStandardHeightPixels() {#getStandardHeightPixels--}
```
public int getStandardHeightPixels()
```


Ottiene l'altezza predefinita delle righe in questo foglio di lavoro, in unità di pixel.

**Returns:**
int
### getStandardWidth() {#getStandardWidth--}
```
public double getStandardWidth()
```


Ottiene la larghezza predefinita delle colonne nel foglio di lavoro, in unità di caratteri.

**Returns:**
double
### getStandardWidthInch() {#getStandardWidthInch--}
```
public double getStandardWidthInch()
```


Ottiene la larghezza predefinita delle colonne nel foglio di lavoro, in unità di pollici.

**Returns:**
double
### getStandardWidthPixels() {#getStandardWidthPixels--}
```
public int getStandardWidthPixels()
```


Ottiene la larghezza predefinita delle colonne nel foglio di lavoro, in unità di pixel.

**Returns:**
int
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Ottiene lo stile predefinito del foglio di lavoro.

**Returns:**
[Style](../../com.aspose.cells/style)
### getViewColumnWidthPixel(int column) {#getViewColumnWidthPixel-int-}
```
public int getViewColumnWidthPixel(int column)
```


Ottieni la larghezza in diversi tipi di visualizzazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | L'indice della colonna. |

**Returns:**
int - la larghezza della colonna in unità di pixel
### getViewRowHeight(int row) {#getViewRowHeight-int-}
```
public double getViewRowHeight(int row)
```


Ottiene l'altezza di una riga specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice di riga. |

**Returns:**
double - Altezza della riga.
### getViewRowHeightInch(int row) {#getViewRowHeightInch-int-}
```
public double getViewRowHeightInch(int row)
```


Ottiene l'altezza di una riga specificata in unità di pollici.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice della riga |

**Returns:**
double - Altezza della riga
### groupColumns(int firstIndex, int lastIndex) {#groupColumns-int-int-}
```
public void groupColumns(int firstIndex, int lastIndex)
```


Raggruppa le colonne.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstIndex | int | Il primo indice di colonna da raggruppare. |
| lastIndex | int | L'ultimo indice di colonna da raggruppare. |

### groupColumns(int firstIndex, int lastIndex, boolean isHidden) {#groupColumns-int-int-boolean-}
```
public void groupColumns(int firstIndex, int lastIndex, boolean isHidden)
```


Raggruppa le colonne.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstIndex | int | Il primo indice di colonna da raggruppare. |
| lastIndex | int | L'ultimo indice di colonna da raggruppare. |
| isHidden | boolean | Specifica se le colonne raggruppate sono nascoste. |

### groupRows(int firstIndex, int lastIndex) {#groupRows-int-int-}
```
public void groupRows(int firstIndex, int lastIndex)
```


Raggruppa le righe.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstIndex | int | Il primo indice di riga da raggruppare. |
| lastIndex | int | L'ultimo indice di riga da raggruppare. |

### groupRows(int firstIndex, int lastIndex, boolean isHidden) {#groupRows-int-int-boolean-}
```
public void groupRows(int firstIndex, int lastIndex, boolean isHidden)
```


Raggruppa le righe.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstIndex | int | Il primo indice di riga da raggruppare. |
| lastIndex | int | L'ultimo indice di riga da raggruppare. |
| isHidden | boolean | Specifica se le righe raggruppate sono nascoste. |

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


Nasconde una colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | Indice di colonna. |

### hideColumns(int column, int totalColumns) {#hideColumns-int-int-}
```
public void hideColumns(int column, int totalColumns)
```


Nascondi più colonne.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | Indice di colonna. |
| totalColumns | int | Numero di colonna. |

### hideGroupDetail(boolean isVertical, int index) {#hideGroupDetail-boolean-int-}
```
public void hideGroupDetail(boolean isVertical, int index)
```


Comprimi le righe/colonne raggruppate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isVertical | boolean | True, comprimi le righe raggruppate. |
| indice | int | L'indice riga/colonna |

### hideRow(int row) {#hideRow-int-}
```
public void hideRow(int row)
```


Nasconde una riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice di riga. |

### hideRows(int row, int totalRows) {#hideRows-int-int-}
```
public void hideRows(int row, int totalRows)
```


Nasconde più righe.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | L'indice della riga. |
| totalRows | int | Il numero di riga. |

### importArray(double[] doubleArray, int firstRow, int firstColumn, boolean isVertical) {#importArray-double---int-int-boolean-}
```
public void importArray(double[] doubleArray, int firstRow, int firstColumn, boolean isVertical)
```


Importa un array di double in un foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| doubleArray | double[] | Array di double. |
| firstRow | int | Il numero di riga della prima cella da importare. |
| firstColumn | int | Il numero di colonna della prima cella da importare. |
| isVertical | boolean | Specifica se importare i dati verticalmente o orizzontalmente. |

### importArray(double[][] doubleArray, int firstRow, int firstColumn) {#importArray-double-----int-int-}
```
public void importArray(double[][] doubleArray, int firstRow, int firstColumn)
```


Importa un array bidimensionale di double in un foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| doubleArray | double[][] | Array double bidimensionale. |
| firstRow | int | Il numero di riga della prima cella da importare. |
| firstColumn | int | Il numero di colonna della prima cella da importare. |

### importArray(int[] intArray, int firstRow, int firstColumn, boolean isVertical) {#importArray-int---int-int-boolean-}
```
public void importArray(int[] intArray, int firstRow, int firstColumn, boolean isVertical)
```


Importa un array di integer in un foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| intArray | int[] | Array di interi. |
| firstRow | int | Il numero di riga della prima cella da importare. |
| firstColumn | int | Il numero di colonna della prima cella da importare. |
| isVertical | boolean | Specifica se importare i dati verticalmente o orizzontalmente. |

### importArray(int[][] intArray, int firstRow, int firstColumn) {#importArray-int-----int-int-}
```
public void importArray(int[][] intArray, int firstRow, int firstColumn)
```


Importa un array bidimensionale di integer in un foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| intArray | int[][] | Array di interi bidimensionale. |
| firstRow | int | Il numero di riga della prima cella da importare. |
| firstColumn | int | Il numero di colonna della prima cella da importare. |

### importArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical) {#importArray-java.lang.String---int-int-boolean-}
```
public void importArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)
```


Importa un array di string in un foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stringArray | java.lang.String[] | Array di stringhe. |
| firstRow | int | Il numero di riga della prima cella da importare. |
| firstColumn | int | Il numero di colonna della prima cella da importare. |
| isVertical | boolean | Specifica se importare i dati verticalmente o orizzontalmente. |

### importArray(String[][] stringArray, int firstRow, int firstColumn) {#importArray-java.lang.String-----int-int-}
```
public void importArray(String[][] stringArray, int firstRow, int firstColumn)
```


Importa un array bidimensionale di string in un foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stringArray | java.lang.String[][] | Array di stringhe bidimensionale. |
| firstRow | int | Il numero di riga della prima cella da importare. |
| firstColumn | int | Il numero di colonna della prima cella da importare. |

### importArrayList(ArrayList arrayList, int firstRow, int firstColumn, boolean isVertical) {#importArrayList-java.util.ArrayList-int-int-boolean-}
```
public void importArrayList(ArrayList arrayList, int firstRow, int firstColumn, boolean isVertical)
```


Importa un arraylist di dati in un foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arrayList | java.util.ArrayList | Arraylist di dati. |
| firstRow | int | Il numero di riga della prima cella da importare. |
| firstColumn | int | Il numero di colonna della prima cella da importare. |
| isVertical | boolean | Specifica se importare i dati verticalmente o orizzontalmente. |

### importCSV(InputStream stream, TxtLoadOptions options, int firstRow, int firstColumn) {#importCSV-java.io.InputStream-com.aspose.cells.TxtLoadOptions-int-int-}
```
public void importCSV(InputStream stream, TxtLoadOptions options, int firstRow, int firstColumn)
```


Importa un file CSV nelle celle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.InputStream | Il flusso del file CSV. |
| options | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | Le opzioni di caricamento per la lettura del file di testo |
| firstRow | int | Il numero di riga della prima cella da importare. |
| firstColumn | int | Il numero di colonna della prima cella da importare. |

### importCSV(InputStream stream, String splitter, boolean convertNumericData, int firstRow, int firstColumn) {#importCSV-java.io.InputStream-java.lang.String-boolean-int-int-}
```
public void importCSV(InputStream stream, String splitter, boolean convertNumericData, int firstRow, int firstColumn)
```


Importa un file CSV nelle celle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.InputStream | Il flusso del file CSV. |
| splitter | java.lang.String | Il separatore |
| convertNumericData | boolean | Indica se la stringa nel file di testo viene convertita in dati numerici. |
| firstRow | int | Il numero di riga della prima cella da importare. |
| firstColumn | int | Il numero di colonna della prima cella da importare. |

### importCSV(String fileName, TxtLoadOptions options, int firstRow, int firstColumn) {#importCSV-java.lang.String-com.aspose.cells.TxtLoadOptions-int-int-}
```
public void importCSV(String fileName, TxtLoadOptions options, int firstRow, int firstColumn)
```


Importa un file CSV nelle celle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | Il nome del file CSV. |
| options | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | Le opzioni di caricamento per la lettura del file di testo |
| firstRow | int | Il numero di riga della prima cella da importare. |
| firstColumn | int | Il numero di colonna della prima cella da importare. |

### importCSV(String fileName, String splitter, boolean convertNumericData, int firstRow, int firstColumn) {#importCSV-java.lang.String-java.lang.String-boolean-int-int-}
```
public void importCSV(String fileName, String splitter, boolean convertNumericData, int firstRow, int firstColumn)
```


Importa un file CSV nelle celle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | Il nome del file CSV. |
| splitter | java.lang.String | Il separatore |
| convertNumericData | boolean | Indica se la stringa nel file di testo viene convertita in dati numerici. |
| firstRow | int | Il numero di riga della prima cella da importare. |
| firstColumn | int | Il numero di colonna della prima cella da importare. |

### importCustomObjects(Collection list, int firstRow, int firstColumn, ImportTableOptions options) {#importCustomObjects-java.util.Collection-int-int-com.aspose.cells.ImportTableOptions-}
```
public int importCustomObjects(Collection list, int firstRow, int firstColumn, ImportTableOptions options)
```


Importa oggetti personalizzati.

**Remarks**

Gli oggetti personalizzati dovrebbero essere dello stesso tipo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| lista | java.util.Collection | L'oggetto personalizzato |
| firstRow | int | Il numero di riga della prima cella da importare. |
| firstColumn | int | Il numero di colonna della prima cella da importare. |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | Le opzioni di importazione. |

**Returns:**
int - Numero totale di righe importate.
### importCustomObjects(Collection list, String[] propertyNames, boolean isPropertyNameShown, int firstRow, int firstColumn, int rowNumber, boolean insertRows, String dateFormatString, boolean convertStringToNumber) {#importCustomObjects-java.util.Collection-java.lang.String---boolean-int-int-int-boolean-java.lang.String-boolean-}
```
public int importCustomObjects(Collection list, String[] propertyNames, boolean isPropertyNameShown, int firstRow, int firstColumn, int rowNumber, boolean insertRows, String dateFormatString, boolean convertStringToNumber)
```


Importa oggetti personalizzati.

**Remarks**

Gli oggetti personalizzati dovrebbero essere dello stesso tipo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| lista | java.util.Collection | L'oggetto personalizzato |
| propertyNames | java.lang.String[] | I nomi delle proprietà. Se è null, importeremo tutte le proprietà dell'oggetto. |
| isPropertyNameShown | boolean | Indica se il nome della proprietà verrà importato nella prima riga. |
| firstRow | int | Il numero di riga della prima cella da importare. |
| firstColumn | int | Il numero di colonna della prima cella da importare. |
| rowNumber | int | Numero di righe da importare. |
| insertRows | boolean | Indica se vengono aggiunte righe extra per adattare i dati. |
| dateFormatString | java.lang.String | Stringa di formato data per le celle. |
| convertStringToNumber | boolean | Indica se questo metodo proverà a convertire la stringa in numero. |

**Returns:**
int - Numero totale di righe importate.
### importData(ICellsDataTable table, int firstRow, int firstColumn, ImportTableOptions options) {#importData-com.aspose.cells.ICellsDataTable-int-int-com.aspose.cells.ImportTableOptions-}
```
public int importData(ICellsDataTable table, int firstRow, int firstColumn, ImportTableOptions options)
```


Importa dati da una tabella dati personalizzata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| table | [ICellsDataTable](../../com.aspose.cells/icellsdatatable) | La tabella dati personalizzata. |
| firstRow | int | Indice della prima riga. |
| firstColumn | int | Indice della prima colonna. |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | Le opzioni di importazione |

**Returns:**
int -
### importFormulaArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical) {#importFormulaArray-java.lang.String---int-int-boolean-}
```
public void importFormulaArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)
```


Importa un array di formula in un foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stringArray | java.lang.String[] | Array di formule. |
| firstRow | int | Il numero di riga della prima cella da importare. |
| firstColumn | int | Il numero di colonna della prima cella da importare. |
| isVertical | boolean | Specifica se importare i dati verticalmente o orizzontalmente. |

### importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical) {#importObjectArray-java.lang.Object---int-int-boolean-}
```
public void importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical)
```


Importa un array di dati in un foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| objArray | java.lang.Object[] | Array di dati. |
| firstRow | int | Il numero di riga della prima cella da importare. |
| firstColumn | int | Il numero di colonna della prima cella da importare. |
| isVertical | boolean | Specifica se importare i dati verticalmente o orizzontalmente. |

### importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical, int skip) {#importObjectArray-java.lang.Object---int-int-boolean-int-}
```
public void importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical, int skip)
```


Importa un array di dati in un foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| objArray | java.lang.Object[] | Array di dati. |
| firstRow | int | Il numero di riga della prima cella da importare. |
| firstColumn | int | Il numero di colonna della prima cella da importare. |
| isVertical | boolean | Specifica se importare i dati verticalmente o orizzontalmente. |
| ignora | int | Numero di righe o colonne saltate. |

### importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-int-int-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown)
```


Importa dati da un oggetto ResultSet nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rs | java.sql.ResultSet | l'oggetto ResultSet da cui importare. |
| rowIndex | int | indice della riga iniziale nel foglio di lavoro. |
| columnIndex | int | indice della colonna iniziale nel foglio di lavoro. |
| isFieldNameShown | boolean | Indica se il nome del campo del resultset verrà importato nella prima riga. |

**Returns:**
int - quante righe sono state effettivamente importate.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber) {#importResultSet-java.sql.ResultSet-int-int-boolean-java.lang.String-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)
```


Importa dati da un oggetto ResultSet nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rs | java.sql.ResultSet | l'oggetto ResultSet da cui importare. |
| rowIndex | int | indice della riga iniziale nel foglio di lavoro. |
| columnIndex | int | indice della colonna iniziale nel foglio di lavoro. |
| isFieldNameShown | boolean | Indica se il nome del campo del resultset verrà importato nella prima riga. |
| customDateFormatString | java.lang.String | Stringa di formato data per le celle che contengono un valore di data. |
| convertStringToNumber | boolean | Indica se questo metodo proverà a convertire la stringa in numero. |

**Returns:**
int - quante righe sono state effettivamente importate.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, ImportTableOptions options) {#importResultSet-java.sql.ResultSet-int-int-com.aspose.cells.ImportTableOptions-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, ImportTableOptions options)
```


Importa dati da un oggetto ResultSet nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rs | java.sql.ResultSet | l'oggetto ResultSet da cui importare. |
| rowIndex | int | indice della riga iniziale nel foglio di lavoro. |
| columnIndex | int | indice della colonna iniziale nel foglio di lavoro. |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | Le opzioni di importazione |

**Returns:**
int - quante righe sono state effettivamente importate.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown)
```


Importa dati da un oggetto ResultSet nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rs | java.sql.ResultSet | l'oggetto ResultSet da cui importare. |
| rowIndex | int | indice della riga iniziale nel foglio di lavoro. |
| columnIndex | int | indice della colonna iniziale nel foglio di lavoro. |
| rowNum | int | numero di righe da importare. -1 per importare tutti i record nel resultset specificato. |
| columnNum | int | numero di colonne da importare. -1 per importare tutte le colonne nel resultset specificato. |
| isFieldNameShown | boolean | Indica se il nome del campo del resultset verrà importato nella prima riga. |

**Returns:**
int - quante righe sono state effettivamente importate.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber) {#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-java.lang.String-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)
```


Importa dati da un oggetto ResultSet nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rs | java.sql.ResultSet | l'oggetto ResultSet da cui importare. |
| rowIndex | int | indice della riga iniziale nel foglio di lavoro. |
| columnIndex | int | indice della colonna iniziale nel foglio di lavoro. |
| rowNum | int | numero di righe da importare. -1 per importare tutti i record nel resultset specificato. |
| columnNum | int | numero di colonne da importare. -1 per importare tutte le colonne nel resultset specificato. |
| isFieldNameShown | boolean | Indica se il nome del campo del resultset verrà importato nella prima riga. |
| customDateFormatString | java.lang.String | Stringa di formato data per le celle che contengono un valore di data. |
| convertStringToNumber | boolean | Indica se questo metodo proverà a convertire la stringa in numero. |

**Returns:**
int - quante righe sono state effettivamente importate.
### importResultSet(ResultSet rs, String startCell, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-java.lang.String-boolean-}
```
public int importResultSet(ResultSet rs, String startCell, boolean isFieldNameShown)
```


Importa dati da un oggetto ResultSet nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rs | java.sql.ResultSet | l'oggetto ResultSet da cui importare. |
| startCell | java.lang.String | nome della cella iniziale in cui inserire il resultset, ad esempio "A1". |
| isFieldNameShown | boolean | Indica se il nome del campo del resultset verrà importato nella prima riga. |

**Returns:**
int - quante righe sono state effettivamente importate.
### importResultSet(ResultSet rs, String startCell, ImportTableOptions options) {#importResultSet-java.sql.ResultSet-java.lang.String-com.aspose.cells.ImportTableOptions-}
```
public int importResultSet(ResultSet rs, String startCell, ImportTableOptions options)
```


Importa dati da un oggetto ResultSet nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rs | java.sql.ResultSet | l'oggetto ResultSet da cui importare. |
| startCell | java.lang.String | nome della cella iniziale in cui inserire il resultset, ad esempio "A1". |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | Le opzioni di importazione |

**Returns:**
int - quante righe sono state effettivamente importate.
### importResultSet(ResultSet rs, String startCell, int rowNum, int columnNum, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-java.lang.String-int-int-boolean-}
```
public int importResultSet(ResultSet rs, String startCell, int rowNum, int columnNum, boolean isFieldNameShown)
```


Importa dati da un oggetto ResultSet nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rs | java.sql.ResultSet | l'oggetto ResultSet da cui importare. |
| startCell | java.lang.String | nome della cella iniziale in cui inserire il resultset, ad esempio "A1". |
| rowNum | int | numero di righe da importare. -1 per importare tutti i record nel resultset specificato. |
| columnNum | int | numero di colonne da importare. -1 per importare tutte le colonne nel resultset specificato. |
| isFieldNameShown | boolean | Indica se il nome del campo del resultset verrà importato nella prima riga. |

**Returns:**
int - quante righe sono state effettivamente importate.
### importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn) {#importTwoDimensionArray-java.lang.Object-----int-int-}
```
public void importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn)
```


Importa un array bidimensionale di dati in un foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| objArray | java.lang.Object[][] | Array di dati bidimensionale. |
| firstRow | int | Il numero di riga della prima cella da importare. |
| firstColumn | int | Il numero di colonna della prima cella da importare. |

### importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn, boolean convertStringToNumber) {#importTwoDimensionArray-java.lang.Object-----int-int-boolean-}
```
public void importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn, boolean convertStringToNumber)
```


Importa un array bidimensionale di dati in un foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| objArray | java.lang.Object[][] | Array di dati bidimensionale. |
| firstRow | int | Il numero di riga della prima cella da importare. |
| firstColumn | int | Il numero di colonna della prima cella da importare. |
| convertStringToNumber | boolean | Indica se questo metodo proverà a convertire la stringa in numero. |

### importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, boolean convertStringToNumber) {#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-boolean-}
```
public void importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, boolean convertStringToNumber)
```


Importa un array bidimensionale di dati in un foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| objArray | java.lang.Object[][] | Array di dati bidimensionale. |
| stili | java.lang.Object[][] | Stile dei dati bidimensionale. |
| firstRow | int | Il numero di riga della prima cella da importare. |
| firstColumn | int | Il numero di colonna della prima cella da importare. |
| convertStringToNumber | boolean | Indica se questo metodo proverà a convertire la stringa in numero. |

### importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, TxtLoadOptions opts) {#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-com.aspose.cells.TxtLoadOptions-}
```
public void importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, TxtLoadOptions opts)
```


Importa un array bidimensionale di dati in un foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| objArray | java.lang.Object[][] | Array di dati bidimensionale. |
| stili | java.lang.Object[][] | Stile dei dati bidimensionale. |
| firstRow | int | Il numero di riga della prima cella da importare. |
| firstColumn | int | Il numero di colonna della prima cella da importare. |
| opts | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | Opzioni per la conversione dei valori stringa |

### insertColumn(int columnIndex) {#insertColumn-int-}
```
public void insertColumn(int columnIndex)
```


Inserisce una nuova colonna nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | int | Indice di colonna. |

### insertColumn(int columnIndex, boolean updateReference) {#insertColumn-int-boolean-}
```
public void insertColumn(int columnIndex, boolean updateReference)
```


Inserisce una nuova colonna nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | int | Indice di colonna. |
| updateReference | boolean | Indica se i riferimenti in altri fogli di lavoro saranno aggiornati. |

### insertColumns(int columnIndex, int totalColumns) {#insertColumns-int-int-}
```
public void insertColumns(int columnIndex, int totalColumns)
```


Inserisce alcune colonne nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | int | Indice di colonna. |
| totalColumns | int | Il numero di colonne. |

### insertColumns(int columnIndex, int totalColumns, boolean updateReference) {#insertColumns-int-int-boolean-}
```
public void insertColumns(int columnIndex, int totalColumns, boolean updateReference)
```


Inserisce alcune colonne nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | int | Indice di colonna. |
| totalColumns | int | Il numero di colonne. |
| updateReference | boolean | Indica se i riferimenti in altri fogli di lavoro saranno aggiornati. |

### insertColumns(int columnIndex, int totalColumns, InsertOptions options) {#insertColumns-int-int-com.aspose.cells.InsertOptions-}
```
public void insertColumns(int columnIndex, int totalColumns, InsertOptions options)
```


Inserisce alcune colonne nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | int | Indice di colonna. |
| totalColumns | int | Il numero di colonne. |
| options | [InsertOptions](../../com.aspose.cells/insertoptions) | Le opzioni per l'operazione di inserimento. |

### insertCutCells(Range cutRange, int row, int column, int shiftType) {#insertCutCells-com.aspose.cells.Range-int-int-int-}
```
public void insertCutCells(Range cutRange, int row, int column, int shiftType)
```


Inserisci intervallo tagliato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cutRange | [Range](../../com.aspose.cells/range) | L'intervallo di taglio. |
| riga | int | La riga. |
| colonna | int | La colonna. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Indica come spostare gli altri oggetti dell'intervallo di destinazione quando si inserisce l'intervallo tagliato. |

### insertRange(CellArea area, int shiftType) {#insertRange-com.aspose.cells.CellArea-int-}
```
public void insertRange(CellArea area, int shiftType)
```


Inserisce un intervallo di celle e sposta le celle in base all'opzione di spostamento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| area | [CellArea](../../com.aspose.cells/cellarea) | Sposta area. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Opzione di spostamento delle celle. |

### insertRange(CellArea area, int shiftNumber, int shiftType) {#insertRange-com.aspose.cells.CellArea-int-int-}
```
public void insertRange(CellArea area, int shiftNumber, int shiftType)
```


Inserisce un intervallo di celle e sposta le celle in base all'opzione di spostamento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| area | [CellArea](../../com.aspose.cells/cellarea) | Sposta area. |
| shiftNumber | int | Numero di righe o colonne da inserire. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Opzione di spostamento delle celle. |

### insertRange(CellArea area, int shiftNumber, int shiftType, boolean updateReference) {#insertRange-com.aspose.cells.CellArea-int-int-boolean-}
```
public void insertRange(CellArea area, int shiftNumber, int shiftType, boolean updateReference)
```


Inserisce un intervallo di celle e sposta le celle in base all'opzione di spostamento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| area | [CellArea](../../com.aspose.cells/cellarea) | Sposta area. |
| shiftNumber | int | Numero di righe o colonne da inserire. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Opzione di spostamento delle celle. |
| updateReference | boolean | Indica se aggiornare i riferimenti in altri fogli di lavoro. |

### insertRow(int rowIndex) {#insertRow-int-}
```
public void insertRow(int rowIndex)
```


Inserisce una nuova riga nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int | Indice di riga. |

### insertRows(int rowIndex, int totalRows) {#insertRows-int-int-}
```
public void insertRows(int rowIndex, int totalRows)
```


Inserisce più righe nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int | Indice di riga. |
| totalRows | int | Numero di righe da inserire. |

### insertRows(int rowIndex, int totalRows, boolean updateReference) {#insertRows-int-int-boolean-}
```
public void insertRows(int rowIndex, int totalRows, boolean updateReference)
```


Inserisce più righe nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int | Indice di riga. |
| totalRows | int | Numero di righe da inserire. |
| updateReference | boolean | Indica se i riferimenti in altri fogli di lavoro saranno aggiornati. |

### insertRows(int rowIndex, int totalRows, InsertOptions options) {#insertRows-int-int-com.aspose.cells.InsertOptions-}
```
public void insertRows(int rowIndex, int totalRows, InsertOptions options)
```


Inserisce più righe nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int | Indice di riga. |
| totalRows | int | Numero di righe da inserire. |
| options | [InsertOptions](../../com.aspose.cells/insertoptions) | Opzioni per l'operazione di inserimento. |

### isBlankColumn(int columnIndex) {#isBlankColumn-int-}
```
public boolean isBlankColumn(int columnIndex)
```


Verifica se la colonna specificata è vuota (non contiene alcun dato).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | int | l'indice della colonna |

**Returns:**
boolean - true se la colonna specificata non contiene alcun dato
### isColumnHidden(int columnIndex) {#isColumnHidden-int-}
```
public boolean isColumnHidden(int columnIndex)
```


Verifica se una colonna all'indice specificato è nascosta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | int | indice della colonna |

**Returns:**
boolean - true se la colonna è nascosta.
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


Indica che l'altezza della riga e l'altezza predefinita del carattere corrispondono.

**Returns:**
boolean
### isDefaultRowHidden() {#isDefaultRowHidden--}
```
public boolean isDefaultRowHidden()
```


Indica se la riga è nascosta di default.

**Returns:**
boolean
### isDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns) {#isDeletingRangeEnabled-int-int-int-int-}
```
public boolean isDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns)
```


Verifica se l'intervallo può essere eliminato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | int | L'indice della riga iniziale dell'intervallo. |
| startColumn | int | L'indice della colonna iniziale dell'intervallo. |
| totalRows | int | Il numero di righe nell'intervallo. |
| totalColumns | int | Il numero di colonne nell'intervallo. |

**Returns:**
boolean -
### isRowHidden(int rowIndex) {#isRowHidden-int-}
```
public boolean isRowHidden(int rowIndex)
```


Verifica se una riga all'indice specificato è nascosta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int | indice di riga |

**Returns:**
boolean - true se la riga è nascosta
### iterator() {#iterator--}
```
public Iterator iterator()
```


Ottiene l'enumeratore delle celle.

**Remarks**

Durante l'attraversamento degli elementi tramite l'Enumerator restituito, la collezione di celle non dovrebbe essere modificata (ad esempio operazioni che creano nuove Cell/Row o eliminano celle/righe esistenti). Altrimenti l'enumeratore potrebbe non riuscire a attraversare correttamente tutte le celle (alcuni elementi potrebbero essere attraversati più volte o saltati).

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
java.util.Iterator - L'enumeratore delle celle
### linkToXmlMap(String mapName, int row, int column, String path) {#linkToXmlMap-java.lang.String-int-int-java.lang.String-}
```
public void linkToXmlMap(String mapName, int row, int column, String path)
```


Collegamento a una mappa XML.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| mapName | java.lang.String | nome della mappa xml |
| riga | int | riga della cella di destinazione |
| colonna | int | colonna della cella di destinazione |
| percorso | java.lang.String | percorso dell'elemento xml nella mappa xml |

### merge(int firstRow, int firstColumn, int totalRows, int totalColumns) {#merge-int-int-int-int-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Unisce un intervallo specificato di celle in una singola cella.

**Remarks**

Fai riferimento alla cella unita tramite l'indirizzo della cella in alto a sinistra nell'intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstRow | int | Prima riga di questo intervallo(basato su zero) |
| firstColumn | int | Prima colonna di questo intervallo(basato su zero) |
| totalRows | int | Numero di righe(basato su uno) |
| totalColumns | int | Numero di colonne (basato su 1) |

### merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean mergeConflict) {#merge-int-int-int-int-boolean-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean mergeConflict)
```


Unisce un intervallo specificato di celle in una singola cella.

**Remarks**

Fai riferimento alla cella unita tramite l'indirizzo della cella in alto a sinistra dell'intervallo. Se mergeConflict è true e l'intervallo unito entra in conflitto con altre celle unite, le altre celle unite verranno rimosse automaticamente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstRow | int | Prima riga di questo intervallo(basato su zero) |
| firstColumn | int | Prima colonna di questo intervallo(basato su zero) |
| totalRows | int | Numero di righe(basato su uno) |
| totalColumns | int | Numero di colonne (basato su 1) |
| mergeConflict | boolean | Intervalli uniti in conflitto di merge. |

### merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean checkConflict, boolean mergeConflict) {#merge-int-int-int-int-boolean-boolean-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean checkConflict, boolean mergeConflict)
```


Unisce un intervallo specificato di celle in una singola cella.

**Remarks**

Fai riferimento alla cella unita tramite l'indirizzo della cella in alto a sinistra dell'intervallo. Se mergeConflict è true e l'intervallo unito entra in conflitto con altre celle unite, le altre celle unite verranno rimosse automaticamente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstRow | int | Prima riga di questo intervallo(basato su zero) |
| firstColumn | int | Prima colonna di questo intervallo(basato su zero) |
| totalRows | int | Numero di righe(basato su uno) |
| totalColumns | int | Numero di colonne (basato su 1) |
| checkConflict | boolean | Indica se verificare se le celle unite si intersecano con altre celle unite |
| mergeConflict | boolean | Intervalli uniti in conflitto di merge. |

### moveRange(CellArea sourceArea, int destRow, int destColumn) {#moveRange-com.aspose.cells.CellArea-int-int-}
```
public void moveRange(CellArea sourceArea, int destRow, int destColumn)
```


Sposta l'intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceArea | [CellArea](../../com.aspose.cells/cellarea) | L'intervallo che dovrebbe essere spostato. |
| destRow | int | La riga di destinazione. |
| destColumn | int | La colonna di destinazione. |

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


Rimuove le righe duplicate nel foglio.

### removeDuplicates(int startRow, int startColumn, int endRow, int endColumn) {#removeDuplicates-int-int-int-int-}
```
public void removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)
```


Rimuove i valori duplicati nell'intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | int | Riga di inizio. |
| startColumn | int | Colonna di inizio |
| endRow | int | L'indice della riga finale. |
| endColumn | int | L'indice della colonna finale. |

### removeDuplicates(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders, int[] columnOffsets) {#removeDuplicates-int-int-int-int-boolean-int---}
```
public void removeDuplicates(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders, int[] columnOffsets)
```


Rimuove i dati duplicati dell'intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | int | Riga di inizio. |
| startColumn | int | Colonna di inizio |
| endRow | int | L'indice della riga finale. |
| endColumn | int | L'indice della colonna finale. |
| hasHeaders | boolean | Indica se l'intervallo contiene intestazioni. |
| columnOffsets | int[] | Gli offset di colonna. |

### removeFormulas() {#removeFormulas--}
```
public void removeFormulas()
```


Rimuove tutte le formule e le sostituisce con il valore della formula.

### retrieveSubtotalSetting(CellArea ca) {#retrieveSubtotalSetting-com.aspose.cells.CellArea-}
```
public SubtotalSetting retrieveSubtotalSetting(CellArea ca)
```


Recupera le impostazioni dei subtotali dell'intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | L'intervallo |

**Returns:**
[SubtotalSetting](../../com.aspose.cells/subtotalsetting) - 
### setColumnWidth(int column, double width) {#setColumnWidth-int-double-}
```
public void setColumnWidth(int column, double width)
```


Imposta la larghezza della colonna specificata nella visualizzazione normale.

**Remarks**

Per i fogli di calcolo, la larghezza della colonna è misurata come il numero di caratteri della larghezza massima delle cifre dei numeri 0~9 così come renderizzati nel carattere dello stile normale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | Indice di colonna. |
| larghezza | double | Larghezza della colonna in unità di caratteri. La larghezza della colonna deve essere compresa tra 0 e 255. |

### setColumnWidthInch(int column, double inches) {#setColumnWidthInch-int-double-}
```
public void setColumnWidthInch(int column, double inches)
```


Imposta la larghezza della colonna in unità di pollici nella visualizzazione normale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | Indice di colonna. |
| pollici | double | Numero di pollici. |

### setColumnWidthPixel(int column, int pixels) {#setColumnWidthPixel-int-int-}
```
public void setColumnWidthPixel(int column, int pixels)
```


Imposta la larghezza della colonna in unità di pixel nella visualizzazione normale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | Indice di colonna. |
| pixel | int | Numero di pixel. |

### setDefaultColumnHidden(boolean value) {#setDefaultColumnHidden-boolean-}
```
public void setDefaultColumnHidden(boolean value)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setDefaultRowHeightMatched(boolean value) {#setDefaultRowHeightMatched-boolean-}
```
public void setDefaultRowHeightMatched(boolean value)
```


Indica che l'altezza della riga e l'altezza predefinita del carattere corrispondono.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setDefaultRowHidden(boolean value) {#setDefaultRowHidden-boolean-}
```
public void setDefaultRowHidden(boolean value)
```


Indica se la riga è nascosta di default.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


Imposta l'opzione di utilizzo della memoria per queste celle.

Vedi [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Limiti notevoli e operazioni consigliate per alcune modalità:

| Modalità | Osservazioni | Supportato |
| ------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
| [MemorySetting.MEMORY\_PREFERENCE](../../com.aspose.cells/memorysetting\#MEMORY-PREFERENCE) | Cells data will be maintained in compact format to decrease the memory cost. On other hand, the compact data also may cause higher time cost, especially when updating the cells data, or accessing cells/rows randomly | v8.0.0 |
|  | [MemorySetting.FILE\_CACHE](../../com.aspose.cells/memorysetting\#FILE-CACHE) | Quando questa modalità è usata per qualsiasi foglio di lavoro in una cartella di lavoro, [Workbook.dispose()](../../com.aspose.cells/workbook\#dispose--) dovrebbe essere chiamato alla fine del lavoro per rilasciare tutte le risorse, come i file temporanei. |
 
L'accesso casuale alle celle comporta scarse prestazioni perché i dati devono essere letti/aggiornati in modo casuale e ripetuto (così il puntatore nel file verrà modificato di conseguenza e saranno necessarie operazioni di I/O ripetute). Se possibile, accedi sempre ai dati in modo sequenziale (riga per riga).
 
Quando i dati di una riga/cella vengono modificati, i dati di altre celle/righe possono essere influenzati (ad esempio i dati vengono spostati/trasferiti altrove per allocare spazio sufficiente per i dati modificati). Pertanto ogni modifica richiede la sincronizzazione con gli altri oggetti esistenti (come l'oggetto Row o Cell). Per ottenere migliori prestazioni, non mantenere più righe/celle contemporaneamente. Elaborarle una alla volta ridurrà la sincronizzazione dei dati, migliorando leggermente le prestazioni. | v25.7     |

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMultiThreadReading(boolean value) {#setMultiThreadReading-boolean-}
```
public void setMultiThreadReading(boolean value)
```


Imposta se il modello dati delle celle deve supportare la lettura Multi-Thread. Il valore predefinito di questa proprietà è false.

**Remarks**

Se ci sono più thread che leggono oggetti Row/Cell in questa collezione contemporaneamente, questa proprietà dovrebbe essere impostata su true, altrimenti potrebbero verificarsi risultati inattesi. Supportare la lettura Multi-Thread può degradare le prestazioni per l'accesso agli oggetti Row/Cell da questa collezione. Si prega di notare che alcune funzionalità non possono supportare la lettura Multi-Thread, come la formattazione dei valori (tramite [Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--), [Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), ecc.). Quindi, anche con questa proprietà impostata su true, quelle API potrebbero comunque dare risultati inattesi per la lettura Multi-Thread.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setPreserveString(boolean value) {#setPreserveString-boolean-}
```
public void setPreserveString(boolean value)
```


Imposta un valore che indica se tutti i valori del foglio di lavoro sono conservati come stringhe. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setRowHeight(int row, double height) {#setRowHeight-int-double-}
```
public void setRowHeight(int row, double height)
```


Imposta l'altezza della riga specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice di riga. |
| altezza | double | Altezza della riga. In unità di punto deve essere compresa tra 0 e 409,5. |

### setRowHeightInch(int row, double inches) {#setRowHeightInch-int-double-}
```
public void setRowHeightInch(int row, double inches)
```


Imposta l'altezza della riga in unità di pollici.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice di riga. |
| pollici | double | Numero di pollici. Deve essere compreso tra 0 e 409,5/72. |

### setRowHeightPixel(int row, int pixels) {#setRowHeightPixel-int-int-}
```
public void setRowHeightPixel(int row, int pixels)
```


Imposta l'altezza della riga in unità di pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice di riga. |
| pixel | int | Numero di pixel. |

### setStandardHeight(double value) {#setStandardHeight-double-}
```
public void setStandardHeight(double value)
```


Imposta l'altezza predefinita della riga in questo foglio di lavoro, in unità di punti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setStandardHeightInch(double value) {#setStandardHeightInch-double-}
```
public void setStandardHeightInch(double value)
```


Imposta l'altezza predefinita della riga in questo foglio di lavoro, in unità di pollici.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setStandardHeightPixels(int value) {#setStandardHeightPixels-int-}
```
public void setStandardHeightPixels(int value)
```


Imposta l'altezza predefinita della riga in questo foglio di lavoro, in unità di pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setStandardWidth(double value) {#setStandardWidth-double-}
```
public void setStandardWidth(double value)
```


Imposta la larghezza predefinita della colonna nel foglio di lavoro, in unità di caratteri.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setStandardWidthInch(double value) {#setStandardWidthInch-double-}
```
public void setStandardWidthInch(double value)
```


Imposta la larghezza predefinita della colonna nel foglio di lavoro, in unità di pollici.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setStandardWidthPixels(int value) {#setStandardWidthPixels-int-}
```
public void setStandardWidthPixels(int value)
```


Imposta la larghezza predefinita della colonna nel foglio di lavoro, in unità di pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setStyle(Style value) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style value)
```


Imposta lo stile predefinito del foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setViewColumnWidthPixel(int column, int pixels) {#setViewColumnWidthPixel-int-int-}
```
public void setViewColumnWidthPixel(int column, int pixels)
```


Imposta la larghezza della colonna in diverse visualizzazioni.

**Remarks**

Se il tipo di visualizzazione corrente è [ViewType.PAGE\_LAYOUT\_VIEW](../../com.aspose.cells/viewtype\#PAGE-LAYOUT-VIEW), la larghezza della colonna è la stessa della larghezza stampata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | L'indice della colonna. |
| pixel | int | La larghezza in unità di pixel. |

### showGroupDetail(boolean isVertical, int index) {#showGroupDetail-boolean-int-}
```
public void showGroupDetail(boolean isVertical, int index)
```


Espande le righe/colonne raggruppate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isVertical | boolean | True, espande le righe raggruppate. |
| indice | int | L'indice riga/colonna |

### subtotal(CellArea ca, int groupBy, int function, int[] totalList) {#subtotal-com.aspose.cells.CellArea-int-int-int---}
```
public void subtotal(CellArea ca, int groupBy, int function, int[] totalList)
```


Crea subtotali per l'intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | L'intervallo |
| groupBy | int | Il campo da raggruppare, come offset intero a base zero |
| function | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). La funzione di subtotale. |
| totalList | int[] | Un array di offset di campo a base zero, che indica i campi a cui vengono aggiunti i subtotali. |

### subtotal(CellArea ca, int groupBy, int function, int[] totalList, boolean replace, boolean pageBreaks, boolean summaryBelowData) {#subtotal-com.aspose.cells.CellArea-int-int-int---boolean-boolean-boolean-}
```
public void subtotal(CellArea ca, int groupBy, int function, int[] totalList, boolean replace, boolean pageBreaks, boolean summaryBelowData)
```


Crea subtotali per l'intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | L'intervallo |
| groupBy | int | Il campo da raggruppare, come offset intero a base zero |
| function | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). La funzione di subtotale. |
| totalList | int[] | Un array di offset di campo a base zero, che indica i campi a cui vengono aggiunti i subtotali. |
| replace | boolean | Indica se sostituire i subtotali attuali |
| pageBreaks | boolean | Indica se aggiungere un'interruzione di pagina tra i gruppi |
| summaryBelowData | boolean | Indica se aggiungere un riepilogo sotto i dati. |

### textToColumns(int row, int column, int totalRows, TxtLoadOptions options) {#textToColumns-int-int-int-com.aspose.cells.TxtLoadOptions-}
```
public int textToColumns(int row, int column, int totalRows, TxtLoadOptions options)
```


Divide il contenuto nella colonna specificata in più colonne..

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | L'indice della riga. |
| colonna | int | L'indice della colonna. |
| totalRows | int | Numero di righe. |
| options | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | Le opzioni di divisione. |

**Returns:**
int - Conteggio totale delle colonne dei valori divisi.
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


Separa un intervallo specificato di celle unite.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstRow | int | Prima riga di questo intervallo(basato su zero) |
| firstColumn | int | Prima colonna di questo intervallo(basato su zero) |
| totalRows | int | Numero di righe(basato su uno) |
| totalColumns | int | Numero di colonne (basato su 1) |

### ungroupColumns(int firstIndex, int lastIndex) {#ungroupColumns-int-int-}
```
public void ungroupColumns(int firstIndex, int lastIndex)
```


Separa le colonne.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstIndex | int | Il primo indice di colonna da separare. |
| lastIndex | int | L'ultimo indice di colonna da separare. |

### ungroupRows(int firstIndex, int lastIndex) {#ungroupRows-int-int-}
```
public void ungroupRows(int firstIndex, int lastIndex)
```


Separa le righe.

**Remarks**

Rimuove solo le informazioni del gruppo esterno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstIndex | int | Il primo indice di riga da separare. |
| lastIndex | int | L'ultimo indice di riga da separare. |

### ungroupRows(int firstIndex, int lastIndex, boolean isAll) {#ungroupRows-int-int-boolean-}
```
public void ungroupRows(int firstIndex, int lastIndex, boolean isAll)
```


Separa le righe.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstIndex | int | Il primo indice di riga da separare. |
| lastIndex | int | L'ultimo indice di riga da separare. |
| isAll | boolean | True, rimuove tutte le informazioni raggruppate. Altrimenti, rimuove le informazioni del gruppo esterno. |

### unhideColumn(int column, double width) {#unhideColumn-int-double-}
```
public void unhideColumn(int column, double width)
```


Rivela una colonna

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | Indice di colonna. |
| larghezza | double | Larghezza colonna. |

### unhideColumns(int column, int totalColumns, double width) {#unhideColumns-int-int-double-}
```
public void unhideColumns(int column, int totalColumns, double width)
```


Rivela più colonne.

**Remarks**

Applica la larghezza della colonna solo alle colonne nascoste.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | Indice di colonna. |
| totalColumns | int | Numero colonna |
| larghezza | double | Larghezza colonna. |

### unhideRow(int row, double height) {#unhideRow-int-double-}
```
public void unhideRow(int row, double height)
```


Rivela una riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice di riga. |
| altezza | double | Altezza riga. L'altezza della riga verrà modificata solo quando la riga è nascosta e il valore di altezza fornito è positivo. |

### unhideRows(int row, int totalRows, double height) {#unhideRows-int-int-double-}
```
public void unhideRows(int row, int totalRows, double height)
```


Rivela le righe nascoste.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | L'indice della riga. |
| totalRows | int | Il numero di riga. |
| altezza | double | Altezza riga. L'altezza della riga verrà modificata solo quando la riga è nascosta e il valore di altezza fornito è positivo. |

### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

