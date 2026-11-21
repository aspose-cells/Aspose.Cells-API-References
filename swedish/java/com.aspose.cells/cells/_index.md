---
title: "Cells"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar en samling av cellrelaterade objekt såsom   ...etc."
type: docs
url: /sv/java/com.aspose.cells/cells/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Cells implements Iterable
```

Inkapslar en samling av cellrelaterade objekt, såsom [Cell](../../com.aspose.cells/cell), [Row](../../com.aspose.cells/row), ...etc.

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
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addRange(Range rangeObject)](#addRange-com.aspose.cells.Range-) | Lägger till en referens till ett intervallobjekt i celler |
| [applyColumnStyle(int column, Style style, StyleFlag flag)](#applyColumnStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Tillämpar format för en hel kolumn. |
| [applyRowStyle(int row, Style style, StyleFlag flag)](#applyRowStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Tillämpar format för en hel rad. |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Tillämpar format för ett helt arbetsblad. |
| [checkCell(int row, int column)](#checkCell-int-int-) | Hämtar [Cell](../../com.aspose.cells/cell)-elementet eller null på det angivna cellradindexet och kolumnindexet. |
| [checkColumn(int columnIndex)](#checkColumn-int-) | Hämtar [Column](../../com.aspose.cells/column)-elementet eller null på det angivna kolumnindexet. |
| [checkRow(int row)](#checkRow-int-) | Hämtar [Row](../../com.aspose.cells/row)-elementet eller null på det angivna cellradindexet. |
| [clear()](#clear--) | Rensar all data i arbetsbladet. |
| [clearContents(CellArea range)](#clearContents-com.aspose.cells.CellArea-) | Rensar innehållet i ett intervall. |
| [clearContents(int startRow, int startColumn, int endRow, int endColumn)](#clearContents-int-int-int-int-) | Rensar innehållet i ett intervall. |
| [clearFormats(CellArea range)](#clearFormats-com.aspose.cells.CellArea-) | Rensar formatering av ett intervall. |
| [clearFormats(int startRow, int startColumn, int endRow, int endColumn)](#clearFormats-int-int-int-int-) | Rensar formatering av ett intervall. |
| [clearMergedCells()](#clearMergedCells--) | Rensar alla sammanslagna intervall. |
| [clearRange(CellArea range)](#clearRange-com.aspose.cells.CellArea-) | Rensar innehåll och formatering av ett intervall. |
| [clearRange(int startRow, int startColumn, int endRow, int endColumn)](#clearRange-int-int-int-int-) | Rensar innehåll och formatering av ett intervall. |
| [convertStringToNumericValue()](#convertStringToNumericValue--) | Konverterar all strängdata i arbetsbladet till numeriskt värde om möjligt. |
| [copyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex)](#copyColumn-com.aspose.cells.Cells-int-int-) | Kopierar data och format för en hel kolumn. |
| [copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)](#copyColumns-com.aspose.cells.Cells-int-int-int-) | Kopierar data och format för hela kolumner. |
| [copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber, PasteOptions pasteOptions)](#copyColumns-com.aspose.cells.Cells-int-int-int-com.aspose.cells.PasteOptions-) | Kopierar data och format för en hel kolumn. |
| [copyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, int destinationColumnIndex, int destinationTotalColumns)](#copyColumns-com.aspose.cells.Cells-int-int-int-int-) | Kopierar data och format för hela kolumnerna. |
| [copyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex)](#copyRow-com.aspose.cells.Cells-int-int-) | Kopierar data och format för en hel rad. |
| [copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)](#copyRows-com.aspose.cells.Cells-int-int-int-) | Kopierar data och format för vissa hela rader. |
| [copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions)](#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-) | Kopierar data och format för vissa hela rader. |
| [copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)](#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-com.aspose.cells.PasteOptions-) | Kopierar data och format för vissa hela rader. |
| [createRange(int firstIndex, int number, boolean isVertical)](#createRange-int-int-boolean-) | Skapar ett [Range](../../com.aspose.cells/range)-objekt från rader med celler eller kolumner med celler. |
| [createRange(int firstRow, int firstColumn, int totalRows, int totalColumns)](#createRange-int-int-int-int-) | Skapar ett [Range](../../com.aspose.cells/range)-objekt från ett cellområde. |
| [createRange(String address)](#createRange-java.lang.String-) | Skapar ett [Range](../../com.aspose.cells/range)-objekt från en adress för området. |
| [createRange(String upperLeftCell, String lowerRightCell)](#createRange-java.lang.String-java.lang.String-) | Skapar ett [Range](../../com.aspose.cells/range)-objekt från ett cellområde. |
| [deleteBlankColumns()](#deleteBlankColumns--) | Ta bort alla tomma kolumner som inte innehåller någon data. |
| [deleteBlankColumns(DeleteOptions options)](#deleteBlankColumns-com.aspose.cells.DeleteOptions-) | Ta bort alla tomma kolumner som inte innehåller någon data. |
| [deleteBlankRows()](#deleteBlankRows--) | Ta bort alla tomma rader som inte innehåller någon data eller annat objekt. |
| [deleteBlankRows(DeleteOptions options)](#deleteBlankRows-com.aspose.cells.DeleteOptions-) | Ta bort alla tomma rader som inte innehåller någon data eller vissa speciella objekt såsom synlig kommentar, pivottabell. |
| [deleteColumn(int columnIndex)](#deleteColumn-int-) | Tar bort en kolumn. |
| [deleteColumn(int columnIndex, boolean updateReference)](#deleteColumn-int-boolean-) | Tar bort en kolumn. |
| [deleteColumns(int columnIndex, int totalColumns, boolean updateReference)](#deleteColumns-int-int-boolean-) | Tar bort flera kolumner. |
| [deleteColumns(int columnIndex, int totalColumns, DeleteOptions options)](#deleteColumns-int-int-com.aspose.cells.DeleteOptions-) | Tar bort flera kolumner. |
| [deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)](#deleteRange-int-int-int-int-int-) | Tar bort ett cellområde och flyttar celler enligt förskjutningsalternativet. |
| [deleteRow(int rowIndex)](#deleteRow-int-) | Tar bort en rad. |
| [deleteRow(int rowIndex, boolean updateReference)](#deleteRow-int-boolean-) | Tar bort en rad. |
| [deleteRows(int rowIndex, int totalRows)](#deleteRows-int-int-) | Tar bort flera rader. |
| [deleteRows(int rowIndex, int totalRows, boolean updateReference)](#deleteRows-int-int-boolean-) | Tar bort flera rader i kalkylbladet. |
| [deleteRows(int rowIndex, int totalRows, DeleteOptions options)](#deleteRows-int-int-com.aspose.cells.DeleteOptions-) | Tar bort flera rader i kalkylbladet. |
| [dispose()](#dispose--) | Utför applikationsdefinierade uppgifter som är relaterade till att frigöra, släppa eller återställa ohanterade resurser. |
| [endCellInColumn(int columnIndex)](#endCellInColumn-int-) | Hämtar den sista cellen i den här kolumnen. |
| [endCellInColumn(int startRow, int endRow, int startColumn, int endColumn)](#endCellInColumn-int-int-int-int-) | Hämtar den sista cellen med högsta kolumnindex i detta område. |
| [endCellInRow(int rowIndex)](#endCellInRow-int-) | Hämtar den sista cellen i den här raden. |
| [endCellInRow(int startRow, int endRow, int startColumn, int endColumn)](#endCellInRow-int-int-int-int-) | Hämtar den sista cellen med högsta radindex i detta område. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)](#exportArray-int-int-int-int-) | Exporterar data i [Cells](../../com.aspose.cells/cells)-samlingen till ett tvådimensionellt array‑objekt. |
| [exportTypeArray(int firstRow, int firstColumn, int totalRows, int totalColumns)](#exportTypeArray-int-int-int-int-) | Exporterar cellvärdestyp i [Cells](../../com.aspose.cells/cells)-samlingen till ett tvådimensionellt array‑objekt. |
| [find(Object what, Cell previousCell)](#find-java.lang.Object-com.aspose.cells.Cell-) | Hittar cellen som innehåller det angivna objektet. |
| [find(Object what, Cell previousCell, FindOptions findOptions)](#find-java.lang.Object-com.aspose.cells.Cell-com.aspose.cells.FindOptions-) | Hittar cellen som innehåller det angivna objektet. |
| [get(int row, int column)](#get-int-int-) | Hämtar [Cell](../../com.aspose.cells/cell)-elementet vid angivet cellradindex och kolumnindex. |
| [get(String cellName)](#get-java.lang.String-) | Hämtar [Cell](../../com.aspose.cells/cell)-elementet vid det angivna cellnamnet. |
| [getCellDisplayStyle(int row, int column)](#getCellDisplayStyle-int-int-) | Hämta visningsstilen för den angivna cellen. |
| [getCellDisplayStyle(int row, int column, int adjacentBorders)](#getCellDisplayStyle-int-int-int-) | Hämta visningsstilen för den angivna cellen. |
| [getCellStyle(int row, int column)](#getCellStyle-int-int-) | Hämta stilen för den angivna cellen. |
| [getCellsWithPlaceInCellPicture()](#getCellsWithPlaceInCellPicture--) | Hämtar alla celler som innehåller inbäddade bilder. |
| [getClass()](#getClass--) |  |
| [getColumnOriginalWidthPoint(int column)](#getColumnOriginalWidthPoint-int-) | Hämtar den ursprungliga kolumnens höjd i punkt om kolumnen är dold |
| [getColumnWidth(int column)](#getColumnWidth-int-) | Hämtar bredden (i enhet av tecken) för den angivna kolumnen i normal vy |
| [getColumnWidth(int column, boolean isOriginal, int unitType)](#getColumnWidth-int-boolean-int-) | Hämtar kolumnbredden. |
| [getColumnWidthInch(int column)](#getColumnWidthInch-int-) | Hämtar bredden på den angivna kolumnen i normal vy, i tum. |
| [getColumnWidthPixel(int column)](#getColumnWidthPixel-int-) | Hämtar bredden på den angivna kolumnen i normal vy, i pixlar. |
| [getColumnWidthPixel(int column, boolean original)](#getColumnWidthPixel-int-boolean-) | Hämtar bredden på den angivna kolumnen i normal vy, i pixlar. |
| [getColumns()](#getColumns--) | Hämtar samlingen av [Column](../../com.aspose.cells/column)-objekt som representerar de enskilda kolumnerna i detta kalkylblad. |
| [getCount()](#getCount--) | Hämtar det totala antalet instansierade Cell-objekt. |
| [getCountLarge()](#getCountLarge--) | Hämtar det totala antalet instansierade Cell-objekt. |
| [getDependents(boolean isAll, int row, int column)](#getDependents-boolean-int-int-) | Hämta alla celler som refererar till den specifika cellen. |
| [getDependentsInCalculation(int row, int column, boolean recursive)](#getDependentsInCalculation-int-int-boolean-) | Hämtar alla celler vars beräknade resultat beror på en specifik cell. |
| [getFirstCell()](#getFirstCell--) | Hämtar den första cellen i detta kalkylblad. |
| [getFirstDataRow(int column)](#getFirstDataRow-int-) | Hämtar det första radindexet för cellen som innehåller data i den angivna kolumnen. |
| [getGroupedColumnOutlineLevel(int columnIndex)](#getGroupedColumnOutlineLevel-int-) | Hämtar konturnivån (nollbaserad) för kolumnen. |
| [getGroupedRowOutlineLevel(int rowIndex)](#getGroupedRowOutlineLevel-int-) | Hämtar konturnivån (nollbaserad) för raden. |
| [getLastCell()](#getLastCell--) | Hämtar den sista cellen i detta kalkylblad. |
| [getLastDataRow(int column)](#getLastDataRow-int-) | Hämtar det sista radindexet för cellen som innehåller data i den angivna kolumnen. |
| [getMaxColumn()](#getMaxColumn--) | Maximalt kolumnindex för de celler som har instansierats i samlingen (inkluderar inte kolumnen där stil är definierad för hela kolumnen men ingen cell har instansierats i den). |
| [getMaxDataColumn()](#getMaxDataColumn--) | Maximalt kolumnindex för cellen som innehåller data. |
| [getMaxDataRow()](#getMaxDataRow--) | Maximalt radindex för cellen som innehåller data. |
| [getMaxDisplayRange()](#getMaxDisplayRange--) | Hämtar det maximala området som inkluderar data, sammanslagna celler och former. |
| [getMaxGroupedColumnOutlineLevel()](#getMaxGroupedColumnOutlineLevel--) | Hämtar den maximala grupperade kolumnens konturnivå (nollbaserad). |
| [getMaxGroupedRowOutlineLevel()](#getMaxGroupedRowOutlineLevel--) | Hämtar den maximala grupperade radens konturnivå (nollbaserad). |
| [getMaxRow()](#getMaxRow--) | Maximalt radindex för cellen som innehåller data eller stil. |
| [getMemorySetting()](#getMemorySetting--) | Hämtar minnesanvändningsalternativet för dessa celler. |
| [getMergedAreas()](#getMergedAreas--) | Hämtar alla sammanslagna celler. |
| [getMergedCells()](#getMergedCells--) | Hämtar samlingen av sammanslagna celler. |
| [getMinColumn()](#getMinColumn--) | Minimalt kolumnindex för de celler som har instansierats i samlingen (inkluderar inte kolumnen där stil är definierad för hela kolumnen men ingen cell har instansierats i den). |
| [getMinDataColumn()](#getMinDataColumn--) | Minsta kolumnindex för cell som innehåller data. |
| [getMinDataRow()](#getMinDataRow--) | Minsta radindex för cell som innehåller data. |
| [getMinRow()](#getMinRow--) | Minsta radindex för cell som innehåller data eller stil. |
| [getMultiThreadReading()](#getMultiThreadReading--) | Hämtar om cellernas datamodell ska stödja Multi-Thread-läsning. |
| [getOdsCellFields()](#getOdsCellFields--) | Hämtar listan över fält i ods. |
| [getPreserveString()](#getPreserveString--) | Hämtar ett värde som indikerar om alla kalkylbladsvärden bevaras som strängar. |
| [getRanges()](#getRanges--) | Hämtar samlingen av [Range](../../com.aspose.cells/range)-objekt som skapas vid körning. |
| [getRowEnumerator()](#getRowEnumerator--) | Hämtar radernas enumerator. |
| [getRowHeight(int row)](#getRowHeight-int-) | Hämtar höjden på en specificerad rad, i enheten punkter. |
| [getRowHeight(int row, boolean isOriginal, int unitType)](#getRowHeight-int-boolean-int-) | Hämtar radens höjd. |
| [getRowHeightInch(int row)](#getRowHeightInch-int-) | Hämtar höjden på en specificerad rad i enheten tum. |
| [getRowHeightPixel(int row)](#getRowHeightPixel-int-) | Hämtar höjden på en specificerad rad i enheten pixel. |
| [getRowOriginalHeightPoint(int row)](#getRowOriginalHeightPoint-int-) | Hämtar den ursprungliga radens höjd i enheten punkt om raden är dold. |
| [getRows()](#getRows--) | Hämtar samlingen av [Row](../../com.aspose.cells/row)-objekt som representerar de enskilda raderna i detta kalkylblad. |
| [getStandardHeight()](#getStandardHeight--) | Hämtar standardradens höjd i detta kalkylblad, i enheten punkter. |
| [getStandardHeightInch()](#getStandardHeightInch--) | Hämtar standardradens höjd i detta kalkylblad, i enheten tum. |
| [getStandardHeightPixels()](#getStandardHeightPixels--) | Hämtar standardradens höjd i detta kalkylblad, i enheten pixlar. |
| [getStandardWidth()](#getStandardWidth--) | Hämtar standardkolumnens bredd i kalkylbladet, i enheten tecken. |
| [getStandardWidthInch()](#getStandardWidthInch--) | Hämtar standardkolumnens bredd i kalkylbladet, i enheten tum. |
| [getStandardWidthPixels()](#getStandardWidthPixels--) | Hämtar standardkolumnens bredd i kalkylbladet, i enheten pixlar. |
| [getStyle()](#getStyle--) | Hämtar standardstilen för kalkylbladet. |
| [getViewColumnWidthPixel(int column)](#getViewColumnWidthPixel-int-) | Hämta bredden i olika vystyper. |
| [getViewRowHeight(int row)](#getViewRowHeight-int-) | Hämtar höjden på en specificerad rad. |
| [getViewRowHeightInch(int row)](#getViewRowHeightInch-int-) | Hämtar höjden på en specificerad rad i enheten tum. |
| [groupColumns(int firstIndex, int lastIndex)](#groupColumns-int-int-) | Grupperar kolumner. |
| [groupColumns(int firstIndex, int lastIndex, boolean isHidden)](#groupColumns-int-int-boolean-) | Grupperar kolumner. |
| [groupRows(int firstIndex, int lastIndex)](#groupRows-int-int-) | Grupperar rader. |
| [groupRows(int firstIndex, int lastIndex, boolean isHidden)](#groupRows-int-int-boolean-) | Grupperar rader. |
| [hashCode()](#hashCode--) |  |
| [hideColumn(int column)](#hideColumn-int-) | Döljer en kolumn. |
| [hideColumns(int column, int totalColumns)](#hideColumns-int-int-) | Dölj flera kolumner. |
| [hideGroupDetail(boolean isVertical, int index)](#hideGroupDetail-boolean-int-) | Komprimerar de grupperade raderna/kolumnerna. |
| [hideRow(int row)](#hideRow-int-) | Döljer en rad. |
| [hideRows(int row, int totalRows)](#hideRows-int-int-) | Dölj flera rader. |
| [importArray(double[] doubleArray, int firstRow, int firstColumn, boolean isVertical)](#importArray-double---int-int-boolean-) | Importerar en array av double till ett kalkylblad. |
| [importArray(double[][] doubleArray, int firstRow, int firstColumn)](#importArray-double-----int-int-) | Importerar en tvådimensionell array av double till ett kalkylblad. |
| [importArray(int[] intArray, int firstRow, int firstColumn, boolean isVertical)](#importArray-int---int-int-boolean-) | Importerar en array av integer till ett kalkylblad. |
| [importArray(int[][] intArray, int firstRow, int firstColumn)](#importArray-int-----int-int-) | Importerar en tvådimensionell array av integer till ett kalkylblad. |
| [importArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)](#importArray-java.lang.String---int-int-boolean-) | Importerar en array av string till ett kalkylblad. |
| [importArray(String[][] stringArray, int firstRow, int firstColumn)](#importArray-java.lang.String-----int-int-) | Importerar en tvådimensionell array av string till ett kalkylblad. |
| [importArrayList(ArrayList arrayList, int firstRow, int firstColumn, boolean isVertical)](#importArrayList-java.util.ArrayList-int-int-boolean-) | Importerar en arraylist av data till ett kalkylblad. |
| [importCSV(InputStream stream, TxtLoadOptions options, int firstRow, int firstColumn)](#importCSV-java.io.InputStream-com.aspose.cells.TxtLoadOptions-int-int-) | Importera en CSV-fil till cellerna. |
| [importCSV(InputStream stream, String splitter, boolean convertNumericData, int firstRow, int firstColumn)](#importCSV-java.io.InputStream-java.lang.String-boolean-int-int-) | Importera en CSV-fil till cellerna. |
| [importCSV(String fileName, TxtLoadOptions options, int firstRow, int firstColumn)](#importCSV-java.lang.String-com.aspose.cells.TxtLoadOptions-int-int-) | Importera en CSV-fil till cellerna. |
| [importCSV(String fileName, String splitter, boolean convertNumericData, int firstRow, int firstColumn)](#importCSV-java.lang.String-java.lang.String-boolean-int-int-) | Importera en CSV-fil till cellerna. |
| [importCustomObjects(Collection list, int firstRow, int firstColumn, ImportTableOptions options)](#importCustomObjects-java.util.Collection-int-int-com.aspose.cells.ImportTableOptions-) | Importerar anpassade objekt. |
| [importCustomObjects(Collection list, String[] propertyNames, boolean isPropertyNameShown, int firstRow, int firstColumn, int rowNumber, boolean insertRows, String dateFormatString, boolean convertStringToNumber)](#importCustomObjects-java.util.Collection-java.lang.String---boolean-int-int-int-boolean-java.lang.String-boolean-) | Importerar anpassade objekt. |
| [importData(ICellsDataTable table, int firstRow, int firstColumn, ImportTableOptions options)](#importData-com.aspose.cells.ICellsDataTable-int-int-com.aspose.cells.ImportTableOptions-) | Importera data från en anpassad datatabell. |
| [importFormulaArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)](#importFormulaArray-java.lang.String---int-int-boolean-) | Importerar en array av formel till ett kalkylblad. |
| [importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical)](#importObjectArray-java.lang.Object---int-int-boolean-) | Importerar en array av data till ett kalkylblad. |
| [importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical, int skip)](#importObjectArray-java.lang.Object---int-int-boolean-int-) | Importerar en array av data till ett kalkylblad. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-int-int-boolean-) | Importerar data i ett ResultSet-objekt till kalkylbladet. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)](#importResultSet-java.sql.ResultSet-int-int-boolean-java.lang.String-boolean-) | Importerar data i ett ResultSet-objekt till kalkylbladet. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, ImportTableOptions options)](#importResultSet-java.sql.ResultSet-int-int-com.aspose.cells.ImportTableOptions-) | Importerar data i ett ResultSet-objekt till kalkylbladet. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-) | Importerar data i ett ResultSet-objekt till kalkylbladet. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)](#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-java.lang.String-boolean-) | Importerar data i ett ResultSet-objekt till kalkylbladet. |
| [importResultSet(ResultSet rs, String startCell, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-java.lang.String-boolean-) | Importerar data i ett ResultSet-objekt till kalkylbladet. |
| [importResultSet(ResultSet rs, String startCell, ImportTableOptions options)](#importResultSet-java.sql.ResultSet-java.lang.String-com.aspose.cells.ImportTableOptions-) | Importerar data i ett ResultSet-objekt till kalkylbladet. |
| [importResultSet(ResultSet rs, String startCell, int rowNum, int columnNum, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-java.lang.String-int-int-boolean-) | Importerar data i ett ResultSet-objekt till kalkylbladet. |
| [importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn)](#importTwoDimensionArray-java.lang.Object-----int-int-) | Importerar en tvådimensionell array av data till ett kalkylblad. |
| [importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn, boolean convertStringToNumber)](#importTwoDimensionArray-java.lang.Object-----int-int-boolean-) | Importerar en tvådimensionell array av data till ett kalkylblad. |
| [importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, boolean convertStringToNumber)](#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-boolean-) | Importerar en tvådimensionell array av data till ett kalkylblad. |
| [importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, TxtLoadOptions opts)](#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-com.aspose.cells.TxtLoadOptions-) | Importerar en tvådimensionell array av data till ett kalkylblad. |
| [insertColumn(int columnIndex)](#insertColumn-int-) | Infogar en ny kolumn i kalkylbladet. |
| [insertColumn(int columnIndex, boolean updateReference)](#insertColumn-int-boolean-) | Infogar en ny kolumn i kalkylbladet. |
| [insertColumns(int columnIndex, int totalColumns)](#insertColumns-int-int-) | Infogar några kolumner i kalkylbladet. |
| [insertColumns(int columnIndex, int totalColumns, boolean updateReference)](#insertColumns-int-int-boolean-) | Infogar några kolumner i kalkylbladet. |
| [insertColumns(int columnIndex, int totalColumns, InsertOptions options)](#insertColumns-int-int-com.aspose.cells.InsertOptions-) | Infogar några kolumner i kalkylbladet. |
| [insertCutCells(Range cutRange, int row, int column, int shiftType)](#insertCutCells-com.aspose.cells.Range-int-int-int-) | Infoga klippt område. |
| [insertRange(CellArea area, int shiftType)](#insertRange-com.aspose.cells.CellArea-int-) | Infogar ett cellområde och flyttar celler enligt förskjutningsalternativet. |
| [insertRange(CellArea area, int shiftNumber, int shiftType)](#insertRange-com.aspose.cells.CellArea-int-int-) | Infogar ett cellområde och flyttar celler enligt förskjutningsalternativet. |
| [insertRange(CellArea area, int shiftNumber, int shiftType, boolean updateReference)](#insertRange-com.aspose.cells.CellArea-int-int-boolean-) | Infogar ett cellområde och flyttar celler enligt förskjutningsalternativet. |
| [insertRow(int rowIndex)](#insertRow-int-) | Infogar en ny rad i kalkylbladet. |
| [insertRows(int rowIndex, int totalRows)](#insertRows-int-int-) | Infogar flera rader i kalkylbladet. |
| [insertRows(int rowIndex, int totalRows, boolean updateReference)](#insertRows-int-int-boolean-) | Infogar flera rader i kalkylbladet. |
| [insertRows(int rowIndex, int totalRows, InsertOptions options)](#insertRows-int-int-com.aspose.cells.InsertOptions-) | Infogar flera rader i kalkylbladet. |
| [isBlankColumn(int columnIndex)](#isBlankColumn-int-) | Kontrollerar om given kolumn är tom (innehåller ingen data). |
| [isColumnHidden(int columnIndex)](#isColumnHidden-int-) | Kontrollerar om en kolumn på angivet index är dold. |
| [isDefaultColumnHidden()](#isDefaultColumnHidden--) |  |
| [isDefaultRowHeightMatched()](#isDefaultRowHeightMatched--) | Indikerar att radhöjd och standardteckensnittshöjd matchar |
| [isDefaultRowHidden()](#isDefaultRowHidden--) | Indikerar om raden är standarddolt. |
| [isDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns)](#isDeletingRangeEnabled-int-int-int-int-) | Kontrollera om området kan tas bort. |
| [isRowHidden(int rowIndex)](#isRowHidden-int-) | Kontrollerar om en rad på angivet index är dold. |
| [iterator()](#iterator--) | Hämtar cellernas enumerator. |
| [linkToXmlMap(String mapName, int row, int column, String path)](#linkToXmlMap-java.lang.String-int-int-java.lang.String-) | Länk till en XML-karta. |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#merge-int-int-int-int-) | Slår ihop ett angivet cellområde till en enda cell. |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean mergeConflict)](#merge-int-int-int-int-boolean-) | Slår ihop ett angivet cellområde till en enda cell. |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean checkConflict, boolean mergeConflict)](#merge-int-int-int-int-boolean-boolean-) | Slår ihop ett angivet cellområde till en enda cell. |
| [moveRange(CellArea sourceArea, int destRow, int destColumn)](#moveRange-com.aspose.cells.CellArea-int-int-) | Flyttar området. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeDuplicates()](#removeDuplicates--) | Tar bort dubblett rader i bladet. |
| [removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)](#removeDuplicates-int-int-int-int-) | Tar bort dubblettvärden i området. |
| [removeDuplicates(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders, int[] columnOffsets)](#removeDuplicates-int-int-int-int-boolean-int---) | Tar bort dubblettdata i området. |
| [removeFormulas()](#removeFormulas--) | Tar bort alla formler och ersätter dem med formelns värde. |
| [retrieveSubtotalSetting(CellArea ca)](#retrieveSubtotalSetting-com.aspose.cells.CellArea-) | Hämtar delsummeinställningarna för området. |
| [setColumnWidth(int column, double width)](#setColumnWidth-int-double-) | Ställer in bredden på den angivna kolumnen i normal vy. |
| [setColumnWidthInch(int column, double inches)](#setColumnWidthInch-int-double-) | Ställer in kolumnbredd i tum i normal vy. |
| [setColumnWidthPixel(int column, int pixels)](#setColumnWidthPixel-int-int-) | Ställer in kolumnbredd i pixlar i normal vy. |
| [setDefaultColumnHidden(boolean value)](#setDefaultColumnHidden-boolean-) |  |
| [setDefaultRowHeightMatched(boolean value)](#setDefaultRowHeightMatched-boolean-) | Indikerar att radhöjd och standardteckensnittshöjd matchar |
| [setDefaultRowHidden(boolean value)](#setDefaultRowHidden-boolean-) | Indikerar om raden är standarddolt. |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Ställer in minnesanvändningsalternativet för dessa celler. |
| [setMultiThreadReading(boolean value)](#setMultiThreadReading-boolean-) | Ställer in om cellernas datamodell ska stödja flertrådad läsning. |
| [setPreserveString(boolean value)](#setPreserveString-boolean-) | Ställer in ett värde som indikerar om alla kalkylbladsvärden bevaras som strängar. |
| [setRowHeight(int row, double height)](#setRowHeight-int-double-) | Ställer in höjden på den angivna raden. |
| [setRowHeightInch(int row, double inches)](#setRowHeightInch-int-double-) | Ställer in radhöjd i tum. |
| [setRowHeightPixel(int row, int pixels)](#setRowHeightPixel-int-int-) | Ställer in radhöjd i pixlar. |
| [setStandardHeight(double value)](#setStandardHeight-double-) | Ställer in standardradhöjd i detta kalkylblad, i punktenheter. |
| [setStandardHeightInch(double value)](#setStandardHeightInch-double-) | Ställer in standardradhöjden i detta kalkylblad, i enheten tum. |
| [setStandardHeightPixels(int value)](#setStandardHeightPixels-int-) | Ställer in standardradhöjden i detta kalkylblad, i enheten pixlar. |
| [setStandardWidth(double value)](#setStandardWidth-double-) | Ställer in standardkolumnbredden i kalkylbladet, i enheten tecken. |
| [setStandardWidthInch(double value)](#setStandardWidthInch-double-) | Ställer in standardkolumnbredden i kalkylbladet, i enheten tum. |
| [setStandardWidthPixels(int value)](#setStandardWidthPixels-int-) | Ställer in standardkolumnbredden i kalkylbladet, i enheten pixlar. |
| [setStyle(Style value)](#setStyle-com.aspose.cells.Style-) | Ställer in standardstilen för kalkylbladet. |
| [setViewColumnWidthPixel(int column, int pixels)](#setViewColumnWidthPixel-int-int-) | Ställer in kolumnens bredd i olika vyer. |
| [showGroupDetail(boolean isVertical, int index)](#showGroupDetail-boolean-int-) | Expanderar de grupperade raderna/kolumnerna. |
| [subtotal(CellArea ca, int groupBy, int function, int[] totalList)](#subtotal-com.aspose.cells.CellArea-int-int-int---) | Skapar delsummer för intervallet. |
| [subtotal(CellArea ca, int groupBy, int function, int[] totalList, boolean replace, boolean pageBreaks, boolean summaryBelowData)](#subtotal-com.aspose.cells.CellArea-int-int-int---boolean-boolean-boolean-) | Skapar delsummer för intervallet. |
| [textToColumns(int row, int column, int totalRows, TxtLoadOptions options)](#textToColumns-int-int-int-com.aspose.cells.TxtLoadOptions-) | Delar upp innehållet i angiven kolumn i flera kolumner.. |
| [toString()](#toString--) |  |
| [unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#unMerge-int-int-int-int-) | Tar bort sammanslagning av ett angivet område med sammanslagna celler. |
| [ungroupColumns(int firstIndex, int lastIndex)](#ungroupColumns-int-int-) | Avgrupperar kolumner. |
| [ungroupRows(int firstIndex, int lastIndex)](#ungroupRows-int-int-) | Avgrupperar rader. |
| [ungroupRows(int firstIndex, int lastIndex, boolean isAll)](#ungroupRows-int-int-boolean-) | Avgrupperar rader. |
| [unhideColumn(int column, double width)](#unhideColumn-int-double-) | Visar en kolumn |
| [unhideColumns(int column, int totalColumns, double width)](#unhideColumns-int-int-double-) | Visa flera kolumner. |
| [unhideRow(int row, double height)](#unhideRow-int-double-) | Visar en rad. |
| [unhideRows(int row, int totalRows, double height)](#unhideRows-int-int-double-) | Visar de dolda raderna. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addRange(Range rangeObject) {#addRange-com.aspose.cells.Range-}
```
public void addRange(Range rangeObject)
```


Lägger till en referens till ett intervallobjekt i celler

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rangeObject | [Range](../../com.aspose.cells/range) | Områdesobjektet kommer att finnas i cellerna |

### applyColumnStyle(int column, Style style, StyleFlag flag) {#applyColumnStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyColumnStyle(int column, Style style, StyleFlag flag)
```


Tillämpar format för en hel kolumn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindexet. |
| style | [Style](../../com.aspose.cells/style) | Stilobjektet som kommer att tillämpas. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Flaggor som indikerar tillämpade formateringsegenskaper. |

### applyRowStyle(int row, Style style, StyleFlag flag) {#applyRowStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyRowStyle(int row, Style style, StyleFlag flag)
```


Tillämpar format för en hel rad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindexet. |
| style | [Style](../../com.aspose.cells/style) | Stilobjektet som kommer att tillämpas. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Flaggor som indikerar tillämpade formateringsegenskaper. |

### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Tillämpar format för ett helt arbetsblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Stilobjektet som kommer att tillämpas. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Flaggor som indikerar tillämpade formateringsegenskaper. |

### checkCell(int row, int column) {#checkCell-int-int-}
```
public Cell checkCell(int row, int column)
```


Hämtar [Cell](../../com.aspose.cells/cell)-elementet eller null på det angivna cellradindexet och kolumnindexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex |
| kolumn | int | Kolumnindex |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Return Cell object if a Cell object exists. Return null if the cell does not exist.
### checkColumn(int columnIndex) {#checkColumn-int-}
```
public Column checkColumn(int columnIndex)
```


Hämtar [Column](../../com.aspose.cells/column)-elementet eller null på det angivna kolumnindexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | Kolumnindexet. |

**Returns:**
[Column](../../com.aspose.cells/column) - The Column object.
### checkRow(int row) {#checkRow-int-}
```
public Row checkRow(int row)
```


Hämtar [Row](../../com.aspose.cells/row)-elementet eller null på det angivna cellradindexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex |

**Returns:**
[Row](../../com.aspose.cells/row) - Returns [Row](../../com.aspose.cells/row) object If the row object does exist, otherwise returns null.
### clear() {#clear--}
```
public void clear()
```


Rensar all data i arbetsbladet.

### clearContents(CellArea range) {#clearContents-com.aspose.cells.CellArea-}
```
public void clearContents(CellArea range)
```


Rensar innehållet i ett intervall.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| range | [CellArea](../../com.aspose.cells/cellarea) | Område som ska rensas. |

### clearContents(int startRow, int startColumn, int endRow, int endColumn) {#clearContents-int-int-int-int-}
```
public void clearContents(int startRow, int startColumn, int endRow, int endColumn)
```


Rensar innehållet i ett intervall.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | Startradens index. |
| startColumn | int | Startkolumnens index. |
| slutRad | int | Slutradens index. |
| endColumn | int | Slutkolumnens index. |

### clearFormats(CellArea range) {#clearFormats-com.aspose.cells.CellArea-}
```
public void clearFormats(CellArea range)
```


Rensar formatering av ett intervall.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| range | [CellArea](../../com.aspose.cells/cellarea) | Område som ska rensas. |

### clearFormats(int startRow, int startColumn, int endRow, int endColumn) {#clearFormats-int-int-int-int-}
```
public void clearFormats(int startRow, int startColumn, int endRow, int endColumn)
```


Rensar formatering av ett intervall.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | Startradens index. |
| startColumn | int | Startkolumnens index. |
| slutRad | int | Slutradens index. |
| endColumn | int | Slutkolumnens index. |

### clearMergedCells() {#clearMergedCells--}
```
public void clearMergedCells()
```


Rensar alla sammanslagna intervall.

### clearRange(CellArea range) {#clearRange-com.aspose.cells.CellArea-}
```
public void clearRange(CellArea range)
```


Rensar innehåll och formatering av ett intervall.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| range | [CellArea](../../com.aspose.cells/cellarea) | Område som ska rensas. |

### clearRange(int startRow, int startColumn, int endRow, int endColumn) {#clearRange-int-int-int-int-}
```
public void clearRange(int startRow, int startColumn, int endRow, int endColumn)
```


Rensar innehåll och formatering av ett intervall.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | Startradens index. |
| startColumn | int | Startkolumnens index. |
| slutRad | int | Slutradens index. |
| endColumn | int | Slutkolumnens index. |

### convertStringToNumericValue() {#convertStringToNumericValue--}
```
public void convertStringToNumericValue()
```


Konverterar all strängdata i arbetsbladet till numeriskt värde om möjligt.

### copyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex) {#copyColumn-com.aspose.cells.Cells-int-int-}
```
public void copyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex)
```


Kopierar data och format för en hel kolumn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Källcellobjektet innehåller data och format att kopiera. |
| sourceColumnIndex | int | Källkolumnindex. |
| destinationColumnIndex | int | Destination kolumnindex. |

### copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber) {#copyColumns-com.aspose.cells.Cells-int-int-int-}
```
public void copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)
```


Kopierar data och format för hela kolumner.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Källcellobjektet innehåller data och format att kopiera. |
| sourceColumnIndex | int | Källkolumnindex. |
| destinationColumnIndex | int | Destination kolumnindex. |
| columnNumber | int | Det kopierade kolumnnumret. |

### copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber, PasteOptions pasteOptions) {#copyColumns-com.aspose.cells.Cells-int-int-int-com.aspose.cells.PasteOptions-}
```
public void copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber, PasteOptions pasteOptions)
```


Kopierar data och format för en hel kolumn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Källcellobjektet innehåller data och format att kopiera. |
| sourceColumnIndex | int | Källkolumnindex. |
| destinationColumnIndex | int | Destination kolumnindex. |
| columnNumber | int | Det kopierade kolumnnumret. |
| pasteOptions | [PasteOptions](../../com.aspose.cells/pasteoptions) | alternativen för inklistring. |

### copyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, int destinationColumnIndex, int destinationTotalColumns) {#copyColumns-com.aspose.cells.Cells-int-int-int-int-}
```
public void copyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, int destinationColumnIndex, int destinationTotalColumns)
```


Kopierar data och format för hela kolumnerna.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Källcellobjektet innehåller data och format att kopiera. |
| sourceColumnIndex | int | Källkolumnindex. |
| sourceTotalColumns | int | Antalet källkolumner. |
| destinationColumnIndex | int | Destination kolumnindex. |
| destinationTotalColumns | int | Antalet destinationskolumner. |

### copyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex) {#copyRow-com.aspose.cells.Cells-int-int-}
```
public void copyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex)
```


Kopierar data och format för en hel rad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Källcellobjektet innehåller data och format att kopiera. |
| sourceRowIndex | int | Källradindex. |
| destinationRowIndex | int | Destinationsradindex. |

### copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber) {#copyRows-com.aspose.cells.Cells-int-int-int-}
```
public void copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```


Kopierar data och format för vissa hela rader.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Källcellobjektet innehåller data och format att kopiera. |
| sourceRowIndex | int | Källradindex. |
| destinationRowIndex | int | Destinationsradindex. |
| rowNumber | int | Det kopierade radnumret. |

### copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions) {#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-}
```
public void copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions)
```


Kopierar data och format för vissa hela rader.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Källcellobjektet innehåller data och format att kopiera. |
| sourceRowIndex | int | Källradindex. |
| destinationRowIndex | int | Destinationsradindex. |
| rowNumber | int | Det kopierade radnumret. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Kopieringsalternativen. |

### copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions) {#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-com.aspose.cells.PasteOptions-}
```
public void copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)
```


Kopierar data och format för vissa hela rader.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceCells0 | [Cells](../../com.aspose.cells/cells) | Källcellobjektet innehåller data och format att kopiera. |
| sourceRowIndex | int | Källradindex. |
| destinationRowIndex | int | Destinationsradindex. |
| rowNumber | int | Det kopierade radnumret. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Kopieringsalternativen. |
| pasteOptions | [PasteOptions](../../com.aspose.cells/pasteoptions) | alternativen för inklistring. |

### createRange(int firstIndex, int number, boolean isVertical) {#createRange-int-int-boolean-}
```
public Range createRange(int firstIndex, int number, boolean isVertical)
```


Skapar ett [Range](../../com.aspose.cells/range)-objekt från rader med celler eller kolumner med celler.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstIndex | int | Första radindex eller första kolumnindex, nollbaserat. |
| nummer | int | Totalt antal rader eller kolumner, enbaserat. |
| isVertical | boolean | Sant - Område skapat från cellers kolumner. Falskt - Område skapat från cellers rader. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object.
### createRange(int firstRow, int firstColumn, int totalRows, int totalColumns) {#createRange-int-int-int-int-}
```
public Range createRange(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Skapar ett [Range](../../com.aspose.cells/range)-objekt från ett cellområde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstRow | int | Första rad i detta område |
| firstColumn | int | Första kolumn i detta område |
| totalRows | int | Antal rader |
| totalColumns | int | Antal kolumner |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### createRange(String address) {#createRange-java.lang.String-}
```
public Range createRange(String address)
```


Skapar ett [Range](../../com.aspose.cells/range)-objekt från en adress för området.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| adress | java.lang.String | Adressen för området. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### createRange(String upperLeftCell, String lowerRightCell) {#createRange-java.lang.String-java.lang.String-}
```
public Range createRange(String upperLeftCell, String lowerRightCell)
```


Skapar ett [Range](../../com.aspose.cells/range)-objekt från ett cellområde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| upperLeftCell | java.lang.String | Övre vänstra cellnamn. |
| lowerRightCell | java.lang.String | Nedre högra cellnamn. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### deleteBlankColumns() {#deleteBlankColumns--}
```
public void deleteBlankColumns()
```


Ta bort alla tomma kolumner som inte innehåller någon data.

### deleteBlankColumns(DeleteOptions options) {#deleteBlankColumns-com.aspose.cells.DeleteOptions-}
```
public void deleteBlankColumns(DeleteOptions options)
```


Ta bort alla tomma kolumner som inte innehåller någon data.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | Alternativen för att radera område. |

### deleteBlankRows() {#deleteBlankRows--}
```
public void deleteBlankRows()
```


Ta bort alla tomma rader som inte innehåller någon data eller annat objekt.

### deleteBlankRows(DeleteOptions options) {#deleteBlankRows-com.aspose.cells.DeleteOptions-}
```
public void deleteBlankRows(DeleteOptions options)
```


Ta bort alla tomma rader som inte innehåller någon data eller vissa speciella objekt såsom synlig kommentar, pivottabell.

**Remarks**

För tomma rader som ska raderas krävs det inte bara att [Row.isBlank()](../../com.aspose.cells/row\#isBlank--) är sant, utan också att det inte finns någon synlig kommentar definierad för någon cell i dessa rader, och ingen pivottabell vars område skär dem.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | Alternativen för att radera område. |

### deleteColumn(int columnIndex) {#deleteColumn-int-}
```
public void deleteColumn(int columnIndex)
```


Tar bort en kolumn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | Index för kolumnen som ska raderas. |

### deleteColumn(int columnIndex, boolean updateReference) {#deleteColumn-int-boolean-}
```
public void deleteColumn(int columnIndex, boolean updateReference)
```


Tar bort en kolumn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | Index för kolumnen som ska raderas. |
| updateReference | boolean | Anger om referenser ska uppdateras i andra arbetsblad. |

### deleteColumns(int columnIndex, int totalColumns, boolean updateReference) {#deleteColumns-int-int-boolean-}
```
public void deleteColumns(int columnIndex, int totalColumns, boolean updateReference)
```


Tar bort flera kolumner.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | Index för den första kolumnen som ska raderas. |
| totalColumns | int | Antal kolumner som ska raderas. |
| updateReference | boolean | Anger om referenser ska uppdateras i andra arbetsblad. |

### deleteColumns(int columnIndex, int totalColumns, DeleteOptions options) {#deleteColumns-int-int-com.aspose.cells.DeleteOptions-}
```
public void deleteColumns(int columnIndex, int totalColumns, DeleteOptions options)
```


Tar bort flera kolumner.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | Index för den första kolumnen som ska raderas. |
| totalColumns | int | Antal kolumner som ska raderas. |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | Alternativ för raderingsoperationen |

### deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType) {#deleteRange-int-int-int-int-int-}
```
public void deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)
```


Tar bort ett cellområde och flyttar celler enligt förskjutningsalternativet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | Startradens index. |
| startColumn | int | Startkolumnens index. |
| slutRad | int | Slutradens index. |
| endColumn | int | Slutkolumnens index. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Alternativ för att skifta celler. |

### deleteRow(int rowIndex) {#deleteRow-int-}
```
public void deleteRow(int rowIndex)
```


Tar bort en rad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int | Index för raden som ska raderas. |

### deleteRow(int rowIndex, boolean updateReference) {#deleteRow-int-boolean-}
```
public void deleteRow(int rowIndex, boolean updateReference)
```


Tar bort en rad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int | Index för raden som ska raderas. |
| updateReference | boolean | Anger om referenser ska uppdateras i andra arbetsblad. |

### deleteRows(int rowIndex, int totalRows) {#deleteRows-int-int-}
```
public boolean deleteRows(int rowIndex, int totalRows)
```


Tar bort flera rader.

**Remarks**

Om det raderade området innehåller den övre delen (inte hela) av tabellen (ListObject) kan området inte raderas och inget görs. Det fungerar på samma sätt som i MS Excel.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int | Det första radindexet som ska raderas. |
| totalRows | int | Antal rader som ska raderas. |

**Returns:**
boolean
### deleteRows(int rowIndex, int totalRows, boolean updateReference) {#deleteRows-int-int-boolean-}
```
public boolean deleteRows(int rowIndex, int totalRows, boolean updateReference)
```


Tar bort flera rader i kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int | Index för den första raden som ska raderas. |
| totalRows | int | Antal rader som ska raderas. |
| updateReference | boolean | Anger om referenser ska uppdateras i andra arbetsblad. |

**Returns:**
boolean -
### deleteRows(int rowIndex, int totalRows, DeleteOptions options) {#deleteRows-int-int-com.aspose.cells.DeleteOptions-}
```
public boolean deleteRows(int rowIndex, int totalRows, DeleteOptions options)
```


Tar bort flera rader i kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int | Index för den första raden som ska raderas. |
| totalRows | int | Antal rader som ska raderas. |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | Alternativ för raderingsoperationen |

**Returns:**
boolean -
### dispose() {#dispose--}
```
public void dispose()
```


Utför applikationsdefinierade uppgifter som är relaterade till att frigöra, släppa eller återställa ohanterade resurser.

### endCellInColumn(int columnIndex) {#endCellInColumn-int-}
```
public Cell endCellInColumn(int columnIndex)
```


Hämtar den sista cellen i den här kolumnen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | Kolumnindex. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### endCellInColumn(int startRow, int endRow, int startColumn, int endColumn) {#endCellInColumn-int-int-int-int-}
```
public Cell endCellInColumn(int startRow, int endRow, int startColumn, int endColumn)
```


Hämtar den sista cellen med högsta kolumnindex i detta område.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | Startradens index. |
| slutRad | int | Slutradens index. |
| startColumn | int | Startkolumnens index. |
| endColumn | int | Slutkolumnens index. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### endCellInRow(int rowIndex) {#endCellInRow-int-}
```
public Cell endCellInRow(int rowIndex)
```


Hämtar den sista cellen i den här raden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int | Radindex. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### endCellInRow(int startRow, int endRow, int startColumn, int endColumn) {#endCellInRow-int-int-int-int-}
```
public Cell endCellInRow(int startRow, int endRow, int startColumn, int endColumn)
```


Hämtar den sista cellen med högsta radindex i detta område.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | Startradens index. |
| slutRad | int | Slutradens index. |
| startColumn | int | Startkolumnens index. |
| endColumn | int | Slutkolumnens index. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns) {#exportArray-int-int-int-int-}
```
public Object[][] exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Exporterar data i [Cells](../../com.aspose.cells/cells)-samlingen till ett tvådimensionellt array‑objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstRow | int | Radnumret för den första cellen som ska exporteras. |
| firstColumn | int | Kolumnnumret för den första cellen som ska exporteras. |
| totalRows | int | Antal rader att exportera |
| totalColumns | int | Antal kolumner att exportera |

**Returns:**
java.lang.Object[][] - Exporterat cellvärdesmatrisobjekt.
### exportTypeArray(int firstRow, int firstColumn, int totalRows, int totalColumns) {#exportTypeArray-int-int-int-int-}
```
public int[][] exportTypeArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Exporterar cellvärdestyp i [Cells](../../com.aspose.cells/cells)-samlingen till ett tvådimensionellt array‑objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstRow | int | Radnumret för den första cellen som ska exporteras. |
| firstColumn | int | Kolumnnumret för den första cellen som ska exporteras. |
| totalRows | int | Antal rader att exporteras. |
| totalColumns | int | Antal kolumner att exporteras. |

**Returns:**
int[][] - [CellValueType](../../com.aspose.cells/cellvaluetype). Exporterat matrisobjekt som representerar cellvärdestyper.
### find(Object what, Cell previousCell) {#find-java.lang.Object-com.aspose.cells.Cell-}
```
public Cell find(Object what, Cell previousCell)
```


Hittar cellen som innehåller det angivna objektet.

**Remarks**

Returnerar null (Ingenting) om ingen cell hittas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| vad | java.lang.Object | Objektet att söka efter. Typen bör vara int,double,DateTime,string,bool. |
| previousCell | [Cell](../../com.aspose.cells/cell) | Föregående cell med samma objekt. Denna parameter kan sättas till null om sökningen startas från början. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### find(Object what, Cell previousCell, FindOptions findOptions) {#find-java.lang.Object-com.aspose.cells.Cell-com.aspose.cells.FindOptions-}
```
public Cell find(Object what, Cell previousCell, FindOptions findOptions)
```


Hittar cellen som innehåller det angivna objektet.

**Remarks**

Returnerar null (Ingenting) om ingen cell hittas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| vad | java.lang.Object | Objektet att söka efter. Typen bör vara int,double,DateTime,string,bool. |
| previousCell | [Cell](../../com.aspose.cells/cell) | Föregående cell med samma objekt. Denna parameter kan sättas till null om sökningen startas från början. |
| findOptions | [FindOptions](../../com.aspose.cells/findoptions) | Sökalternativ |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### get(int row, int column) {#get-int-int-}
```
public Cell get(int row, int column)
```


Hämtar [Cell](../../com.aspose.cells/cell)-elementet vid angivet cellradindex och kolumnindex.

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
         Cell cell = cells.get(0, 0);	//Gets the cell at "A1"
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex. |
| kolumn | int | Kolumnindex. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - The [Cell](../../com.aspose.cells/cell) object.
### get(String cellName) {#get-java.lang.String-}
```
public Cell get(String cellName)
```


Hämtar [Cell](../../com.aspose.cells/cell)-elementet vid det angivna cellnamnet.

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
         Cell cell = cells.get("A1");	//Gets the cell at "A1"
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellNamn | java.lang.String | Cellnamn, inklusive dess kolumnbokstav och radnummer, till exempel A5. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - A [Cell](../../com.aspose.cells/cell) object
### getCellDisplayStyle(int row, int column) {#getCellDisplayStyle-int-int-}
```
public Style getCellDisplayStyle(int row, int column)
```


Hämta visningsstilen för den angivna cellen.

**Remarks**

Samma med [Cell.getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--), och samma med att använda [BorderType.SIDE\_BORDERS](../../com.aspose.cells/bordertype\#SIDE-BORDERS) för [getCellDisplayStyle(int,int,int)](../../com.aspose.cells/cells\#getCellDisplayStyle-int-int-int-).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | radindex för given cell |
| kolumn | int | kolumn för given cell |

**Returns:**
[Style](../../com.aspose.cells/style) - the display style of given cell.
### getCellDisplayStyle(int row, int column, int adjacentBorders) {#getCellDisplayStyle-int-int-int-}
```
public Style getCellDisplayStyle(int row, int column, int adjacentBorders)
```


Hämta visningsstilen för den angivna cellen.

**Remarks**

Om cellen också påverkas av andra inställningar såsom villkorsstyrd formatering, listobjekt osv., kan visningsstilen vara annorlunda än [getCellStyle(int,int)](../../com.aspose.cells/cells\#getCellStyle-int-int-). Och eftersom dessa inställningar också kan tillämpas på tomma (icke‑existerande) celler, kan användning av denna metod undvika instansiering av dessa tomma celler så att prestandan blir bättre än att hämta Cell‑instansen från Cells och sedan anropa [Cell.getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | radindex för given cell |
| kolumn | int | kolumn för given cell |
| adjacentBorders | int | [BorderType](../../com.aspose.cells/bordertype). Anger vilka kanter som behöver kontrolleras och justeras enligt kanterna på intilliggande celler. Se beskrivningen för samma parameter i [Cell.getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-). |

**Returns:**
[Style](../../com.aspose.cells/style) - the display style of given cell.
### getCellStyle(int row, int column) {#getCellStyle-int-int-}
```
public Style getCellStyle(int row, int column)
```


Hämta stilen för den angivna cellen.

**Remarks**

Den returnerade stilen är endast den som är inställd för cellen eller ärvd från rad/kolumn för cellen, och inkluderar inte de egenskaper som tillämpats av andra inställningar såsom villkorsstyrd formatering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | radindex |
| kolumn | int | kolumn |

**Returns:**
[Style](../../com.aspose.cells/style) - the style of given cell.
### getCellsWithPlaceInCellPicture() {#getCellsWithPlaceInCellPicture--}
```
public Iterator getCellsWithPlaceInCellPicture()
```


Hämtar alla celler som innehåller inbäddade bilder.

**Remarks**

Om det inte finns någon bild som är inställd på "Placera i cell" i detta kalkylblad, returneras null.

**Returns:**
java.util.Iterator – Enumerator för att enumerera alla Cell‑objekt som innehåller inbäddad bild
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


Hämtar den ursprungliga kolumnens höjd i punkt om kolumnen är dold

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället Cells.GetColumnWidth(int ,bool , CellsUnitType )‑metoden. Denna metod kommer att tas bort 12 månader senare från och med april 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Radindexet. |

**Returns:**
double – Kolumnens bredd i normal vy.
### getColumnWidth(int column) {#getColumnWidth-int-}
```
public double getColumnWidth(int column)
```


Hämtar bredden (i enhet av tecken) för den angivna kolumnen i normal vy

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindex |

**Returns:**
double – Kolumnens bredd. För kalkylblad mäts kolumnbredd som antalet tecken av den maximala siffra bredden för siffrorna 0~9 som återges i normalstilens teckensnitt.
### getColumnWidth(int column, boolean isOriginal, int unitType) {#getColumnWidth-int-boolean-int-}
```
public double getColumnWidth(int column, boolean isOriginal, int unitType)
```


Hämtar kolumnbredden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindexet. |
| isOriginal | boolean | Anger om originalbredden hämtas. |
| unitType | int | [CellsUnitType](../../com.aspose.cells/cellsunittype). |

**Returns:**
double -
### getColumnWidthInch(int column) {#getColumnWidthInch-int-}
```
public double getColumnWidthInch(int column)
```


Hämtar bredden på den angivna kolumnen i normal vy, i tum.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället Cells.GetColumnWidth(int ,bool , CellsUnitType )‑metoden. Denna metod kommer att tas bort 12 månader senare från och med april 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindex |

**Returns:**
double – Kolumnens bredd i normal vy.
### getColumnWidthPixel(int column) {#getColumnWidthPixel-int-}
```
public int getColumnWidthPixel(int column)
```


Hämtar bredden på den angivna kolumnen i normal vy, i pixlar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindex |

**Returns:**
int – Kolumnens bredd i normal vy.
### getColumnWidthPixel(int column, boolean original) {#getColumnWidthPixel-int-boolean-}
```
public int getColumnWidthPixel(int column, boolean original)
```


Hämtar bredden på den angivna kolumnen i normal vy, i pixlar.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället Cells.GetColumnWidth(int ,bool , CellsUnitType )‑metoden. Denna metod kommer att tas bort 12 månader senare från och med april 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindex |
| original | boolean | Anger om originalbredden ska returneras även när kolumnen är dold |

**Returns:**
int – Kolumnens bredd i normal vy.
### getColumns() {#getColumns--}
```
public ColumnCollection getColumns()
```


Hämtar samlingen av [Column](../../com.aspose.cells/column)-objekt som representerar de enskilda kolumnerna i detta kalkylblad.

**Returns:**
[ColumnCollection](../../com.aspose.cells/columncollection)
### getCount() {#getCount--}
```
public int getCount()
```


Hämtar det totala antalet instansierade Cell-objekt.

**Returns:**
int
### getCountLarge() {#getCountLarge--}
```
public long getCountLarge()
```


Hämtar det totala antalet instansierade Cell-objekt.

**Returns:**
long
### getDependents(boolean isAll, int row, int column) {#getDependents-boolean-int-int-}
```
public Cell[] getDependents(boolean isAll, int row, int column)
```


Hämta alla celler som refererar till den specifika cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isAll | boolean | Anger om andra kalkylblad ska kontrolleras |
| rad | int | Radindexet. |
| kolumn | int | Kolumnindexet. |

**Returns:**
com.aspose.cells.Cell[] –
### getDependentsInCalculation(int row, int column, boolean recursive) {#getDependentsInCalculation-int-int-boolean-}
```
public Iterator getDependentsInCalculation(int row, int column, boolean recursive)
```


Hämtar alla celler vars beräknade resultat beror på en specifik cell.

**Remarks**

För att använda denna metod, se till att arbetsboken har satts till true för [FormulaSettings.getEnableCalculationChain()](../../com.aspose.cells/formulasettings\#getEnableCalculationChain--) och har beräknats fullt ut med denna inställning. Om det inte finns någon formelreferens till denna cell, returneras null. För mer detaljer och exempel, se [Cell.getDependentsInCalculation(boolean)](../../com.aspose.cells/cell\#getDependentsInCalculation-boolean-)

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex för den specifika cellen |
| kolumn | int | Kolumnindex för den specifika cellen. |
| rekursiv | boolean | Om de returnerar de beroenden som inte refererar direkt till den specifika cellen men refererar till andra löv av den cellen. |

**Returns:**
java.util.Iterator – Enumerator för att enumerera alla beroenden (Cell‑objekt)
### getFirstCell() {#getFirstCell--}
```
public Cell getFirstCell()
```


Hämtar den första cellen i detta kalkylblad.

**Remarks**

Returnerar null om det inte finns någon data i kalkylbladet.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getFirstDataRow(int column) {#getFirstDataRow-int-}
```
public int getFirstDataRow(int column)
```


Hämtar det första radindexet för cellen som innehåller data i den angivna kolumnen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindex. |

**Returns:**
int - första radens index.
### getGroupedColumnOutlineLevel(int columnIndex) {#getGroupedColumnOutlineLevel-int-}
```
public int getGroupedColumnOutlineLevel(int columnIndex)
```


Hämtar konturnivån (nollbaserad) för kolumnen.

**Remarks**

Om kolumnen inte är grupperad returneras noll.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | Kolumnindexet |

**Returns:**
int - Konturnivån för kolumnen
### getGroupedRowOutlineLevel(int rowIndex) {#getGroupedRowOutlineLevel-int-}
```
public int getGroupedRowOutlineLevel(int rowIndex)
```


Hämtar konturnivån (nollbaserad) för raden.

**Remarks**

Om raden inte är grupperad returneras noll.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int | Radindexet. |

**Returns:**
int - Konturnivån (nollbaserad) för raden.
### getLastCell() {#getLastCell--}
```
public Cell getLastCell()
```


Hämtar den sista cellen i detta kalkylblad.

**Remarks**

Returnerar null om det inte finns någon data i kalkylbladet.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getLastDataRow(int column) {#getLastDataRow-int-}
```
public int getLastDataRow(int column)
```


Hämtar det sista radindexet för cellen som innehåller data i den angivna kolumnen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindex. |

**Returns:**
int - sista radens index.
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


Maximalt kolumnindex för de celler som har instansierats i samlingen (inkluderar inte kolumnen där stil är definierad för hela kolumnen men ingen cell har instansierats i den).

**Remarks**

Returnera -1 om ingen cell har instansierats.

**Returns:**
int
### getMaxDataColumn() {#getMaxDataColumn--}
```
public int getMaxDataColumn()
```


Maximalt kolumnindex för cellen som innehåller data.

**Remarks**

\-1 kommer att returneras om det inte finns någon cell som innehåller data. Denna egenskap måste iterera och kontrollera alla celler i ett kalkylblad dynamiskt, så det är en tidskrävande process och bör inte anropas upprepade gånger, exempelvis genom att använda den direkt som villkor i en loop.

**Returns:**
int
### getMaxDataRow() {#getMaxDataRow--}
```
public int getMaxDataRow()
```


Maximalt radindex för cellen som innehåller data.

**Remarks**

Returnera -1 om det inte finns någon cell som innehåller data. Denna egenskap måste iterera och kontrollera celler och rader dynamiskt, så det är en tidskrävande process och bör inte anropas upprepade gånger, exempelvis genom att använda den direkt som villkor i en loop.

**Returns:**
int
### getMaxDisplayRange() {#getMaxDisplayRange--}
```
public Range getMaxDisplayRange()
```


Hämtar det maximala området som inkluderar data, sammanslagna celler och former.

**Remarks**

Returnerar null om kalkylbladet är tomt sedan Aspose.Cells 21.5.2.

**Returns:**
[Range](../../com.aspose.cells/range)
### getMaxGroupedColumnOutlineLevel() {#getMaxGroupedColumnOutlineLevel--}
```
public int getMaxGroupedColumnOutlineLevel()
```


Hämtar den maximala grupperade kolumnens konturnivå (nollbaserad).

**Returns:**
int - Maximal konturnivå för grupperad kolumn (nollbaserad)
### getMaxGroupedRowOutlineLevel() {#getMaxGroupedRowOutlineLevel--}
```
public int getMaxGroupedRowOutlineLevel()
```


Hämtar den maximala grupperade radens konturnivå (nollbaserad).

**Returns:**
int - Maximal konturnivå för grupperad rad (nollbaserad)
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


Maximalt radindex för cellen som innehåller data eller stil.

**Remarks**

Returnera -1 om det inte finns någon cell som innehåller data eller stil i kalkylbladet. Denna egenskap måste iterera och kontrollera celler och rader dynamiskt, så det är en tidskrävande process och bör inte anropas upprepade gånger, exempelvis genom att använda den direkt som villkor i en loop.

**Returns:**
int
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


Hämtar minnesanvändningsalternativet för dessa celler.

Se [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Anmärkningsvärda begränsningar och rekommenderade operationer för vissa lägen:

| Läge | Anmärkningar | Stöds |
| ------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
| [MemorySetting.MEMORY\_PREFERENCE](../../com.aspose.cells/memorysetting\#MEMORY-PREFERENCE) | Cells data will be maintained in compact format to decrease the memory cost. On other hand, the compact data also may cause higher time cost, especially when updating the cells data, or accessing cells/rows randomly | v8.0.0 |
|  | [MemorySetting.FILE\_CACHE](../../com.aspose.cells/memorysetting\#FILE-CACHE) | När detta läge används för ett kalkylblad i en arbetsbok, bör [Workbook.dispose()](../../com.aspose.cells/workbook\#dispose--) anropas i slutet av arbetet för att frigöra alla resurser såsom temporära filer. |
 
Att slumpmässigt komma åt celler ger dålig prestanda eftersom data måste läsas/uppdateras slumpmässigt och upprepade gånger (så pekaren i filen ändras därefter och I/O‑operationer krävs upprepade gånger). Om möjligt, vänligen åtkomst data sekventiellt (rad för rad).
 
När data i en rad/cell ändras kan data i andra celler/rader också påverkas (t.ex. att data flyttas/förflyttas till andra platser för att allokera tillräckligt med utrymme för den ändrade datan). Så varje förändring av varje data kräver synkronisering av andra befintliga objekt (såsom rad‑ eller cell‑objekt). För att få bättre prestanda, vänligen håll inte flera rader/celler samtidigt. Att bearbeta dem en åt gången minskar datasynkroniseringen för dem så prestandan kan förbättras något. | v25.7     |

**Returns:**
int
### getMergedAreas() {#getMergedAreas--}
```
public CellArea[] getMergedAreas()
```


Hämtar alla sammanslagna celler.

**Returns:**
com.aspose.cells.CellArea[]
### getMergedCells() {#getMergedCells--}
```
public ArrayList getMergedCells()
```


Hämtar samlingen av sammanslagna celler.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället Cells.GetMergedAreas()-metoden. Denna metod kommer att tas bort 12 månader senare från och med november 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
java.util.ArrayList
### getMinColumn() {#getMinColumn--}
```
public int getMinColumn()
```


Minimalt kolumnindex för de celler som har instansierats i samlingen (inkluderar inte kolumnen där stil är definierad för hela kolumnen men ingen cell har instansierats i den).

**Remarks**

Denna egenskap måste iterera och kontrollera celler och rader dynamiskt, så det är en tidskrävande process och bör inte anropas upprepade gånger, exempelvis genom att använda den direkt som villkor i en loop.

**Returns:**
int
### getMinDataColumn() {#getMinDataColumn--}
```
public int getMinDataColumn()
```


Minsta kolumnindex för cell som innehåller data.

**Remarks**

\-1 kommer att returneras om det inte finns någon cell som innehåller data. Denna egenskap måste iterera och kontrollera alla celler i ett kalkylblad dynamiskt, så det är en tidskrävande process och bör inte anropas upprepade gånger, exempelvis genom att använda den direkt som villkor i en loop.

**Returns:**
int
### getMinDataRow() {#getMinDataRow--}
```
public int getMinDataRow()
```


Minsta radindex för cell som innehåller data.

**Remarks**

Returnera -1 om det inte finns någon cell som innehåller data. Denna egenskap måste iterera och kontrollera celler och rader dynamiskt, så det är en tidskrävande process och bör inte anropas upprepade gånger, exempelvis genom att använda den direkt som villkor i en loop.

**Returns:**
int
### getMinRow() {#getMinRow--}
```
public int getMinRow()
```


Minsta radindex för cell som innehåller data eller stil.

**Remarks**

Denna egenskap måste iterera och kontrollera celler och rader dynamiskt, så det är en tidskrävande process och bör inte anropas upprepade gånger, exempelvis genom att använda den direkt som villkor i en loop.

**Returns:**
int
### getMultiThreadReading() {#getMultiThreadReading--}
```
public boolean getMultiThreadReading()
```


Hämtar om cellernas datamodell ska stödja flertrådad läsning. Standardvärdet för denna egenskap är falskt.

**Remarks**

Om det finns flera trådar som läser Row/Cell-objekt i den här samlingen samtidigt, bör den här egenskapen sättas till true, annars kan oväntade resultat produceras. Att stödja Multi-Thread-läsning kan försämra prestandan för åtkomst av Row/Cell-objekt från den här samlingen. Observera att vissa funktioner inte kan stödja Multi-Thread-läsning, såsom formateringsvärden (av [Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--), [Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), osv.). Så även om den här egenskapen är satt till true, kan dessa API:er fortfarande ge oväntade resultat för Multi-Thread-läsning.

**Returns:**
boolean
### getOdsCellFields() {#getOdsCellFields--}
```
public OdsCellFieldCollection getOdsCellFields()
```


Hämtar listan över fält i ods.

**Returns:**
[OdsCellFieldCollection](../../com.aspose.cells/odscellfieldcollection)
### getPreserveString() {#getPreserveString--}
```
public boolean getPreserveString()
```


Hämtar ett värde som indikerar om alla kalkylbladsvärden bevaras som strängar. Standard är false.

**Returns:**
boolean
### getRanges() {#getRanges--}
```
public RangeCollection getRanges()
```


Hämtar samlingen av [Range](../../com.aspose.cells/range)-objekt som skapas vid körning.

**Returns:**
[RangeCollection](../../com.aspose.cells/rangecollection)
### getRowEnumerator() {#getRowEnumerator--}
```
public Iterator getRowEnumerator()
```


Hämtar radernas enumerator.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället metoden RowCollection.GetEnumerator(). Denna metod kommer att tas bort 12 månader senare från och med maj 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
java.util.Iterator - Radräknaren.
### getRowHeight(int row) {#getRowHeight-int-}
```
public double getRowHeight(int row)
```


Hämtar höjden på en specificerad rad, i enheten punkter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex |

**Returns:**
double - Radhöjd
### getRowHeight(int row, boolean isOriginal, int unitType) {#getRowHeight-int-boolean-int-}
```
public double getRowHeight(int row, boolean isOriginal, int unitType)
```


Hämtar radens höjd.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindexet. |
| isOriginal | boolean | Anger om den returnerar den ursprungliga radhöjden eller 0 för dold rad. |
| unitType | int | [CellsUnitType](../../com.aspose.cells/cellsunittype). Enhetstyp för det returnerade höjdvärdet |

**Returns:**
double - Radhöjd
### getRowHeightInch(int row) {#getRowHeightInch-int-}
```
public double getRowHeightInch(int row)
```


Hämtar höjden på en specificerad rad i enheten tum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex |

**Returns:**
double - Radhöjd
### getRowHeightPixel(int row) {#getRowHeightPixel-int-}
```
public int getRowHeightPixel(int row)
```


Hämtar höjden på en specificerad rad i enheten pixel.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex |

**Returns:**
int - Radhöjd
### getRowOriginalHeightPoint(int row) {#getRowOriginalHeightPoint-int-}
```
public double getRowOriginalHeightPoint(int row)
```


Hämtar den ursprungliga radens höjd i enheten punkt om raden är dold.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället metoden Cells.GetRowHeight(int,bool,CellsUnitType). Denna metod kommer att tas bort 12 månader senare från och med april 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindexet. |

**Returns:**
double -
### getRows() {#getRows--}
```
public RowCollection getRows()
```


Hämtar samlingen av [Row](../../com.aspose.cells/row)-objekt som representerar de enskilda raderna i detta kalkylblad.

**Returns:**
[RowCollection](../../com.aspose.cells/rowcollection)
### getStandardHeight() {#getStandardHeight--}
```
public double getStandardHeight()
```


Hämtar standardradens höjd i detta kalkylblad, i enheten punkter.

**Returns:**
double
### getStandardHeightInch() {#getStandardHeightInch--}
```
public double getStandardHeightInch()
```


Hämtar standardradens höjd i detta kalkylblad, i enheten tum.

**Returns:**
double
### getStandardHeightPixels() {#getStandardHeightPixels--}
```
public int getStandardHeightPixels()
```


Hämtar standardradens höjd i detta kalkylblad, i enheten pixlar.

**Returns:**
int
### getStandardWidth() {#getStandardWidth--}
```
public double getStandardWidth()
```


Hämtar standardkolumnens bredd i kalkylbladet, i enheten tecken.

**Returns:**
double
### getStandardWidthInch() {#getStandardWidthInch--}
```
public double getStandardWidthInch()
```


Hämtar standardkolumnens bredd i kalkylbladet, i enheten tum.

**Returns:**
double
### getStandardWidthPixels() {#getStandardWidthPixels--}
```
public int getStandardWidthPixels()
```


Hämtar standardkolumnens bredd i kalkylbladet, i enheten pixlar.

**Returns:**
int
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Hämtar standardstilen för kalkylbladet.

**Returns:**
[Style](../../com.aspose.cells/style)
### getViewColumnWidthPixel(int column) {#getViewColumnWidthPixel-int-}
```
public int getViewColumnWidthPixel(int column)
```


Hämta bredden i olika vystyper.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindexet. |

**Returns:**
int - kolumnbredd i enhet av pixlar
### getViewRowHeight(int row) {#getViewRowHeight-int-}
```
public double getViewRowHeight(int row)
```


Hämtar höjden på en specificerad rad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex. |

**Returns:**
double - Radhöjd.
### getViewRowHeightInch(int row) {#getViewRowHeightInch-int-}
```
public double getViewRowHeightInch(int row)
```


Hämtar höjden på en specificerad rad i enheten tum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex |

**Returns:**
double - Radhöjd
### groupColumns(int firstIndex, int lastIndex) {#groupColumns-int-int-}
```
public void groupColumns(int firstIndex, int lastIndex)
```


Grupperar kolumner.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstIndex | int | Det första kolumnindexet som ska grupperas. |
| lastIndex | int | Det sista kolumnindexet som ska grupperas. |

### groupColumns(int firstIndex, int lastIndex, boolean isHidden) {#groupColumns-int-int-boolean-}
```
public void groupColumns(int firstIndex, int lastIndex, boolean isHidden)
```


Grupperar kolumner.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstIndex | int | Det första kolumnindexet som ska grupperas. |
| lastIndex | int | Det sista kolumnindexet som ska grupperas. |
| isHidden | boolean | Anger om de grupperade kolumnerna är dolda. |

### groupRows(int firstIndex, int lastIndex) {#groupRows-int-int-}
```
public void groupRows(int firstIndex, int lastIndex)
```


Grupperar rader.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstIndex | int | Det första radindexet som ska grupperas. |
| lastIndex | int | Det sista radindexet som ska grupperas. |

### groupRows(int firstIndex, int lastIndex, boolean isHidden) {#groupRows-int-int-boolean-}
```
public void groupRows(int firstIndex, int lastIndex, boolean isHidden)
```


Grupperar rader.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstIndex | int | Det första radindexet som ska grupperas. |
| lastIndex | int | Det sista radindexet som ska grupperas. |
| isHidden | boolean | Anger om de grupperade raderna är dolda. |

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


Döljer en kolumn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindex. |

### hideColumns(int column, int totalColumns) {#hideColumns-int-int-}
```
public void hideColumns(int column, int totalColumns)
```


Dölj flera kolumner.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindex. |
| totalColumns | int | Kolumnnummer. |

### hideGroupDetail(boolean isVertical, int index) {#hideGroupDetail-boolean-int-}
```
public void hideGroupDetail(boolean isVertical, int index)
```


Komprimerar de grupperade raderna/kolumnerna.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isVertical | boolean | True, kollapsa de grupperade raderna. |
| index | int | Rad-/kolumnindexet |

### hideRow(int row) {#hideRow-int-}
```
public void hideRow(int row)
```


Döljer en rad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex. |

### hideRows(int row, int totalRows) {#hideRows-int-int-}
```
public void hideRows(int row, int totalRows)
```


Dölj flera rader.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindexet. |
| totalRows | int | Radnumret. |

### importArray(double[] doubleArray, int firstRow, int firstColumn, boolean isVertical) {#importArray-double---int-int-boolean-}
```
public void importArray(double[] doubleArray, int firstRow, int firstColumn, boolean isVertical)
```


Importerar en array av double till ett kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| doubleArray | double[] | Dubbel array. |
| firstRow | int | Radnumret för den första cellen att importera i. |
| firstColumn | int | Kolumnnumret för den första cellen att importera i. |
| isVertical | boolean | Anger att importera data vertikalt eller horisontellt. |

### importArray(double[][] doubleArray, int firstRow, int firstColumn) {#importArray-double-----int-int-}
```
public void importArray(double[][] doubleArray, int firstRow, int firstColumn)
```


Importerar en tvådimensionell array av double till ett kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| doubleArray | double[][] | Tvådimensionell double-array. |
| firstRow | int | Radnumret för den första cellen att importera i. |
| firstColumn | int | Kolumnnumret för den första cellen att importera i. |

### importArray(int[] intArray, int firstRow, int firstColumn, boolean isVertical) {#importArray-int---int-int-boolean-}
```
public void importArray(int[] intArray, int firstRow, int firstColumn, boolean isVertical)
```


Importerar en array av integer till ett kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| intArray | int[] | Heltalsarray. |
| firstRow | int | Radnumret för den första cellen att importera i. |
| firstColumn | int | Kolumnnumret för den första cellen att importera i. |
| isVertical | boolean | Anger att importera data vertikalt eller horisontellt. |

### importArray(int[][] intArray, int firstRow, int firstColumn) {#importArray-int-----int-int-}
```
public void importArray(int[][] intArray, int firstRow, int firstColumn)
```


Importerar en tvådimensionell array av integer till ett kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| intArray | int[][] | Tvådimensionell heltalsarray. |
| firstRow | int | Radnumret för den första cellen att importera i. |
| firstColumn | int | Kolumnnumret för den första cellen att importera i. |

### importArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical) {#importArray-java.lang.String---int-int-boolean-}
```
public void importArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)
```


Importerar en array av string till ett kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stringArray | java.lang.String[] | Strängarray. |
| firstRow | int | Radnumret för den första cellen att importera i. |
| firstColumn | int | Kolumnnumret för den första cellen att importera i. |
| isVertical | boolean | Anger att importera data vertikalt eller horisontellt. |

### importArray(String[][] stringArray, int firstRow, int firstColumn) {#importArray-java.lang.String-----int-int-}
```
public void importArray(String[][] stringArray, int firstRow, int firstColumn)
```


Importerar en tvådimensionell array av string till ett kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stringArray | java.lang.String[][] | Tvådimensionell strängarray. |
| firstRow | int | Radnumret för den första cellen att importera i. |
| firstColumn | int | Kolumnnumret för den första cellen att importera i. |

### importArrayList(ArrayList arrayList, int firstRow, int firstColumn, boolean isVertical) {#importArrayList-java.util.ArrayList-int-int-boolean-}
```
public void importArrayList(ArrayList arrayList, int firstRow, int firstColumn, boolean isVertical)
```


Importerar en arraylist av data till ett kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arrayList | java.util.ArrayList | Data arraylist. |
| firstRow | int | Radnumret för den första cellen att importera i. |
| firstColumn | int | Kolumnnumret för den första cellen att importera i. |
| isVertical | boolean | Anger att importera data vertikalt eller horisontellt. |

### importCSV(InputStream stream, TxtLoadOptions options, int firstRow, int firstColumn) {#importCSV-java.io.InputStream-com.aspose.cells.TxtLoadOptions-int-int-}
```
public void importCSV(InputStream stream, TxtLoadOptions options, int firstRow, int firstColumn)
```


Importera en CSV-fil till cellerna.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.InputStream | CSV-filströmmen. |
| options | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | Inläsningsalternativen för att läsa textfil. |
| firstRow | int | Radnumret för den första cellen att importera i. |
| firstColumn | int | Kolumnnumret för den första cellen att importera i. |

### importCSV(InputStream stream, String splitter, boolean convertNumericData, int firstRow, int firstColumn) {#importCSV-java.io.InputStream-java.lang.String-boolean-int-int-}
```
public void importCSV(InputStream stream, String splitter, boolean convertNumericData, int firstRow, int firstColumn)
```


Importera en CSV-fil till cellerna.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.InputStream | CSV-filströmmen. |
| splitter | java.lang.String | Delaren |
| convertNumericData | boolean | Om strängen i textfilen konverteras till numerisk data. |
| firstRow | int | Radnumret för den första cellen att importera i. |
| firstColumn | int | Kolumnnumret för den första cellen att importera i. |

### importCSV(String fileName, TxtLoadOptions options, int firstRow, int firstColumn) {#importCSV-java.lang.String-com.aspose.cells.TxtLoadOptions-int-int-}
```
public void importCSV(String fileName, TxtLoadOptions options, int firstRow, int firstColumn)
```


Importera en CSV-fil till cellerna.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | java.lang.String | CSV-filnamnet. |
| options | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | Inläsningsalternativen för att läsa textfil. |
| firstRow | int | Radnumret för den första cellen att importera i. |
| firstColumn | int | Kolumnnumret för den första cellen att importera i. |

### importCSV(String fileName, String splitter, boolean convertNumericData, int firstRow, int firstColumn) {#importCSV-java.lang.String-java.lang.String-boolean-int-int-}
```
public void importCSV(String fileName, String splitter, boolean convertNumericData, int firstRow, int firstColumn)
```


Importera en CSV-fil till cellerna.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | java.lang.String | CSV-filnamnet. |
| splitter | java.lang.String | Delaren |
| convertNumericData | boolean | Om strängen i textfilen konverteras till numerisk data. |
| firstRow | int | Radnumret för den första cellen att importera i. |
| firstColumn | int | Kolumnnumret för den första cellen att importera i. |

### importCustomObjects(Collection list, int firstRow, int firstColumn, ImportTableOptions options) {#importCustomObjects-java.util.Collection-int-int-com.aspose.cells.ImportTableOptions-}
```
public int importCustomObjects(Collection list, int firstRow, int firstColumn, ImportTableOptions options)
```


Importerar anpassade objekt.

**Remarks**

De anpassade objekten bör vara av samma typ.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| list | java.util.Collection | Det anpassade objektet |
| firstRow | int | Radnumret för den första cellen att importera i. |
| firstColumn | int | Kolumnnumret för den första cellen att importera i. |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | Importalternativen. |

**Returns:**
int - Totalt antal importerade rader.
### importCustomObjects(Collection list, String[] propertyNames, boolean isPropertyNameShown, int firstRow, int firstColumn, int rowNumber, boolean insertRows, String dateFormatString, boolean convertStringToNumber) {#importCustomObjects-java.util.Collection-java.lang.String---boolean-int-int-int-boolean-java.lang.String-boolean-}
```
public int importCustomObjects(Collection list, String[] propertyNames, boolean isPropertyNameShown, int firstRow, int firstColumn, int rowNumber, boolean insertRows, String dateFormatString, boolean convertStringToNumber)
```


Importerar anpassade objekt.

**Remarks**

De anpassade objekten bör vara av samma typ.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| list | java.util.Collection | Det anpassade objektet |
| propertyNames | java.lang.String[] | Egenskapsnamnen. Om det är null, importerar vi alla egenskaper i objektet. |
| isPropertyNameShown | boolean | Indikerar om egendomsnamnet kommer att importeras till den första raden. |
| firstRow | int | Radnumret för den första cellen att importera i. |
| firstColumn | int | Kolumnnumret för den första cellen att importera i. |
| rowNumber | int | Antal rader som ska importeras. |
| insertRows | boolean | Indikerar om extra rader läggs till för att passa data. |
| dateFormatString | java.lang.String | Datumformatsträng för celler. |
| convertStringToNumber | boolean | Indikerar om denna metod kommer att försöka konvertera sträng till tal. |

**Returns:**
int - Totalt antal importerade rader.
### importData(ICellsDataTable table, int firstRow, int firstColumn, ImportTableOptions options) {#importData-com.aspose.cells.ICellsDataTable-int-int-com.aspose.cells.ImportTableOptions-}
```
public int importData(ICellsDataTable table, int firstRow, int firstColumn, ImportTableOptions options)
```


Importera data från en anpassad datatabell.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| table | [ICellsDataTable](../../com.aspose.cells/icellsdatatable) | Den anpassade datatabellen. |
| firstRow | int | Första radens index. |
| firstColumn | int | Första kolumnens index. |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | Importalternativen |

**Returns:**
int -
### importFormulaArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical) {#importFormulaArray-java.lang.String---int-int-boolean-}
```
public void importFormulaArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)
```


Importerar en array av formel till ett kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stringArray | java.lang.String[] | Formelarray. |
| firstRow | int | Radnumret för den första cellen att importera i. |
| firstColumn | int | Kolumnnumret för den första cellen att importera i. |
| isVertical | boolean | Anger att importera data vertikalt eller horisontellt. |

### importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical) {#importObjectArray-java.lang.Object---int-int-boolean-}
```
public void importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical)
```


Importerar en array av data till ett kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| objArray | java.lang.Object[] | Dataarray. |
| firstRow | int | Radnumret för den första cellen att importera i. |
| firstColumn | int | Kolumnnumret för den första cellen att importera i. |
| isVertical | boolean | Anger att importera data vertikalt eller horisontellt. |

### importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical, int skip) {#importObjectArray-java.lang.Object---int-int-boolean-int-}
```
public void importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical, int skip)
```


Importerar en array av data till ett kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| objArray | java.lang.Object[] | Dataarray. |
| firstRow | int | Radnumret för den första cellen att importera i. |
| firstColumn | int | Kolumnnumret för den första cellen att importera i. |
| isVertical | boolean | Anger att importera data vertikalt eller horisontellt. |
| skip | int | Antal rader eller kolumner som hoppats över. |

### importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-int-int-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown)
```


Importerar data i ett ResultSet-objekt till kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rs | java.sql.ResultSet | ResultSet-objektet att importera från. |
| rowIndex | int | Startradindex i kalkylbladet. |
| columnIndex | int | Startkolumnindex i kalkylbladet. |
| isFieldNameShown | boolean | Indikerar om fältnamnet i resultsetet kommer att importeras till den första raden. |

**Returns:**
int – hur många rader som faktiskt importerades.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber) {#importResultSet-java.sql.ResultSet-int-int-boolean-java.lang.String-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)
```


Importerar data i ett ResultSet-objekt till kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rs | java.sql.ResultSet | ResultSet-objektet att importera från. |
| rowIndex | int | Startradindex i kalkylbladet. |
| columnIndex | int | Startkolumnindex i kalkylbladet. |
| isFieldNameShown | boolean | Indikerar om fältnamnet i resultsetet kommer att importeras till den första raden. |
| customDateFormatString | java.lang.String | Datumformatsträng för celler som innehåller datumvärde. |
| convertStringToNumber | boolean | Indikerar om denna metod kommer att försöka konvertera sträng till tal. |

**Returns:**
int – hur många rader som faktiskt importerades.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, ImportTableOptions options) {#importResultSet-java.sql.ResultSet-int-int-com.aspose.cells.ImportTableOptions-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, ImportTableOptions options)
```


Importerar data i ett ResultSet-objekt till kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rs | java.sql.ResultSet | ResultSet-objektet att importera från. |
| rowIndex | int | Startradindex i kalkylbladet. |
| columnIndex | int | Startkolumnindex i kalkylbladet. |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | Importalternativen |

**Returns:**
int – hur många rader som faktiskt importerades.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown)
```


Importerar data i ett ResultSet-objekt till kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rs | java.sql.ResultSet | ResultSet-objektet att importera från. |
| rowIndex | int | Startradindex i kalkylbladet. |
| columnIndex | int | Startkolumnindex i kalkylbladet. |
| rowNum | int | antal rader att importera. -1 för att importera alla poster i angivet resultset. |
| columnNum | int | antal kolumner att importera. -1 för att importera alla kolumner i angivet resultset. |
| isFieldNameShown | boolean | Indikerar om fältnamnet i resultsetet kommer att importeras till den första raden. |

**Returns:**
int – hur många rader som faktiskt importerades.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber) {#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-java.lang.String-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)
```


Importerar data i ett ResultSet-objekt till kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rs | java.sql.ResultSet | ResultSet-objektet att importera från. |
| rowIndex | int | Startradindex i kalkylbladet. |
| columnIndex | int | Startkolumnindex i kalkylbladet. |
| rowNum | int | antal rader att importera. -1 för att importera alla poster i angivet resultset. |
| columnNum | int | antal kolumner att importera. -1 för att importera alla kolumner i angivet resultset. |
| isFieldNameShown | boolean | Indikerar om fältnamnet i resultsetet kommer att importeras till den första raden. |
| customDateFormatString | java.lang.String | Datumformatsträng för celler som innehåller datumvärde. |
| convertStringToNumber | boolean | Indikerar om denna metod kommer att försöka konvertera sträng till tal. |

**Returns:**
int – hur många rader som faktiskt importerades.
### importResultSet(ResultSet rs, String startCell, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-java.lang.String-boolean-}
```
public int importResultSet(ResultSet rs, String startCell, boolean isFieldNameShown)
```


Importerar data i ett ResultSet-objekt till kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rs | java.sql.ResultSet | ResultSet-objektet att importera från. |
| startCell | java.lang.String | namn på startcell för att infoga resultsetet, till exempel \"A1\". |
| isFieldNameShown | boolean | Indikerar om fältnamnet i resultsetet kommer att importeras till den första raden. |

**Returns:**
int – hur många rader som faktiskt importerades.
### importResultSet(ResultSet rs, String startCell, ImportTableOptions options) {#importResultSet-java.sql.ResultSet-java.lang.String-com.aspose.cells.ImportTableOptions-}
```
public int importResultSet(ResultSet rs, String startCell, ImportTableOptions options)
```


Importerar data i ett ResultSet-objekt till kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rs | java.sql.ResultSet | ResultSet-objektet att importera från. |
| startCell | java.lang.String | namn på startcell för att infoga resultsetet, till exempel \"A1\". |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | Importalternativen |

**Returns:**
int – hur många rader som faktiskt importerades.
### importResultSet(ResultSet rs, String startCell, int rowNum, int columnNum, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-java.lang.String-int-int-boolean-}
```
public int importResultSet(ResultSet rs, String startCell, int rowNum, int columnNum, boolean isFieldNameShown)
```


Importerar data i ett ResultSet-objekt till kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rs | java.sql.ResultSet | ResultSet-objektet att importera från. |
| startCell | java.lang.String | namn på startcell för att infoga resultsetet, till exempel \"A1\". |
| rowNum | int | antal rader att importera. -1 för att importera alla poster i angivet resultset. |
| columnNum | int | antal kolumner att importera. -1 för att importera alla kolumner i angivet resultset. |
| isFieldNameShown | boolean | Indikerar om fältnamnet i resultsetet kommer att importeras till den första raden. |

**Returns:**
int – hur många rader som faktiskt importerades.
### importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn) {#importTwoDimensionArray-java.lang.Object-----int-int-}
```
public void importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn)
```


Importerar en tvådimensionell array av data till ett kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| objArray | java.lang.Object[][] | Tvådimensionell dataarray. |
| firstRow | int | Radnumret för den första cellen att importera i. |
| firstColumn | int | Kolumnnumret för den första cellen att importera i. |

### importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn, boolean convertStringToNumber) {#importTwoDimensionArray-java.lang.Object-----int-int-boolean-}
```
public void importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn, boolean convertStringToNumber)
```


Importerar en tvådimensionell array av data till ett kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| objArray | java.lang.Object[][] | Tvådimensionell dataarray. |
| firstRow | int | Radnumret för den första cellen att importera i. |
| firstColumn | int | Kolumnnumret för den första cellen att importera i. |
| convertStringToNumber | boolean | Indikerar om denna metod kommer att försöka konvertera sträng till tal. |

### importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, boolean convertStringToNumber) {#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-boolean-}
```
public void importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, boolean convertStringToNumber)
```


Importerar en tvådimensionell array av data till ett kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| objArray | java.lang.Object[][] | Tvådimensionell dataarray. |
| stilar | java.lang.Object[][] | Tvådimensionell datastil. |
| firstRow | int | Radnumret för den första cellen att importera i. |
| firstColumn | int | Kolumnnumret för den första cellen att importera i. |
| convertStringToNumber | boolean | Indikerar om denna metod kommer att försöka konvertera sträng till tal. |

### importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, TxtLoadOptions opts) {#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-com.aspose.cells.TxtLoadOptions-}
```
public void importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, TxtLoadOptions opts)
```


Importerar en tvådimensionell array av data till ett kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| objArray | java.lang.Object[][] | Tvådimensionell dataarray. |
| stilar | java.lang.Object[][] | Tvådimensionell datastil. |
| firstRow | int | Radnumret för den första cellen att importera i. |
| firstColumn | int | Kolumnnumret för den första cellen att importera i. |
| opts | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | Alternativ för konvertering av strängvärden |

### insertColumn(int columnIndex) {#insertColumn-int-}
```
public void insertColumn(int columnIndex)
```


Infogar en ny kolumn i kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | Kolumnindex. |

### insertColumn(int columnIndex, boolean updateReference) {#insertColumn-int-boolean-}
```
public void insertColumn(int columnIndex, boolean updateReference)
```


Infogar en ny kolumn i kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | Kolumnindex. |
| updateReference | boolean | Indikerar om referenser i andra arbetsblad kommer att uppdateras. |

### insertColumns(int columnIndex, int totalColumns) {#insertColumns-int-int-}
```
public void insertColumns(int columnIndex, int totalColumns)
```


Infogar några kolumner i kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | Kolumnindex. |
| totalColumns | int | Antalet kolumner. |

### insertColumns(int columnIndex, int totalColumns, boolean updateReference) {#insertColumns-int-int-boolean-}
```
public void insertColumns(int columnIndex, int totalColumns, boolean updateReference)
```


Infogar några kolumner i kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | Kolumnindex. |
| totalColumns | int | Antalet kolumner. |
| updateReference | boolean | Indikerar om referenser i andra arbetsblad kommer att uppdateras. |

### insertColumns(int columnIndex, int totalColumns, InsertOptions options) {#insertColumns-int-int-com.aspose.cells.InsertOptions-}
```
public void insertColumns(int columnIndex, int totalColumns, InsertOptions options)
```


Infogar några kolumner i kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | Kolumnindex. |
| totalColumns | int | Antalet kolumner. |
| options | [InsertOptions](../../com.aspose.cells/insertoptions) | Alternativen för infogningsoperationen. |

### insertCutCells(Range cutRange, int row, int column, int shiftType) {#insertCutCells-com.aspose.cells.Range-int-int-int-}
```
public void insertCutCells(Range cutRange, int row, int column, int shiftType)
```


Infoga klippt område.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cutRange | [Range](../../com.aspose.cells/range) | Klippområdet. |
| rad | int | Raden. |
| kolumn | int | Kolumnen. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Indikerar hur andra objekt i målområdet ska flyttas när klippområdet infogas. |

### insertRange(CellArea area, int shiftType) {#insertRange-com.aspose.cells.CellArea-int-}
```
public void insertRange(CellArea area, int shiftType)
```


Infogar ett cellområde och flyttar celler enligt förskjutningsalternativet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| area | [CellArea](../../com.aspose.cells/cellarea) | Flyttområde. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Alternativ för att skifta celler. |

### insertRange(CellArea area, int shiftNumber, int shiftType) {#insertRange-com.aspose.cells.CellArea-int-int-}
```
public void insertRange(CellArea area, int shiftNumber, int shiftType)
```


Infogar ett cellområde och flyttar celler enligt förskjutningsalternativet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| area | [CellArea](../../com.aspose.cells/cellarea) | Flyttområde. |
| shiftNumber | int | Antal rader eller kolumner som ska infogas. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Alternativ för att skifta celler. |

### insertRange(CellArea area, int shiftNumber, int shiftType, boolean updateReference) {#insertRange-com.aspose.cells.CellArea-int-int-boolean-}
```
public void insertRange(CellArea area, int shiftNumber, int shiftType, boolean updateReference)
```


Infogar ett cellområde och flyttar celler enligt förskjutningsalternativet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| area | [CellArea](../../com.aspose.cells/cellarea) | Flyttområde. |
| shiftNumber | int | Antal rader eller kolumner som ska infogas. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Alternativ för att skifta celler. |
| updateReference | boolean | Anger om referenser ska uppdateras i andra arbetsblad. |

### insertRow(int rowIndex) {#insertRow-int-}
```
public void insertRow(int rowIndex)
```


Infogar en ny rad i kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int | Radindex. |

### insertRows(int rowIndex, int totalRows) {#insertRows-int-int-}
```
public void insertRows(int rowIndex, int totalRows)
```


Infogar flera rader i kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int | Radindex. |
| totalRows | int | Antal rader som ska infogas. |

### insertRows(int rowIndex, int totalRows, boolean updateReference) {#insertRows-int-int-boolean-}
```
public void insertRows(int rowIndex, int totalRows, boolean updateReference)
```


Infogar flera rader i kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int | Radindex. |
| totalRows | int | Antal rader som ska infogas. |
| updateReference | boolean | Indikerar om referenser i andra arbetsblad kommer att uppdateras. |

### insertRows(int rowIndex, int totalRows, InsertOptions options) {#insertRows-int-int-com.aspose.cells.InsertOptions-}
```
public void insertRows(int rowIndex, int totalRows, InsertOptions options)
```


Infogar flera rader i kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int | Radindex. |
| totalRows | int | Antal rader som ska infogas. |
| options | [InsertOptions](../../com.aspose.cells/insertoptions) | Alternativ för infogningsoperation. |

### isBlankColumn(int columnIndex) {#isBlankColumn-int-}
```
public boolean isBlankColumn(int columnIndex)
```


Kontrollerar om given kolumn är tom (innehåller ingen data).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | kolumnindexet |

**Returns:**
boolesk - true om given kolumn inte innehåller någon data
### isColumnHidden(int columnIndex) {#isColumnHidden-int-}
```
public boolean isColumnHidden(int columnIndex)
```


Kontrollerar om en kolumn på angivet index är dold.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | kolumnindex |

**Returns:**
boolesk - true om kolumnen är dold.
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


Indikerar att radhöjd och standardteckensnittshöjd matchar

**Returns:**
boolean
### isDefaultRowHidden() {#isDefaultRowHidden--}
```
public boolean isDefaultRowHidden()
```


Indikerar om raden är standarddolt.

**Returns:**
boolean
### isDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns) {#isDeletingRangeEnabled-int-int-int-int-}
```
public boolean isDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns)
```


Kontrollera om området kan tas bort.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | Startradindexet för intervallet. |
| startColumn | int | Startkolumnindexet för intervallet. |
| totalRows | int | Antalet rader i intervallet. |
| totalColumns | int | Antalet kolumner i intervallet. |

**Returns:**
boolean -
### isRowHidden(int rowIndex) {#isRowHidden-int-}
```
public boolean isRowHidden(int rowIndex)
```


Kontrollerar om en rad på angivet index är dold.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int | radindex |

**Returns:**
boolesk - true om raden är dold
### iterator() {#iterator--}
```
public Iterator iterator()
```


Hämtar cellernas enumerator.

**Remarks**

När element traverseras med den returnerade Enumerator bör cellsamlingen inte modifieras (såsom operationer som skapar nya Cell/Row eller tar bort befintliga Cell/Row). Annars kan enumeratorn misslyckas med att traversera alla celler korrekt (vissa element kan traverseras flera gånger eller hoppas över).

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
java.util.Iterator - Cellernas enumerator
### linkToXmlMap(String mapName, int row, int column, String path) {#linkToXmlMap-java.lang.String-int-int-java.lang.String-}
```
public void linkToXmlMap(String mapName, int row, int column, String path)
```


Länk till en XML-karta.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| mapName | java.lang.String | namn på xml-karta |
| rad | int | rad för destinationscellen |
| kolumn | int | kolumn för destinationscellen |
| sökväg | java.lang.String | sökväg till xml-element i xml-karta |

### merge(int firstRow, int firstColumn, int totalRows, int totalColumns) {#merge-int-int-int-int-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Slår ihop ett angivet cellområde till en enda cell.

**Remarks**

Referera till den sammanslagna cellen via adressen för den övre vänstra cellen i intervallet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstRow | int | Första raden i detta intervall (nollbaserat) |
| firstColumn | int | Första kolumnen i detta intervall (nollbaserat) |
| totalRows | int | Antal rader (enbaserat) |
| totalColumns | int | Antal kolumner (enbaserat) |

### merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean mergeConflict) {#merge-int-int-int-int-boolean-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean mergeConflict)
```


Slår ihop ett angivet cellområde till en enda cell.

**Remarks**

Referera till den sammanslagna cellen via adressen för den övre vänstra cellen i intervallet. Om mergeConflict är true och det sammanslagna intervallet konflikterar med andra sammanslagna celler, kommer de andra sammanslagna cellerna att tas bort automatiskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstRow | int | Första raden i detta intervall (nollbaserat) |
| firstColumn | int | Första kolumnen i detta intervall (nollbaserat) |
| totalRows | int | Antal rader (enbaserat) |
| totalColumns | int | Antal kolumner (enbaserat) |
| mergeConflict | boolean | Sammanfoga konflikt sammanslagna områden. |

### merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean checkConflict, boolean mergeConflict) {#merge-int-int-int-int-boolean-boolean-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean checkConflict, boolean mergeConflict)
```


Slår ihop ett angivet cellområde till en enda cell.

**Remarks**

Referera till den sammanslagna cellen via adressen för den övre vänstra cellen i intervallet. Om mergeConflict är true och det sammanslagna intervallet konflikterar med andra sammanslagna celler, kommer de andra sammanslagna cellerna att tas bort automatiskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstRow | int | Första raden i detta intervall (nollbaserat) |
| firstColumn | int | Första kolumnen i detta intervall (nollbaserat) |
| totalRows | int | Antal rader (enbaserat) |
| totalColumns | int | Antal kolumner (enbaserat) |
| checkConflict | boolean | Indikerar om kontrollen av de sammanslagna cellerna intersecterar andra sammanslagna celler. |
| mergeConflict | boolean | Sammanfoga konflikt sammanslagna områden. |

### moveRange(CellArea sourceArea, int destRow, int destColumn) {#moveRange-com.aspose.cells.CellArea-int-int-}
```
public void moveRange(CellArea sourceArea, int destRow, int destColumn)
```


Flyttar området.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceArea | [CellArea](../../com.aspose.cells/cellarea) | Det område som ska flyttas. |
| destRow | int | Målraden. |
| destColumn | int | Målkolumnen. |

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


Tar bort dubblett rader i bladet.

### removeDuplicates(int startRow, int startColumn, int endRow, int endColumn) {#removeDuplicates-int-int-int-int-}
```
public void removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)
```


Tar bort dubblettvärden i området.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | Startrad. |
| startColumn | int | Startkolumn |
| slutRad | int | Slutradens index. |
| endColumn | int | Slutkolumnens index. |

### removeDuplicates(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders, int[] columnOffsets) {#removeDuplicates-int-int-int-int-boolean-int---}
```
public void removeDuplicates(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders, int[] columnOffsets)
```


Tar bort dubblettdata i området.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | Startrad. |
| startColumn | int | Startkolumn |
| slutRad | int | Slutradens index. |
| endColumn | int | Slutkolumnens index. |
| hasHeaders | boolean | Indikerar om området innehåller rubriker. |
| columnOffsets | int[] | Kolumnförskjutningarna. |

### removeFormulas() {#removeFormulas--}
```
public void removeFormulas()
```


Tar bort alla formler och ersätter dem med formelns värde.

### retrieveSubtotalSetting(CellArea ca) {#retrieveSubtotalSetting-com.aspose.cells.CellArea-}
```
public SubtotalSetting retrieveSubtotalSetting(CellArea ca)
```


Hämtar delsummeinställningarna för området.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Området |

**Returns:**
[SubtotalSetting](../../com.aspose.cells/subtotalsetting) - 
### setColumnWidth(int column, double width) {#setColumnWidth-int-double-}
```
public void setColumnWidth(int column, double width)
```


Ställer in bredden på den angivna kolumnen i normal vy.

**Remarks**

För kalkylblad mäts kolumnbredden som antalet tecken av den maximala siffrabredden för siffrorna 0~9 när de renderas i det normala stilens teckensnitt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindex. |
| bredd | double | Kolumnbredd i teckenenheter. Kolumnbredden måste vara mellan 0 och 255. |

### setColumnWidthInch(int column, double inches) {#setColumnWidthInch-int-double-}
```
public void setColumnWidthInch(int column, double inches)
```


Ställer in kolumnbredd i tum i normal vy.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindex. |
| tum | double | Antal tum. |

### setColumnWidthPixel(int column, int pixels) {#setColumnWidthPixel-int-int-}
```
public void setColumnWidthPixel(int column, int pixels)
```


Ställer in kolumnbredd i pixlar i normal vy.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindex. |
| pixlar | int | Antal pixlar. |

### setDefaultColumnHidden(boolean value) {#setDefaultColumnHidden-boolean-}
```
public void setDefaultColumnHidden(boolean value)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setDefaultRowHeightMatched(boolean value) {#setDefaultRowHeightMatched-boolean-}
```
public void setDefaultRowHeightMatched(boolean value)
```


Indikerar att radhöjd och standardteckensnittshöjd matchar

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setDefaultRowHidden(boolean value) {#setDefaultRowHidden-boolean-}
```
public void setDefaultRowHidden(boolean value)
```


Indikerar om raden är standarddolt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


Ställer in minnesanvändningsalternativet för dessa celler.

Se [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Anmärkningsvärda begränsningar och rekommenderade operationer för vissa lägen:

| Läge | Anmärkningar | Stöds |
| ------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
| [MemorySetting.MEMORY\_PREFERENCE](../../com.aspose.cells/memorysetting\#MEMORY-PREFERENCE) | Cells data will be maintained in compact format to decrease the memory cost. On other hand, the compact data also may cause higher time cost, especially when updating the cells data, or accessing cells/rows randomly | v8.0.0 |
|  | [MemorySetting.FILE\_CACHE](../../com.aspose.cells/memorysetting\#FILE-CACHE) | När detta läge används för ett kalkylblad i en arbetsbok, bör [Workbook.dispose()](../../com.aspose.cells/workbook\#dispose--) anropas i slutet av arbetet för att frigöra alla resurser såsom temporära filer. |
 
Att slumpmässigt komma åt celler ger dålig prestanda eftersom data måste läsas/uppdateras slumpmässigt och upprepade gånger (så pekaren i filen ändras därefter och I/O‑operationer krävs upprepade gånger). Om möjligt, vänligen åtkomst data sekventiellt (rad för rad).
 
När data i en rad/cell ändras kan data i andra celler/rader också påverkas (t.ex. att data flyttas/förflyttas till andra platser för att allokera tillräckligt med utrymme för den ändrade datan). Så varje förändring av varje data kräver synkronisering av andra befintliga objekt (såsom rad‑ eller cell‑objekt). För att få bättre prestanda, vänligen håll inte flera rader/celler samtidigt. Att bearbeta dem en åt gången minskar datasynkroniseringen för dem så prestandan kan förbättras något. | v25.7     |

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setMultiThreadReading(boolean value) {#setMultiThreadReading-boolean-}
```
public void setMultiThreadReading(boolean value)
```


Anger om cellernas datamodell ska stödja flerdelat läsning. Standardvärdet för denna egenskap är falskt.

**Remarks**

Om det finns flera trådar som läser Row/Cell-objekt i den här samlingen samtidigt, bör den här egenskapen sättas till true, annars kan oväntade resultat produceras. Att stödja Multi-Thread-läsning kan försämra prestandan för åtkomst av Row/Cell-objekt från den här samlingen. Observera att vissa funktioner inte kan stödja Multi-Thread-läsning, såsom formateringsvärden (av [Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--), [Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), osv.). Så även om den här egenskapen är satt till true, kan dessa API:er fortfarande ge oväntade resultat för Multi-Thread-läsning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPreserveString(boolean value) {#setPreserveString-boolean-}
```
public void setPreserveString(boolean value)
```


Anger ett värde som indikerar om alla arbetsbladsvärden bevaras som strängar. Standard är falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setRowHeight(int row, double height) {#setRowHeight-int-double-}
```
public void setRowHeight(int row, double height)
```


Ställer in höjden på den angivna raden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex. |
| höjd | double | Radhöjd i punktenheter. Den bör vara mellan 0 och 409,5. |

### setRowHeightInch(int row, double inches) {#setRowHeightInch-int-double-}
```
public void setRowHeightInch(int row, double inches)
```


Ställer in radhöjd i tum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex. |
| tum | double | Antal tum. Den bör vara mellan 0 och 409,5/72. |

### setRowHeightPixel(int row, int pixels) {#setRowHeightPixel-int-int-}
```
public void setRowHeightPixel(int row, int pixels)
```


Ställer in radhöjd i pixlar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex. |
| pixlar | int | Antal pixlar. |

### setStandardHeight(double value) {#setStandardHeight-double-}
```
public void setStandardHeight(double value)
```


Ställer in standardradhöjd i detta kalkylblad, i punktenheter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setStandardHeightInch(double value) {#setStandardHeightInch-double-}
```
public void setStandardHeightInch(double value)
```


Ställer in standardradhöjden i detta kalkylblad, i enheten tum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setStandardHeightPixels(int value) {#setStandardHeightPixels-int-}
```
public void setStandardHeightPixels(int value)
```


Ställer in standardradhöjden i detta kalkylblad, i enheten pixlar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setStandardWidth(double value) {#setStandardWidth-double-}
```
public void setStandardWidth(double value)
```


Ställer in standardkolumnbredden i kalkylbladet, i enheten tecken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setStandardWidthInch(double value) {#setStandardWidthInch-double-}
```
public void setStandardWidthInch(double value)
```


Ställer in standardkolumnbredden i kalkylbladet, i enheten tum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setStandardWidthPixels(int value) {#setStandardWidthPixels-int-}
```
public void setStandardWidthPixels(int value)
```


Ställer in standardkolumnbredden i kalkylbladet, i enheten pixlar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setStyle(Style value) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style value)
```


Ställer in standardstilen för kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setViewColumnWidthPixel(int column, int pixels) {#setViewColumnWidthPixel-int-int-}
```
public void setViewColumnWidthPixel(int column, int pixels)
```


Ställer in kolumnens bredd i olika vyer.

**Remarks**

Om den aktuella vystyper är [ViewType.PAGE\_LAYOUT\_VIEW](../../com.aspose.cells/viewtype\#PAGE-LAYOUT-VIEW), är kolumnens bredd densamma som den utskrivna bredden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindexet. |
| pixlar | int | Bredden i pixelenheter. |

### showGroupDetail(boolean isVertical, int index) {#showGroupDetail-boolean-int-}
```
public void showGroupDetail(boolean isVertical, int index)
```


Expanderar de grupperade raderna/kolumnerna.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isVertical | boolean | Sant, expanderar de grupperade raderna. |
| index | int | Rad-/kolumnindexet |

### subtotal(CellArea ca, int groupBy, int function, int[] totalList) {#subtotal-com.aspose.cells.CellArea-int-int-int---}
```
public void subtotal(CellArea ca, int groupBy, int function, int[] totalList)
```


Skapar delsummer för intervallet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Området |
| groupBy | int | Fältet att gruppera efter, som ett nollbaserat heltalsavstånd |
| function | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Subtotalfunktionen. |
| totalList | int[] | En array av nollbaserade fältavstånd som anger de fält till vilka subtotalerna läggs till. |

### subtotal(CellArea ca, int groupBy, int function, int[] totalList, boolean replace, boolean pageBreaks, boolean summaryBelowData) {#subtotal-com.aspose.cells.CellArea-int-int-int---boolean-boolean-boolean-}
```
public void subtotal(CellArea ca, int groupBy, int function, int[] totalList, boolean replace, boolean pageBreaks, boolean summaryBelowData)
```


Skapar delsummer för intervallet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Området |
| groupBy | int | Fältet att gruppera efter, som ett nollbaserat heltalsavstånd |
| function | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Subtotalfunktionen. |
| totalList | int[] | En array av nollbaserade fältavstånd som anger de fält till vilka subtotalerna läggs till. |
| replace | boolean | Anger om de nuvarande subtotalerna ska ersättas |
| pageBreaks | boolean | Anger om en sidbrytning ska läggas till mellan grupper |
| summaryBelowData | boolean | Anger om en sammanfattning ska läggas till under data. |

### textToColumns(int row, int column, int totalRows, TxtLoadOptions options) {#textToColumns-int-int-int-com.aspose.cells.TxtLoadOptions-}
```
public int textToColumns(int row, int column, int totalRows, TxtLoadOptions options)
```


Delar upp innehållet i angiven kolumn i flera kolumner..

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindexet. |
| kolumn | int | Kolumnindexet. |
| totalRows | int | Antalet rader. |
| options | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | Delningsalternativen. |

**Returns:**
int – Totalt antal kolumner för de delade värdena.
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


Tar bort sammanslagning av ett angivet område med sammanslagna celler.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstRow | int | Första raden i detta intervall (nollbaserat) |
| firstColumn | int | Första kolumnen i detta intervall (nollbaserat) |
| totalRows | int | Antal rader (enbaserat) |
| totalColumns | int | Antal kolumner (enbaserat) |

### ungroupColumns(int firstIndex, int lastIndex) {#ungroupColumns-int-int-}
```
public void ungroupColumns(int firstIndex, int lastIndex)
```


Avgrupperar kolumner.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstIndex | int | Det första kolumnindexet som ska avgrupperas. |
| lastIndex | int | Det sista kolumnindexet som ska avgrupperas. |

### ungroupRows(int firstIndex, int lastIndex) {#ungroupRows-int-int-}
```
public void ungroupRows(int firstIndex, int lastIndex)
```


Avgrupperar rader.

**Remarks**

Tar endast bort yttre gruppinformation.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstIndex | int | Det första radindexet som ska avgrupperas. |
| lastIndex | int | Det sista radindexet som ska avgrupperas. |

### ungroupRows(int firstIndex, int lastIndex, boolean isAll) {#ungroupRows-int-int-boolean-}
```
public void ungroupRows(int firstIndex, int lastIndex, boolean isAll)
```


Avgrupperar rader.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstIndex | int | Det första radindexet som ska avgrupperas. |
| lastIndex | int | Det sista radindexet som ska avgrupperas. |
| isAll | boolean | Sant, tar bort all grupperad information. Annars tas den yttre gruppinformationen bort. |

### unhideColumn(int column, double width) {#unhideColumn-int-double-}
```
public void unhideColumn(int column, double width)
```


Visar en kolumn

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindex. |
| bredd | double | Kolumnbredd. |

### unhideColumns(int column, int totalColumns, double width) {#unhideColumns-int-int-double-}
```
public void unhideColumns(int column, int totalColumns, double width)
```


Visa flera kolumner.

**Remarks**

Tillämpar endast kolumnbredden på dolda kolumner.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindex. |
| totalColumns | int | Kolumnnummer |
| bredd | double | Kolumnbredd. |

### unhideRow(int row, double height) {#unhideRow-int-double-}
```
public void unhideRow(int row, double height)
```


Visar en rad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex. |
| höjd | double | Radhöjd. Radvärdet ändras endast när raden är dold och det angivna höjdvärdet är positivt. |

### unhideRows(int row, int totalRows, double height) {#unhideRows-int-int-double-}
```
public void unhideRows(int row, int totalRows, double height)
```


Visar de dolda raderna.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindexet. |
| totalRows | int | Radnumret. |
| höjd | double | Radhöjd. Radvärdet ändras endast när raden är dold och det angivna höjdvärdet är positivt. |

### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

