---
title: Worksheet
second_title: Aspose.Cells for Java API Reference
description: Encapsulates the object that represents a single worksheet.
type: docs
url: /java/com.aspose.cells/worksheet/
---

**Inheritance:**
java.lang.Object
```
public class Worksheet
```

Encapsulates the object that represents a single worksheet.

**Example**

The following example shows how to freeze panes and insert hyperlink to worksheet with .Net or VB.

```
Workbook workbook = new Workbook();
 
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Freeze panes at "AS40" with 10 rows and 10 columns
         sheet.freezePanes("AS40", 10, 10);
 
         //Add a hyperlink in Cell A1
         sheet.getHyperlinks().add("A1", 1, 1, "http://www.aspose.com");
```
## Methods

| Method | Description |
| --- | --- |
| [addPageBreaks(String cellName)](#addPageBreaks-java.lang.String-) | Adds page break. |
| [advancedFilter(boolean isFilter, String listRange, String criteriaRange, String copyTo, boolean uniqueRecordOnly)](#advancedFilter-boolean-java.lang.String-java.lang.String-java.lang.String-boolean-) | Filters data using complex criteria. |
| [autoFitColumn(int columnIndex)](#autoFitColumn-int-) | Autofits the column width. |
| [autoFitColumn(int columnIndex, int firstRow, int lastRow)](#autoFitColumn-int-int-int-) | Autofits the column width. |
| [autoFitColumns()](#autoFitColumns--) | Autofits all columns in this worksheet. |
| [autoFitColumns(AutoFitterOptions options)](#autoFitColumns-com.aspose.cells.AutoFitterOptions-) | Autofits all columns in this worksheet. |
| [autoFitColumns(int firstColumn, int lastColumn)](#autoFitColumns-int-int-) | Autofits the columns width. |
| [autoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options)](#autoFitColumns-int-int-com.aspose.cells.AutoFitterOptions-) | Autofits the columns width. |
| [autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn)](#autoFitColumns-int-int-int-int-) | Autofits the columns width. |
| [autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, AutoFitterOptions options)](#autoFitColumns-int-int-int-int-com.aspose.cells.AutoFitterOptions-) | Autofits the columns width. |
| [autoFitRow(int rowIndex)](#autoFitRow-int-) | Autofits the row height. |
| [autoFitRow(int rowIndex, int firstColumn, int lastColumn)](#autoFitRow-int-int-int-) | Autofits the row height. |
| [autoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options)](#autoFitRow-int-int-int-com.aspose.cells.AutoFitterOptions-) | Autofits the row height. |
| [autoFitRow(int startRow, int endRow, int startColumn, int endColumn)](#autoFitRow-int-int-int-int-) | Autofits row height in a rectangle range. |
| [autoFitRows()](#autoFitRows--) | Autofits all rows in this worksheet. |
| [autoFitRows(boolean onlyAuto)](#autoFitRows-boolean-) | Autofits all rows in this worksheet. |
| [autoFitRows(AutoFitterOptions options)](#autoFitRows-com.aspose.cells.AutoFitterOptions-) | Autofits all rows in this worksheet. |
| [autoFitRows(int startRow, int endRow)](#autoFitRows-int-int-) | Autofits row height in a range. |
| [autoFitRows(int startRow, int endRow, AutoFitterOptions options)](#autoFitRows-int-int-com.aspose.cells.AutoFitterOptions-) | Autofits row height in a range. |
| [calculateArrayFormula(String formula, CalculationOptions opts)](#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-) | Calculates a formula as array formula. |
| [calculateArrayFormula(String formula, CalculationOptions opts, int maxRowCount, int maxColumnCount)](#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-int-int-) | Calculates a formula as array formula. |
| [calculateFormula(boolean recursive, boolean ignoreError, ICustomFunction customFunction)](#calculateFormula-boolean-boolean-com.aspose.cells.ICustomFunction-) | Calculates all formulas in this worksheet. |
| [calculateFormula(CalculationOptions options, boolean recursive)](#calculateFormula-com.aspose.cells.CalculationOptions-boolean-) | Calculates all formulas in this worksheet. |
| [calculateFormula(String formula)](#calculateFormula-java.lang.String-) | Calculates a formula. |
| [calculateFormula(String formula, CalculationOptions opts)](#calculateFormula-java.lang.String-com.aspose.cells.CalculationOptions-) | Calculates a formula. |
| [clearComments()](#clearComments--) | Clears all comments in designer spreadsheet. |
| [closeAccessCache(int opts)](#closeAccessCache-int-) | Closes the session that uses caches to access the data in this worksheet. |
| [copy(Worksheet sourceSheet)](#copy-com.aspose.cells.Worksheet-) | Copies contents and formats from another worksheet. |
| [copy(Worksheet sourceSheet, CopyOptions copyOptions)](#copy-com.aspose.cells.Worksheet-com.aspose.cells.CopyOptions-) | Copies contents and formats from another worksheet. |
| [dispose()](#dispose--) | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [freezePanes(int row, int column, int freezedRows, int freezedColumns)](#freezePanes-int-int-int-int-) | Freezes panes at the specified cell in the worksheet. |
| [freezePanes(String cellName, int freezedRows, int freezedColumns)](#freezePanes-java.lang.String-int-int-) | Freezes panes at the specified cell in the worksheet. |
| [getActiveCell()](#getActiveCell--) | Gets the active cell in the worksheet. |
| [getAllowEditRanges()](#getAllowEditRanges--) | Gets the allow edit range collection in the worksheet. |
| [getAutoFilter()](#getAutoFilter--) | Represents auto filter for the specified worksheet. |
| [getBackgroundImage()](#getBackgroundImage--) | Gets worksheet background image. |
| [getCellWatches()](#getCellWatches--) | Gets collection of cells on this worksheet being watched in the 'watch window'. |
| [getCells()](#getCells--) | Gets the [Cells](../../com.aspose.cells/cells) collection. |
| [getCharts()](#getCharts--) | Gets a [Chart](../../com.aspose.cells/chart) collection |
| [getCheckBoxes()](#getCheckBoxes--) | Gets a [CheckBox](../../com.aspose.cells/checkbox) collection. |
| [getClass()](#getClass--) |  |
| [getCodeName()](#getCodeName--) | Gets worksheet code name. |
| [getComments()](#getComments--) | Gets the [Comment](../../com.aspose.cells/comment) collection. |
| [getConditionalFormattings()](#getConditionalFormattings--) | Gets the ConditionalFormattings in the worksheet. |
| [getCustomProperties()](#getCustomProperties--) | Gets an object representing the identifier information associated with a worksheet. |
| [getDisplayRightToLeft()](#getDisplayRightToLeft--) | Indicates if the specified worksheet is displayed from right to left instead of from left to right. |
| [getDisplayZeros()](#getDisplayZeros--) | True if zero values are displayed. |
| [getErrorCheckOptions()](#getErrorCheckOptions--) | Gets error check setting applied on certain ranges. |
| [getFirstVisibleColumn()](#getFirstVisibleColumn--) | Represents first visible column index. |
| [getFirstVisibleRow()](#getFirstVisibleRow--) | Represents first visible row index. |
| [getFreezedPanes()](#getFreezedPanes--) | Gets the freeze panes. |
| [getHorizontalPageBreaks()](#getHorizontalPageBreaks--) | Gets the [HorizontalPageBreakCollection](../../com.aspose.cells/horizontalpagebreakcollection) collection. |
| [getHyperlinks()](#getHyperlinks--) | Gets the [HyperlinkCollection](../../com.aspose.cells/hyperlinkcollection) collection. |
| [getIndex()](#getIndex--) | Gets the index of sheet in the worksheet collection. |
| [getListObjects()](#getListObjects--) | Gets all ListObjects in this worksheet. |
| [getName()](#getName--) | Gets the name of the worksheet. |
| [getOleObjects()](#getOleObjects--) | Represents a collection of [OleObject](../../com.aspose.cells/oleobject) in a worksheet. |
| [getOutline()](#getOutline--) | Gets the outline on this worksheet. |
| [getPageSetup()](#getPageSetup--) | Represents the page setup description in this sheet. |
| [getPaneState()](#getPaneState--) | Indicates whether the pane has horizontal or vertical splits, and whether those splits are frozen. |
| [getPanes()](#getPanes--) | Gets the window panes. |
| [getPictures()](#getPictures--) | Gets a [Picture](../../com.aspose.cells/picture) collection. |
| [getPivotTables()](#getPivotTables--) | Gets all pivot tables in this worksheet. |
| [getPrintingPageBreaks(ImageOrPrintOptions options)](#getPrintingPageBreaks-com.aspose.cells.ImageOrPrintOptions-) | Gets automatic page breaks. |
| [getProtection()](#getProtection--) | Represents the various types of protection options available for a worksheet. |
| [getQueryTables()](#getQueryTables--) | Gets [QueryTableCollection](../../com.aspose.cells/querytablecollection) in the worksheet. |
| [getScenarios()](#getScenarios--) | Gets the collection of [Scenario](../../com.aspose.cells/scenario). |
| [getSelectedRanges()](#getSelectedRanges--) | Gets selected ranges of cells in the designer spreadsheet. |
| [getShapes()](#getShapes--) | Returns all drawing shapes in this worksheet. |
| [getShowFormulas()](#getShowFormulas--) | Indicates whether to show formulas or their results. |
| [getSlicers()](#getSlicers--) | Get the Slicer collection in the worksheet |
| [getSmartTagSetting()](#getSmartTagSetting--) | Gets all [SmartTagCollection](../../com.aspose.cells/smarttagcollection) objects of the worksheet. |
| [getSparklineGroupCollection()](#getSparklineGroupCollection--) | Gets the sparkline group collection in the worksheet. |
| [getSparklineGroups()](#getSparklineGroups--) | Gets the sparkline groups in the worksheet. |
| [getTabColor()](#getTabColor--) | Represents worksheet tab color. |
| [getTabId()](#getTabId--) | Specifies the internal identifier for the sheet. |
| [getTextBoxes()](#getTextBoxes--) | Gets a [TextBox](../../com.aspose.cells/textbox) collection. |
| [getTimelines()](#getTimelines--) | Get the Timeline collection in the worksheet |
| [getTransitionEntry()](#getTransitionEntry--) | Indicates whether the Transition Formula Entry (Lotus compatibility) option is enabled. |
| [getTransitionEvaluation()](#getTransitionEvaluation--) | Indicates whether the Transition Formula Evaluation (Lotus compatibility) option is enabled. |
| [getType()](#getType--) | Represents worksheet type. |
| [getUniqueId()](#getUniqueId--) | Gets the unique id, it is same as \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\}. |
| [getValidations()](#getValidations--) | Gets the data validation setting collection in the worksheet. |
| [getVerticalPageBreaks()](#getVerticalPageBreaks--) | Gets the [VerticalPageBreakCollection](../../com.aspose.cells/verticalpagebreakcollection) collection. |
| [getViewType()](#getViewType--) | Gets the view type. |
| [getVisibilityType()](#getVisibilityType--) | Indicates the visible state for this sheet. |
| [getWorkbook()](#getWorkbook--) | Gets the workbook object which contains this sheet. |
| [getZoom()](#getZoom--) | Represents the scaling factor in percentage. |
| [hasAutofilter()](#hasAutofilter--) | Indicates whether this worksheet has auto filter. |
| [hashCode()](#hashCode--) |  |
| [isGridlinesVisible()](#isGridlinesVisible--) | Gets a value indicating whether the gridlines are visible.Default is true. |
| [isOutlineShown()](#isOutlineShown--) | Indicates whether to show outline. |
| [isPageBreakPreview()](#isPageBreakPreview--) | Indicates whether the specified worksheet is shown in normal view or page break preview. |
| [isProtected()](#isProtected--) | Indicates if the worksheet is protected. |
| [isRowColumnHeadersVisible()](#isRowColumnHeadersVisible--) | Gets a value indicating whether the worksheet will display row and column headers. |
| [isRulerVisible()](#isRulerVisible--) | Indicates whether the ruler is visible. |
| [isSelected()](#isSelected--) | Indicates whether this worksheet is selected when the workbook is opened. |
| [isVisible()](#isVisible--) | Represents if the worksheet is visible. |
| [moveTo(int index)](#moveTo-int-) | Moves the sheet to another location in the spreadsheet. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [protect(int type)](#protect-int-) | Protects worksheet. |
| [protect(int type, String password, String oldPassword)](#protect-int-java.lang.String-java.lang.String-) | Protects worksheet. |
| [refreshPivotTables()](#refreshPivotTables--) | Refreshes all the PivotTables in this Worksheet. |
| [removeAllDrawingObjects()](#removeAllDrawingObjects--) | Removes all drawing objects in this worksheet. |
| [removeAutoFilter()](#removeAutoFilter--) | Removes the auto filter of the worksheet. |
| [removeSplit()](#removeSplit--) | Removes split window. |
| [replace(String oldString, String newString)](#replace-java.lang.String-java.lang.String-) | Replaces all cells' text with a new string. |
| [selectRange(int startRow, int startColumn, int totalRows, int totalColumns, boolean removeOthers)](#selectRange-int-int-int-int-boolean-) | Selects a range. |
| [setActiveCell(String value)](#setActiveCell-java.lang.String-) | Sets the active cell in the worksheet. |
| [setBackground(byte[] pictureData)](#setBackground-byte---) | Sets worksheet background image. |
| [setBackgroundImage(byte[] value)](#setBackgroundImage-byte---) | Sets worksheet background image. |
| [setCodeName(String value)](#setCodeName-java.lang.String-) | Gets worksheet code name. |
| [setDisplayRightToLeft(boolean value)](#setDisplayRightToLeft-boolean-) | Indicates if the specified worksheet is displayed from right to left instead of from left to right. |
| [setDisplayZeros(boolean value)](#setDisplayZeros-boolean-) | True if zero values are displayed. |
| [setFirstVisibleColumn(int value)](#setFirstVisibleColumn-int-) | Represents first visible column index. |
| [setFirstVisibleRow(int value)](#setFirstVisibleRow-int-) | Represents first visible row index. |
| [setGridlinesVisible(boolean value)](#setGridlinesVisible-boolean-) | Sets a value indicating whether the gridlines are visible.Default is true. |
| [setName(String value)](#setName-java.lang.String-) | Sets the name of the worksheet. |
| [setOutlineShown(boolean value)](#setOutlineShown-boolean-) | Indicates whether to show outline. |
| [setPageBreakPreview(boolean value)](#setPageBreakPreview-boolean-) | Indicates whether the specified worksheet is shown in normal view or page break preview. |
| [setRowColumnHeadersVisible(boolean value)](#setRowColumnHeadersVisible-boolean-) | Sets a value indicating whether the worksheet will display row and column headers. |
| [setRulerVisible(boolean value)](#setRulerVisible-boolean-) | Indicates whether the ruler is visible. |
| [setSelected(boolean value)](#setSelected-boolean-) | Indicates whether this worksheet is selected when the workbook is opened. |
| [setShowFormulas(boolean value)](#setShowFormulas-boolean-) | Indicates whether to show formulas or their results. |
| [setTabColor(Color value)](#setTabColor-com.aspose.cells.Color-) | Represents worksheet tab color. |
| [setTabId(int value)](#setTabId-int-) | Specifies the internal identifier for the sheet. |
| [setTransitionEntry(boolean value)](#setTransitionEntry-boolean-) | Indicates whether the Transition Formula Entry (Lotus compatibility) option is enabled. |
| [setTransitionEvaluation(boolean value)](#setTransitionEvaluation-boolean-) | Indicates whether the Transition Formula Evaluation (Lotus compatibility) option is enabled. |
| [setType(int value)](#setType-int-) | Represents worksheet type. |
| [setUniqueId(String value)](#setUniqueId-java.lang.String-) | Sets the unique id, it is same as \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\}. |
| [setViewType(int value)](#setViewType-int-) | Sets the view type. |
| [setVisibilityType(int value)](#setVisibilityType-int-) | Indicates the visible state for this sheet. |
| [setVisible(boolean value)](#setVisible-boolean-) | Represents if the worksheet is visible. |
| [setVisible(boolean isVisible, boolean ignoreError)](#setVisible-boolean-boolean-) | Sets the visible options. |
| [setZoom(int value)](#setZoom-int-) | Represents the scaling factor in percentage. |
| [split()](#split--) | Splits window. |
| [startAccessCache(int opts)](#startAccessCache-int-) | Starts the session that uses caches to access the data in this worksheet. |
| [toString()](#toString--) | Returns a string represents the current Worksheet object. |
| [unFreezePanes()](#unFreezePanes--) | Unfreezes panes in the worksheet. |
| [unprotect()](#unprotect--) | Unprotects worksheet. |
| [unprotect(String password)](#unprotect-java.lang.String-) | Unprotects worksheet. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
| [xmlMapQuery(String path, XmlMap xmlMap)](#xmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-) | Query cell areas that mapped/linked to the specific path of xml map. |
### addPageBreaks(String cellName) {#addPageBreaks-java.lang.String-}
```
public void addPageBreaks(String cellName)
```


Adds page break.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String |  |

### advancedFilter(boolean isFilter, String listRange, String criteriaRange, String copyTo, boolean uniqueRecordOnly) {#advancedFilter-boolean-java.lang.String-java.lang.String-java.lang.String-boolean-}
```
public void advancedFilter(boolean isFilter, String listRange, String criteriaRange, String copyTo, boolean uniqueRecordOnly)
```


Filters data using complex criteria.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isFilter | boolean | Indicates whether filtering the list in place. |
| listRange | java.lang.String | The list range. |
| criteriaRange | java.lang.String | The criteria range. |
| copyTo | java.lang.String | The range where copying data to. |
| uniqueRecordOnly | boolean | Only displaying or copying unique rows. |

### autoFitColumn(int columnIndex) {#autoFitColumn-int-}
```
public void autoFitColumn(int columnIndex)
```


Autofits the column width. AutoFitColumn is an imprecise function.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | int | Column index. |

### autoFitColumn(int columnIndex, int firstRow, int lastRow) {#autoFitColumn-int-int-int-}
```
public void autoFitColumn(int columnIndex, int firstRow, int lastRow)
```


Autofits the column width. This method autofits a row based on content in a range of cells within the row.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | int | Column index. |
| firstRow | int | First row index. |
| lastRow | int | Last row index. |

### autoFitColumns() {#autoFitColumns--}
```
public void autoFitColumns()
```


Autofits all columns in this worksheet.

### autoFitColumns(AutoFitterOptions options) {#autoFitColumns-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitColumns(AutoFitterOptions options)
```


Autofits all columns in this worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | The auto fitting options |

### autoFitColumns(int firstColumn, int lastColumn) {#autoFitColumns-int-int-}
```
public void autoFitColumns(int firstColumn, int lastColumn)
```


Autofits the columns width. AutoFitColumn is an imprecise function.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstColumn | int | First column index. |
| lastColumn | int | Last column index. |

### autoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options) {#autoFitColumns-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options)
```


Autofits the columns width. AutoFitColumn is an imprecise function.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstColumn | int | First column index. |
| lastColumn | int | Last column index. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | The auto fitting options |

### autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn) {#autoFitColumns-int-int-int-int-}
```
public void autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn)
```


Autofits the columns width. AutoFitColumn is an imprecise function.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | int | First row index. |
| firstColumn | int | First column index. |
| lastRow | int | Last row index. |
| lastColumn | int | Last column index. |

### autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, AutoFitterOptions options) {#autoFitColumns-int-int-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, AutoFitterOptions options)
```


Autofits the columns width. AutoFitColumn is an imprecise function.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | int | First row index. |
| firstColumn | int | First column index. |
| lastRow | int | Last row index. |
| lastColumn | int | Last column index. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | The auto fitting options |

### autoFitRow(int rowIndex) {#autoFitRow-int-}
```
public void autoFitRow(int rowIndex)
```


Autofits the row height. AutoFitRow is an imprecise function.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int | Row index. |

### autoFitRow(int rowIndex, int firstColumn, int lastColumn) {#autoFitRow-int-int-int-}
```
public void autoFitRow(int rowIndex, int firstColumn, int lastColumn)
```


Autofits the row height. This method autofits a row based on content in a range of cells within the row.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int | Row index. |
| firstColumn | int | First column index. |
| lastColumn | int | Last column index. |

### autoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options) {#autoFitRow-int-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options)
```


Autofits the row height. This method autofits a row based on content in a range of cells within the row.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int | Row index. |
| firstColumn | int | First column index. |
| lastColumn | int | Last column index. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | The auto fitter options |

### autoFitRow(int startRow, int endRow, int startColumn, int endColumn) {#autoFitRow-int-int-int-int-}
```
public void autoFitRow(int startRow, int endRow, int startColumn, int endColumn)
```


Autofits row height in a rectangle range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | int | Start row index. |
| endRow | int | End row index. |
| startColumn | int | Start column index. |
| endColumn | int | End column index. |

### autoFitRows() {#autoFitRows--}
```
public void autoFitRows()
```


Autofits all rows in this worksheet.

### autoFitRows(boolean onlyAuto) {#autoFitRows-boolean-}
```
public void autoFitRows(boolean onlyAuto)
```


Autofits all rows in this worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| onlyAuto | boolean | True,only autofits the row height when row height is not customed. |

### autoFitRows(AutoFitterOptions options) {#autoFitRows-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitRows(AutoFitterOptions options)
```


Autofits all rows in this worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | The auto fitter options |

### autoFitRows(int startRow, int endRow) {#autoFitRows-int-int-}
```
public void autoFitRows(int startRow, int endRow)
```


Autofits row height in a range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | int | Start row index. |
| endRow | int | End row index. |

### autoFitRows(int startRow, int endRow, AutoFitterOptions options) {#autoFitRows-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitRows(int startRow, int endRow, AutoFitterOptions options)
```


Autofits row height in a range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | int | Start row index. |
| endRow | int | End row index. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | The options of auto fitter. |

### calculateArrayFormula(String formula, CalculationOptions opts) {#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-}
```
public Object[][] calculateArrayFormula(String formula, CalculationOptions opts)
```


Calculates a formula as array formula.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | Formula to be calculated. |
| opts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Options for calculating formula |

**Returns:**
java.lang.Object[][]
### calculateArrayFormula(String formula, CalculationOptions opts, int maxRowCount, int maxColumnCount) {#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-int-int-}
```
public Object[][] calculateArrayFormula(String formula, CalculationOptions opts, int maxRowCount, int maxColumnCount)
```


Calculates a formula as array formula. The formula will be taken as dynamic array formula to calculate the dimension and result. User specified maximum dimension is used for cases that the calculated result is large data set (for example, the calculated result may correspond to a whole row or column data) but user does not need so large an array according to business requirement or for performance consideration.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | Formula to be calculated. |
| opts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Options for calculating formula |
| maxRowCount | int | the maximum row count of resultant data. -1 means it will be determined by the formula itself. |
| maxColumnCount | int | the maximum column count of resultant data. -1 means it is determined by the formula itself. |

**Returns:**
java.lang.Object[][] - Calculated formula result.
### calculateFormula(boolean recursive, boolean ignoreError, ICustomFunction customFunction) {#calculateFormula-boolean-boolean-com.aspose.cells.ICustomFunction-}
```
public void calculateFormula(boolean recursive, boolean ignoreError, ICustomFunction customFunction)
```


Calculates all formulas in this worksheet. NOTE: This member is now obsolete. Instead, please use CalculateFormula(CalculationOptions, bool) method. This method will be removed 12 months later since August 2020. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| recursive | boolean | True means if the worksheet' cells depend on the cells of other worksheets, the dependent cells in other worksheets will be calculated too. False means all the formulas in the worksheet have been calculated and the values are right. |
| ignoreError | boolean | Indicates if hide the error in calculating formulas. The error may be unsupported function, external links, etc. |
| customFunction | [ICustomFunction](../../com.aspose.cells/icustomfunction) | The custom formula calculation functions to extend the calculation engine. |

### calculateFormula(CalculationOptions options, boolean recursive) {#calculateFormula-com.aspose.cells.CalculationOptions-boolean-}
```
public void calculateFormula(CalculationOptions options, boolean recursive)
```


Calculates all formulas in this worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Options for calculation |
| recursive | boolean | True means if the worksheet' cells depend on the cells of other worksheets, the dependent cells in other worksheets will be calculated too. False means all the formulas in the worksheet have been calculated and the values are right. |

### calculateFormula(String formula) {#calculateFormula-java.lang.String-}
```
public Object calculateFormula(String formula)
```


Calculates a formula.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | Formula to be calculated. |

**Returns:**
java.lang.Object - Calculated formula result.
### calculateFormula(String formula, CalculationOptions opts) {#calculateFormula-java.lang.String-com.aspose.cells.CalculationOptions-}
```
public Object calculateFormula(String formula, CalculationOptions opts)
```


Calculates a formula.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | Formula to be calculated. |
| opts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Options for calculating formula |

**Returns:**
java.lang.Object - Calculated formula result.
### clearComments() {#clearComments--}
```
public void clearComments()
```


Clears all comments in designer spreadsheet.

### closeAccessCache(int opts) {#closeAccessCache-int-}
```
public void closeAccessCache(int opts)
```


Closes the session that uses caches to access the data in this worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). options of data access |

### copy(Worksheet sourceSheet) {#copy-com.aspose.cells.Worksheet-}
```
public void copy(Worksheet sourceSheet)
```


Copies contents and formats from another worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceSheet | [Worksheet](../../com.aspose.cells/worksheet) | Source worksheet. |

### copy(Worksheet sourceSheet, CopyOptions copyOptions) {#copy-com.aspose.cells.Worksheet-com.aspose.cells.CopyOptions-}
```
public void copy(Worksheet sourceSheet, CopyOptions copyOptions)
```


Copies contents and formats from another worksheet. You can copy data from another worksheet in the same file or another file. However, this method does not support to copy drawing objects, such as comments, images and charts.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceSheet | [Worksheet](../../com.aspose.cells/worksheet) | Source worksheet. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) |  |

### dispose() {#dispose--}
```
public void dispose()
```


Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### freezePanes(int row, int column, int freezedRows, int freezedColumns) {#freezePanes-int-int-int-int-}
```
public void freezePanes(int row, int column, int freezedRows, int freezedColumns)
```


Freezes panes at the specified cell in the worksheet.

Row index and column index cannot all be zero. Number of rows and number of columns also cannot all be zero.

The first two parameters specify the froze position and the last two parameters specify the area frozen on the left top pane.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index. |
| column | int | Column index. |
| freezedRows | int | Number of visible rows in top pane, no more than row index. |
| freezedColumns | int | Number of visible columns in left pane, no more than column index. |

### freezePanes(String cellName, int freezedRows, int freezedColumns) {#freezePanes-java.lang.String-int-int-}
```
public void freezePanes(String cellName, int freezedRows, int freezedColumns)
```


Freezes panes at the specified cell in the worksheet. Row index and column index cannot all be zero. Number of rows and number of columns also cannot all be zero.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String | Cell name. |
| freezedRows | int | Number of visible rows in top pane, no more than row index. |
| freezedColumns | int | Number of visible columns in left pane, no more than column index. |

### getActiveCell() {#getActiveCell--}
```
public String getActiveCell()
```


Gets the active cell in the worksheet.

**Returns:**
java.lang.String
### getAllowEditRanges() {#getAllowEditRanges--}
```
public ProtectedRangeCollection getAllowEditRanges()
```


Gets the allow edit range collection in the worksheet.

**Returns:**
[ProtectedRangeCollection](../../com.aspose.cells/protectedrangecollection)
### getAutoFilter() {#getAutoFilter--}
```
public AutoFilter getAutoFilter()
```


Represents auto filter for the specified worksheet.

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getBackgroundImage() {#getBackgroundImage--}
```
public byte[] getBackgroundImage()
```


Gets worksheet background image.

**Returns:**
byte[]
### getCellWatches() {#getCellWatches--}
```
public CellWatchCollection getCellWatches()
```


Gets collection of cells on this worksheet being watched in the 'watch window'.

**Returns:**
[CellWatchCollection](../../com.aspose.cells/cellwatchcollection)
### getCells() {#getCells--}
```
public Cells getCells()
```


Gets the [Cells](../../com.aspose.cells/cells) collection.

**Returns:**
[Cells](../../com.aspose.cells/cells)
### getCharts() {#getCharts--}
```
public ChartCollection getCharts()
```


Gets a [Chart](../../com.aspose.cells/chart) collection

**Returns:**
[ChartCollection](../../com.aspose.cells/chartcollection)
### getCheckBoxes() {#getCheckBoxes--}
```
public CheckBoxCollection getCheckBoxes()
```


Gets a [CheckBox](../../com.aspose.cells/checkbox) collection.

**Returns:**
[CheckBoxCollection](../../com.aspose.cells/checkboxcollection)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCodeName() {#getCodeName--}
```
public String getCodeName()
```


Gets worksheet code name.

**Returns:**
java.lang.String
### getComments() {#getComments--}
```
public CommentCollection getComments()
```


Gets the [Comment](../../com.aspose.cells/comment) collection.

**Returns:**
[CommentCollection](../../com.aspose.cells/commentcollection)
### getConditionalFormattings() {#getConditionalFormattings--}
```
public ConditionalFormattingCollection getConditionalFormattings()
```


Gets the ConditionalFormattings in the worksheet.

**Returns:**
[ConditionalFormattingCollection](../../com.aspose.cells/conditionalformattingcollection)
### getCustomProperties() {#getCustomProperties--}
```
public CustomPropertyCollection getCustomProperties()
```


Gets an object representing the identifier information associated with a worksheet. Worksheet.CustomProperties provide a preferred mechanism for storing arbitrary data. It supports legacy third-party document components, as well as those situations that have a stringent need for binary parts.

**Returns:**
[CustomPropertyCollection](../../com.aspose.cells/custompropertycollection)
### getDisplayRightToLeft() {#getDisplayRightToLeft--}
```
public boolean getDisplayRightToLeft()
```


Indicates if the specified worksheet is displayed from right to left instead of from left to right. Default is false.

**Returns:**
boolean
### getDisplayZeros() {#getDisplayZeros--}
```
public boolean getDisplayZeros()
```


True if zero values are displayed.

**Returns:**
boolean
### getErrorCheckOptions() {#getErrorCheckOptions--}
```
public ErrorCheckOptionCollection getErrorCheckOptions()
```


Gets error check setting applied on certain ranges.

**Returns:**
[ErrorCheckOptionCollection](../../com.aspose.cells/errorcheckoptioncollection)
### getFirstVisibleColumn() {#getFirstVisibleColumn--}
```
public int getFirstVisibleColumn()
```


Represents first visible column index.

**Returns:**
int
### getFirstVisibleRow() {#getFirstVisibleRow--}
```
public int getFirstVisibleRow()
```


Represents first visible row index.

**Returns:**
int
### getFreezedPanes() {#getFreezedPanes--}
```
public int[] getFreezedPanes()
```


Gets the freeze panes.

**Returns:**
int[] - Return null means the worksheet is not frozen 0:Row index;1:column;2:freezedRows;3:freezedRows
### getHorizontalPageBreaks() {#getHorizontalPageBreaks--}
```
public HorizontalPageBreakCollection getHorizontalPageBreaks()
```


Gets the [HorizontalPageBreakCollection](../../com.aspose.cells/horizontalpagebreakcollection) collection.

**Returns:**
[HorizontalPageBreakCollection](../../com.aspose.cells/horizontalpagebreakcollection)
### getHyperlinks() {#getHyperlinks--}
```
public HyperlinkCollection getHyperlinks()
```


Gets the [HyperlinkCollection](../../com.aspose.cells/hyperlinkcollection) collection.

**Returns:**
[HyperlinkCollection](../../com.aspose.cells/hyperlinkcollection)
### getIndex() {#getIndex--}
```
public int getIndex()
```


Gets the index of sheet in the worksheet collection.

**Returns:**
int
### getListObjects() {#getListObjects--}
```
public ListObjectCollection getListObjects()
```


Gets all ListObjects in this worksheet.

**Returns:**
[ListObjectCollection](../../com.aspose.cells/listobjectcollection)
### getName() {#getName--}
```
public String getName()
```


Gets the name of the worksheet. The max length of sheet name is 31. And you cannot assign same name(case insensitive) to two worksheets. For example, you cannot set "SheetName1" to the first worksheet and set "SHEETNAME1" to the second worksheet.

**Returns:**
java.lang.String
### getOleObjects() {#getOleObjects--}
```
public OleObjectCollection getOleObjects()
```


Represents a collection of [OleObject](../../com.aspose.cells/oleobject) in a worksheet.

**Returns:**
[OleObjectCollection](../../com.aspose.cells/oleobjectcollection)
### getOutline() {#getOutline--}
```
public Outline getOutline()
```


Gets the outline on this worksheet.

**Returns:**
[Outline](../../com.aspose.cells/outline)
### getPageSetup() {#getPageSetup--}
```
public PageSetup getPageSetup()
```


Represents the page setup description in this sheet.

**Returns:**
[PageSetup](../../com.aspose.cells/pagesetup)
### getPaneState() {#getPaneState--}
```
public int getPaneState()
```


Indicates whether the pane has horizontal or vertical splits, and whether those splits are frozen. [PaneStateType](../../com.aspose.cells/panestatetype).

**Returns:**
int
### getPanes() {#getPanes--}
```
public PaneCollection getPanes()
```


Gets the window panes. If the window is not split or frozen.

**Returns:**
[PaneCollection](../../com.aspose.cells/panecollection)
### getPictures() {#getPictures--}
```
public PictureCollection getPictures()
```


Gets a [Picture](../../com.aspose.cells/picture) collection.

**Returns:**
[PictureCollection](../../com.aspose.cells/picturecollection)
### getPivotTables() {#getPivotTables--}
```
public PivotTableCollection getPivotTables()
```


Gets all pivot tables in this worksheet.

**Returns:**
[PivotTableCollection](../../com.aspose.cells/pivottablecollection)
### getPrintingPageBreaks(ImageOrPrintOptions options) {#getPrintingPageBreaks-com.aspose.cells.ImageOrPrintOptions-}
```
public CellArea[] getPrintingPageBreaks(ImageOrPrintOptions options)
```


Gets automatic page breaks. Each cell area represents a paper.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | The print options |

**Returns:**
com.aspose.cells.CellArea[] - The automatic page breaks areas.
### getProtection() {#getProtection--}
```
public Protection getProtection()
```


Represents the various types of protection options available for a worksheet. Supports advanced protection options in ExcelXP and above version. This property can protect worksheet in all versions of Excel file and support advanced protection options in ExcelXP and above version.

**Returns:**
[Protection](../../com.aspose.cells/protection)
### getQueryTables() {#getQueryTables--}
```
public QueryTableCollection getQueryTables()
```


Gets [QueryTableCollection](../../com.aspose.cells/querytablecollection) in the worksheet.

**Returns:**
[QueryTableCollection](../../com.aspose.cells/querytablecollection)
### getScenarios() {#getScenarios--}
```
public ScenarioCollection getScenarios()
```


Gets the collection of [Scenario](../../com.aspose.cells/scenario).

**Returns:**
[ScenarioCollection](../../com.aspose.cells/scenariocollection)
### getSelectedRanges() {#getSelectedRanges--}
```
public ArrayList getSelectedRanges()
```


Gets selected ranges of cells in the designer spreadsheet.

**Returns:**
java.util.ArrayList - An ArrayList which contains selected ranges.
### getShapes() {#getShapes--}
```
public ShapeCollection getShapes()
```


Returns all drawing shapes in this worksheet.

**Returns:**
[ShapeCollection](../../com.aspose.cells/shapecollection)
### getShowFormulas() {#getShowFormulas--}
```
public boolean getShowFormulas()
```


Indicates whether to show formulas or their results.

**Returns:**
boolean
### getSlicers() {#getSlicers--}
```
public SlicerCollection getSlicers()
```


Get the Slicer collection in the worksheet

**Returns:**
[SlicerCollection](../../com.aspose.cells/slicercollection)
### getSmartTagSetting() {#getSmartTagSetting--}
```
public SmartTagSetting getSmartTagSetting()
```


Gets all [SmartTagCollection](../../com.aspose.cells/smarttagcollection) objects of the worksheet.

**Returns:**
[SmartTagSetting](../../com.aspose.cells/smarttagsetting)
### getSparklineGroupCollection() {#getSparklineGroupCollection--}
```
public SparklineGroupCollection getSparklineGroupCollection()
```


Gets the sparkline group collection in the worksheet. NOTE: This member is now obsolete. Instead, please use Worksheet.SparklineGroups property. This property will be removed 12 months later since November 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
[SparklineGroupCollection](../../com.aspose.cells/sparklinegroupcollection)
### getSparklineGroups() {#getSparklineGroups--}
```
public SparklineGroupCollection getSparklineGroups()
```


Gets the sparkline groups in the worksheet.

**Returns:**
[SparklineGroupCollection](../../com.aspose.cells/sparklinegroupcollection)
### getTabColor() {#getTabColor--}
```
public Color getTabColor()
```


Represents worksheet tab color. This feature is only supported in ExcelXP(Excel2002) and later versions. If you save file as Excel97 or Excel2000 format, it will be omitted.

**Returns:**
[Color](../../com.aspose.cells/color)
### getTabId() {#getTabId--}
```
public int getTabId()
```


Specifies the internal identifier for the sheet.

**Returns:**
int
### getTextBoxes() {#getTextBoxes--}
```
public TextBoxCollection getTextBoxes()
```


Gets a [TextBox](../../com.aspose.cells/textbox) collection.

**Returns:**
[TextBoxCollection](../../com.aspose.cells/textboxcollection)
### getTimelines() {#getTimelines--}
```
public TimelineCollection getTimelines()
```


Get the Timeline collection in the worksheet

**Returns:**
[TimelineCollection](../../com.aspose.cells/timelinecollection)
### getTransitionEntry() {#getTransitionEntry--}
```
public boolean getTransitionEntry()
```


Indicates whether the Transition Formula Entry (Lotus compatibility) option is enabled.

**Returns:**
boolean
### getTransitionEvaluation() {#getTransitionEvaluation--}
```
public boolean getTransitionEvaluation()
```


Indicates whether the Transition Formula Evaluation (Lotus compatibility) option is enabled.

**Returns:**
boolean
### getType() {#getType--}
```
public int getType()
```


Represents worksheet type. [SheetType](../../com.aspose.cells/sheettype).

**Returns:**
int
### getUniqueId() {#getUniqueId--}
```
public String getUniqueId()
```


Gets the unique id, it is same as \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\}.

**Returns:**
java.lang.String
### getValidations() {#getValidations--}
```
public ValidationCollection getValidations()
```


Gets the data validation setting collection in the worksheet.

**Returns:**
[ValidationCollection](../../com.aspose.cells/validationcollection)
### getVerticalPageBreaks() {#getVerticalPageBreaks--}
```
public VerticalPageBreakCollection getVerticalPageBreaks()
```


Gets the [VerticalPageBreakCollection](../../com.aspose.cells/verticalpagebreakcollection) collection.

**Returns:**
[VerticalPageBreakCollection](../../com.aspose.cells/verticalpagebreakcollection)
### getViewType() {#getViewType--}
```
public int getViewType()
```


Gets the view type. [ViewType](../../com.aspose.cells/viewtype).

**Returns:**
int
### getVisibilityType() {#getVisibilityType--}
```
public int getVisibilityType()
```


Indicates the visible state for this sheet. [VisibilityType](../../com.aspose.cells/visibilitytype).

**Returns:**
int
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Gets the workbook object which contains this sheet.

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### getZoom() {#getZoom--}
```
public int getZoom()
```


Represents the scaling factor in percentage. It should be between 10 and 400. Please set the view type first.

**Returns:**
int
### hasAutofilter() {#hasAutofilter--}
```
public boolean hasAutofilter()
```


Indicates whether this worksheet has auto filter.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isGridlinesVisible() {#isGridlinesVisible--}
```
public boolean isGridlinesVisible()
```


Gets a value indicating whether the gridlines are visible.Default is true.

**Returns:**
boolean
### isOutlineShown() {#isOutlineShown--}
```
public boolean isOutlineShown()
```


Indicates whether to show outline.

**Returns:**
boolean
### isPageBreakPreview() {#isPageBreakPreview--}
```
public boolean isPageBreakPreview()
```


Indicates whether the specified worksheet is shown in normal view or page break preview.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Indicates if the worksheet is protected.

**Returns:**
boolean
### isRowColumnHeadersVisible() {#isRowColumnHeadersVisible--}
```
public boolean isRowColumnHeadersVisible()
```


Gets a value indicating whether the worksheet will display row and column headers. Default is true.

**Returns:**
boolean
### isRulerVisible() {#isRulerVisible--}
```
public boolean isRulerVisible()
```


Indicates whether the ruler is visible. This property is only applied for page break preview.

**Returns:**
boolean
### isSelected() {#isSelected--}
```
public boolean isSelected()
```


Indicates whether this worksheet is selected when the workbook is opened.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Represents if the worksheet is visible.

**Returns:**
boolean
### moveTo(int index) {#moveTo-int-}
```
public void moveTo(int index)
```


Moves the sheet to another location in the spreadsheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | Destination sheet index. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### protect(int type) {#protect-int-}
```
public void protect(int type)
```


Protects worksheet. This method protects worksheet without password. It can protect worksheet in all versions of Excel file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [ProtectionType](../../com.aspose.cells/protectiontype). Protection type. |

### protect(int type, String password, String oldPassword) {#protect-int-java.lang.String-java.lang.String-}
```
public void protect(int type, String password, String oldPassword)
```


Protects worksheet. This method can protect worksheet in all versions of Excel file.

**Example**

```
//Instantiating a Workbook object
         Workbook excel = new Workbook("template.xlsx");
         //Accessing the first worksheet in the Excel file
         Worksheet worksheet = excel.getWorksheets().get(0);
         //Protecting the worksheet with a password
         worksheet.protect(ProtectionType.ALL, "aspose", null);
         //Saving the modified Excel file in default (that is Excel 20003) format
         excel.save("output.xls");
         //Closing the file stream to free all resources
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [ProtectionType](../../com.aspose.cells/protectiontype). Protection type. |
| password | java.lang.String | Password. |
| oldPassword | java.lang.String | If the worksheet is already protected by a password, please supply the old password. Otherwise, you can set a null value or blank string to this parameter. |

### refreshPivotTables() {#refreshPivotTables--}
```
public void refreshPivotTables()
```


Refreshes all the PivotTables in this Worksheet.

### removeAllDrawingObjects() {#removeAllDrawingObjects--}
```
public void removeAllDrawingObjects()
```


Removes all drawing objects in this worksheet.

### removeAutoFilter() {#removeAutoFilter--}
```
public void removeAutoFilter()
```


Removes the auto filter of the worksheet.

### removeSplit() {#removeSplit--}
```
public void removeSplit()
```


Removes split window.

### replace(String oldString, String newString) {#replace-java.lang.String-java.lang.String-}
```
public int replace(String oldString, String newString)
```


Replaces all cells' text with a new string.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| oldString | java.lang.String | Old string value. |
| newString | java.lang.String | New string value. |

**Returns:**
int
### selectRange(int startRow, int startColumn, int totalRows, int totalColumns, boolean removeOthers) {#selectRange-int-int-int-int-boolean-}
```
public void selectRange(int startRow, int startColumn, int totalRows, int totalColumns, boolean removeOthers)
```


Selects a range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | int | The start row. |
| startColumn | int | The start column |
| totalRows | int | The number of rows. |
| totalColumns | int | The number of columns |
| removeOthers | boolean | True means removing other selected range and only select this range. |

### setActiveCell(String value) {#setActiveCell-java.lang.String-}
```
public void setActiveCell(String value)
```


Sets the active cell in the worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setBackground(byte[] pictureData) {#setBackground-byte---}
```
public void setBackground(byte[] pictureData)
```


Sets worksheet background image. NOTE: This member is now obsolete. Instead, please use Worksheet.BackgroundImage property. This property will be removed 12 months later since August 2016. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pictureData | byte[] | Picture data. |

### setBackgroundImage(byte[] value) {#setBackgroundImage-byte---}
```
public void setBackgroundImage(byte[] value)
```


Sets worksheet background image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte[] |  |

### setCodeName(String value) {#setCodeName-java.lang.String-}
```
public void setCodeName(String value)
```


Gets worksheet code name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setDisplayRightToLeft(boolean value) {#setDisplayRightToLeft-boolean-}
```
public void setDisplayRightToLeft(boolean value)
```


Indicates if the specified worksheet is displayed from right to left instead of from left to right. Default is false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDisplayZeros(boolean value) {#setDisplayZeros-boolean-}
```
public void setDisplayZeros(boolean value)
```


True if zero values are displayed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFirstVisibleColumn(int value) {#setFirstVisibleColumn-int-}
```
public void setFirstVisibleColumn(int value)
```


Represents first visible column index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setFirstVisibleRow(int value) {#setFirstVisibleRow-int-}
```
public void setFirstVisibleRow(int value)
```


Represents first visible row index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setGridlinesVisible(boolean value) {#setGridlinesVisible-boolean-}
```
public void setGridlinesVisible(boolean value)
```


Sets a value indicating whether the gridlines are visible.Default is true.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Sets the name of the worksheet. The max length of sheet name is 31. And you cannot assign same name(case insensitive) to two worksheets. For example, you cannot set "SheetName1" to the first worksheet and set "SHEETNAME1" to the second worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setOutlineShown(boolean value) {#setOutlineShown-boolean-}
```
public void setOutlineShown(boolean value)
```


Indicates whether to show outline.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setPageBreakPreview(boolean value) {#setPageBreakPreview-boolean-}
```
public void setPageBreakPreview(boolean value)
```


Indicates whether the specified worksheet is shown in normal view or page break preview.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setRowColumnHeadersVisible(boolean value) {#setRowColumnHeadersVisible-boolean-}
```
public void setRowColumnHeadersVisible(boolean value)
```


Sets a value indicating whether the worksheet will display row and column headers. Default is true.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setRulerVisible(boolean value) {#setRulerVisible-boolean-}
```
public void setRulerVisible(boolean value)
```


Indicates whether the ruler is visible. This property is only applied for page break preview.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```


Indicates whether this worksheet is selected when the workbook is opened.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowFormulas(boolean value) {#setShowFormulas-boolean-}
```
public void setShowFormulas(boolean value)
```


Indicates whether to show formulas or their results.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setTabColor(Color value) {#setTabColor-com.aspose.cells.Color-}
```
public void setTabColor(Color value)
```


Represents worksheet tab color. This feature is only supported in ExcelXP(Excel2002) and later versions. If you save file as Excel97 or Excel2000 format, it will be omitted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setTabId(int value) {#setTabId-int-}
```
public void setTabId(int value)
```


Specifies the internal identifier for the sheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTransitionEntry(boolean value) {#setTransitionEntry-boolean-}
```
public void setTransitionEntry(boolean value)
```


Indicates whether the Transition Formula Entry (Lotus compatibility) option is enabled.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setTransitionEvaluation(boolean value) {#setTransitionEvaluation-boolean-}
```
public void setTransitionEvaluation(boolean value)
```


Indicates whether the Transition Formula Evaluation (Lotus compatibility) option is enabled.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Represents worksheet type. [SheetType](../../com.aspose.cells/sheettype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setUniqueId(String value) {#setUniqueId-java.lang.String-}
```
public void setUniqueId(String value)
```


Sets the unique id, it is same as \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\}.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setViewType(int value) {#setViewType-int-}
```
public void setViewType(int value)
```


Sets the view type. [ViewType](../../com.aspose.cells/viewtype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setVisibilityType(int value) {#setVisibilityType-int-}
```
public void setVisibilityType(int value)
```


Indicates the visible state for this sheet. [VisibilityType](../../com.aspose.cells/visibilitytype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Represents if the worksheet is visible.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setVisible(boolean isVisible, boolean ignoreError) {#setVisible-boolean-boolean-}
```
public void setVisible(boolean isVisible, boolean ignoreError)
```


Sets the visible options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isVisible | boolean | Whether the worksheet is visible |
| ignoreError | boolean | Whether to ignore error if this option is not valid. |

### setZoom(int value) {#setZoom-int-}
```
public void setZoom(int value)
```


Represents the scaling factor in percentage. It should be between 10 and 400. Please set the view type first.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### split() {#split--}
```
public void split()
```


Splits window.

### startAccessCache(int opts) {#startAccessCache-int-}
```
public void startAccessCache(int opts)
```


Starts the session that uses caches to access the data in this worksheet. After finishing the access to the data, [Workbook.closeAccessCache(int)](../../com.aspose.cells/workbook\#closeAccessCache-int-) should be invoked with same options to clear all caches and recover normal access mode.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). options of data access |

### toString() {#toString--}
```
public String toString()
```


Returns a string represents the current Worksheet object.

**Returns:**
java.lang.String - 
### unFreezePanes() {#unFreezePanes--}
```
public void unFreezePanes()
```


Unfreezes panes in the worksheet.

### unprotect() {#unprotect--}
```
public void unprotect()
```


Unprotects worksheet. This method unprotects worksheet which is protected without password.

### unprotect(String password) {#unprotect-java.lang.String-}
```
public void unprotect(String password)
```


Unprotects worksheet. If the worksheet is protected without a password, you can set a null value or blank string to password parameter.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | Password |

### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

### xmlMapQuery(String path, XmlMap xmlMap) {#xmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-}
```
public ArrayList xmlMapQuery(String path, XmlMap xmlMap)
```


Query cell areas that mapped/linked to the specific path of xml map.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | xml element path |
| xmlMap | [XmlMap](../../com.aspose.cells/xmlmap) | Specify an xml map if you want to query for the specific path within a specific map |

**Returns:**
java.util.ArrayList - [CellArea](../../com.aspose.cells/cellarea) list that mapped/linked to the specific path of xml map, an empty list is returned if nothing is mapped/linked.
