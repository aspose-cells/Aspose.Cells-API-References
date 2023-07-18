---
title: LightCellsDataProvider
second_title: Aspose.Cells for Java API Reference
description: Represents Data provider for saving large spreadsheet files in light weight mode.
type: docs
url: /java/com.aspose.cells/lightcellsdataprovider/
---
```
public interface LightCellsDataProvider
```

Represents Data provider for saving large spreadsheet files in light weight mode.

**Remarks**

When saving a workbook by this mode, [startSheet(int)](../../com.aspose.cells/lightcellsdataprovider\#startSheet-int-) will be checked when saving every worksheet in the workbook. For one sheet, if [startSheet(int)](../../com.aspose.cells/lightcellsdataprovider\#startSheet-int-) gives true, then all data and properties of rows/cells of this sheet to be saved will be provided by the implementation of this interface. In the first place, [nextRow()](../../com.aspose.cells/lightcellsdataprovider\#nextRow--) will be called to get the next row index to be saved. If a valid row index is returned(the row index must be in ascending order for the rows to be saved), then a Row object representing this row will be provided for implementation to set its properties by [startRow(Row)](../../com.aspose.cells/lightcellsdataprovider\#startRow-Row-). For one row, [nextCell()](../../com.aspose.cells/lightcellsdataprovider\#nextCell--) will be checked firstly. If a valid column index be returned(the column index must be in ascending order for all cells of one row to be saved), then a Cell object representing this cell will be provided for implementation to set its data and properties by [startCell(Cell)](../../com.aspose.cells/lightcellsdataprovider\#startCell-Cell-). After data of this cell is set, this cell will be saved directly to the generated spreadsheet file and the next cell will be checked and processed.
## Methods

| Method | Description |
| --- | --- |
| [isGatherString()](#isGatherString--) | Checks whether the current string value of cell needs to be gathered into a global pool. |
| [nextCell()](#nextCell--) | Gets next cell to be saved. |
| [nextRow()](#nextRow--) | Gets the next row to be saved. |
| [startCell(Cell cell)](#startCell-com.aspose.cells.Cell-) | Starts to save data of one cell. |
| [startRow(Row row)](#startRow-com.aspose.cells.Row-) | Starts to save data of one row. |
| [startSheet(int sheetIndex)](#startSheet-int-) | Starts to save a worksheet. |
### isGatherString() {#isGatherString--}
```
public abstract boolean isGatherString()
```


Checks whether the current string value of cell needs to be gathered into a global pool.

**Remarks**

Gathering string values will take advantage only when there are many duplicated string values for the cells provided by this implementation. In this situation gathering string will save much memory and generate smaller resultant file. If there are many string values for the cells provided by LightCellsDataProvider but few of them are same, gathering string will cost more memory and time and has no advantage for the resultant file.

**Returns:**
boolean - true if string value need to be gathered into a global pool for the resultant file.
### nextCell() {#nextCell--}
```
public abstract int nextCell()
```


Gets next cell to be saved.

**Remarks**

It will be called at the beginning of saving one cell.

**Returns:**
int - column index of the next cell to be saved. -1 means the end of current row data has been reached and no further cell of current row to be saved.
### nextRow() {#nextRow--}
```
public abstract int nextRow()
```


Gets the next row to be saved.

**Remarks**

It will be called at the beginning of saving a row and its cells data(before [startRow(Row)](../../com.aspose.cells/lightcellsdataprovider\#startRow-Row-)).

**Returns:**
int - the next row index to be saved. -1 means the end of current sheet data has been reached and no further row of current sheet to be saved.
### startCell(Cell cell) {#startCell-com.aspose.cells.Cell-}
```
public abstract void startCell(Cell cell)
```


Starts to save data of one cell.

**Remarks**

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | Cell object for implementation to fill data. Its column index is the returned value of latest call of [nextCell()](../../com.aspose.cells/lightcellsdataprovider\#nextCell--). If the cell has been initialized in the inner cells model, the existed cell object will be used. Otherwise a temporary Cell object will be used for implementation to fill data. |

### startRow(Row row) {#startRow-com.aspose.cells.Row-}
```
public abstract void startRow(Row row)
```


Starts to save data of one row.

**Remarks**

It will be called at the beginning of saving a row and its cells data. If current row has some custom properties such as height, style, ...etc., implementation should set those properties to given Row object here.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | [Row](../../com.aspose.cells/row) | Row object for implementation to fill data. Its row index is the returned value of latest call of [nextRow()](../../com.aspose.cells/lightcellsdataprovider\#nextRow--). If the row has been initialized in the inner cells model, the existing row object will be used. Otherwise a temporary Row object will be used for implementation to fill data. |

### startSheet(int sheetIndex) {#startSheet-int-}
```
public abstract boolean startSheet(int sheetIndex)
```


Starts to save a worksheet.

**Remarks**

It will be called at the beginning of saving a worksheet during saving a workbook. If the provider needs to refer to *`sheetIndex`* later in startRow(Row) or startCell(Cell) method, that is, if the process needs to know which worksheet is being processed, the implementation should retain the *`sheetIndex`* value here.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | int | index of current sheet to be saved. |

**Returns:**
boolean - true if this provider will provide data for the given sheet; false if given sheet should use its normal data model(Cells).
