---
title: "Worksheet"
linktitle: "Worksheet"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Encapsulates the object that represents a single worksheet."
type: docs
weight: 4730
url: /nodejs/aspose.cells/worksheet/
---

## Worksheet class

Encapsulates the object that represents a single worksheet.

## Methods

| Name | Description |
| --- | --- |
| [addPageBreaks(cellName)](#addpagebreaks) | Adds page break. |
| [advancedFilter(isFilter, listRange, criteriaRange, copyTo, uniqueRecordOnly)](#advancedfilter) | Filters data using complex criteria. |
| [autoFitColumn(columnIndex, firstRow, lastRow)](#autofitcolumn) | Autofits the column width. This method autofits a row based on content in a range of cells within the row. |
| [autoFitColumn(columnIndex)](#autofitcolumn-1) | Autofits the column width. AutoFitColumn is an imprecise function. |
| [autoFitColumns()](#autofitcolumns) | Autofits all columns in this worksheet. |
| [autoFitColumns(options)](#autofitcolumns-1) | Autofits all columns in this worksheet. |
| [autoFitColumns(firstColumn, lastColumn)](#autofitcolumns-2) | Autofits the columns width. AutoFitColumn is an imprecise function. |
| [autoFitColumns(firstColumn, lastColumn, options)](#autofitcolumns-3) | Autofits the columns width. AutoFitColumn is an imprecise function. |
| [autoFitColumns(firstRow, firstColumn, lastRow, lastColumn)](#autofitcolumns-4) | Autofits the columns width. AutoFitColumn is an imprecise function. |
| [autoFitColumns(firstRow, firstColumn, lastRow, lastColumn, options)](#autofitcolumns-5) | Autofits the columns width. AutoFitColumn is an imprecise function. |
| [autoFitRow(rowIndex, firstColumn, lastColumn)](#autofitrow) | Autofits the row height. This method autofits a row based on content in a range of cells within the row. |
| [autoFitRow(rowIndex, firstColumn, lastColumn, options)](#autofitrow-1) | Autofits the row height. This method autofits a row based on content in a range of cells within the row. |
| [autoFitRow(startRow, endRow, startColumn, endColumn)](#autofitrow-2) | Autofits row height in a rectangle range. |
| [autoFitRow(rowIndex)](#autofitrow-3) | Autofits the row height. AutoFitRow is an imprecise function. |
| [autoFitRows()](#autofitrows) | Autofits all rows in this worksheet. |
| [autoFitRows(onlyAuto)](#autofitrows-1) | Autofits all rows in this worksheet. |
| [autoFitRows(options)](#autofitrows-2) | Autofits all rows in this worksheet. |
| [autoFitRows(startRow, endRow)](#autofitrows-3) | Autofits row height in a range. |
| [autoFitRows(startRow, endRow, options)](#autofitrows-4) | Autofits row height in a range. |
| [calculateArrayFormula(formula, opts)](#calculatearrayformula) | Calculates a formula as array formula. |
| [calculateArrayFormula(formula, opts, maxRowCount, maxColumnCount)](#calculatearrayformula-1) | Calculates a formula as array formula. The formula will be taken as dynamic array formula to calculate the dimension and |
| [calculateArrayFormula(formula, pOpts, cOpts, baseCellRow, baseCellColumn, maxRowCount, maxColumnCount, calculationData)](#calculatearrayformula-2) | Calculates a formula as array formula. The formula will be taken as dynamic array formula to calculate the dimension and |
| [calculateFormula(formula)](#calculateformula) | Calculates a formula. |
| [calculateFormula(formula, opts)](#calculateformula-1) | Calculates a formula expression directly. The formula will be calculated just like it has been set to cell A1. And the f |
| [calculateFormula(formula, pOpts, cOpts, baseCellRow, baseCellColumn, calculationData)](#calculateformula-2) | Calculates a formula expression directly. The formula will be calculated just like it has been set to the specified base |
| [calculateFormula(options, recursive)](#calculateformula-3) | Calculates all formulas in this worksheet. |
| [clearComments()](#clearcomments) | Clears all comments in designer spreadsheet. |
| [closeAccessCache(opts)](#closeaccesscache) | Closes the session that uses caches to access the data in this worksheet. |
| [convertFormulaReferenceStyle(formula, toR1C1, baseCellRow, baseCellColumn)](#convertformulareferencestyle) | Converts the formula reference style. |
| [copy(sourceSheet)](#copy) | Copies contents and formats from another worksheet. |
| [copy(sourceSheet, copyOptions)](#copy-1) | Copies contents and formats from another worksheet. You can copy data from another worksheet in the same file or another |
| [dispose()](#dispose) | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [filter()](#filter) |  |
| [freezePanes(row, column, freezedRows, freezedColumns)](#freezepanes) | Freezes panes at the specified cell in the worksheet. Row index and column index cannot all be zero. Number of rows and  |
| [freezePanes(cellName, freezedRows, freezedColumns)](#freezepanes-1) | Freezes panes at the specified cell in the worksheet. Row index and column index cannot all be zero. Number of rows and  |
| [getActiveCell()](#getactivecell) | Gets or sets the active cell in the worksheet. |
| [getAdvancedFilter()](#getadvancedfilter) | Gets the settings of advanced filter. |
| [getAllPictures()](#getallpictures) |  |
| [getAllowEditRanges()](#getalloweditranges) | Gets the allow edit range collection in the worksheet. |
| [getAutoFilter()](#getautofilter) | Represents auto filter for the specified worksheet. |
| [getBackgroundImage()](#getbackgroundimage) | Gets and sets worksheet background image. |
| [getCellWatches()](#getcellwatches) | Gets collection of cells on this worksheet being watched in the 'watch window'. |
| [getCells()](#getcells) | Gets the Cells collection. |
| [getCharts()](#getcharts) | Gets a Chart collection |
| [getCheckBoxes()](#getcheckboxes) | Gets a CheckBox collection. |
| [getCodeName()](#getcodename) | Gets worksheet code name. |
| [getComments()](#getcomments) | Gets the Comment collection. |
| [getConditionalFormattings()](#getconditionalformattings) | Gets the ConditionalFormattings in the worksheet. |
| [getCustomProperties()](#getcustomproperties) | Gets an object representing the identifier information associated with a worksheet. Worksheet.CustomProperties provide a |
| [getDisplayRightToLeft()](#getdisplayrighttoleft) | Indicates if the specified worksheet is displayed from right to left instead of from left to right. Default is false. |
| [getDisplayZeros()](#getdisplayzeros) | True if zero values are displayed. |
| [getErrorCheckOptions()](#geterrorcheckoptions) | Gets error check setting applied on certain ranges. |
| [getFirstVisibleColumn()](#getfirstvisiblecolumn) | Represents first visible column index. |
| [getFirstVisibleRow()](#getfirstvisiblerow) | Represents first visible row index. |
| [getFreezedPanes()](#getfreezedpanes) | Gets the freeze panes. |
| [getGridlineColor()](#getgridlinecolor) |  |
| [getHorizontalPageBreaks()](#gethorizontalpagebreaks) | Gets the HorizontalPageBreakCollection collection. |
| [getHyperlinks()](#gethyperlinks) | Gets the HyperlinkCollection collection. |
| [getIndex()](#getindex) | Gets the index of sheet in the worksheet collection. |
| [getListObjects()](#getlistobjects) | Gets all ListObjects in this worksheet. |
| [getName()](#getname) | Gets or sets the name of the worksheet. The max length of sheet name is 31. And you cannot assign same name(case insensi |
| [getOleObjects()](#getoleobjects) | Represents a collection of OleObject in a worksheet. |
| [getOutline()](#getoutline) | Gets the outline on this worksheet. |
| [getPageSetup()](#getpagesetup) | Represents the page setup description in this sheet. |
| [getPaneState()](#getpanestate) | Indicates whether the pane has horizontal or vertical splits, and whether those splits are frozen. The value of the prop |
| [getPanes()](#getpanes) | Gets the window panes. If the window is not split or frozen. |
| [getPictures()](#getpictures) | Gets a Picture collection. |
| [getPivotTables()](#getpivottables) | Gets all pivot tables in this worksheet. |
| [getPrintingPageBreaks(options)](#getprintingpagebreaks) | Gets automatic page breaks. Each cell area represents a paper. |
| [getProtection()](#getprotection) | Represents the various types of protection options available for a worksheet. Supports advanced protection options in Ex |
| [getQueryTables()](#getquerytables) | Gets QueryTableCollection in the worksheet. |
| [getScenarios()](#getscenarios) | Gets the collection of Scenario. |
| [getSelectedAreas()](#getselectedareas) |  |
| [getSelectedRanges()](#getselectedranges) | Gets selected ranges of cells in the designer spreadsheet. |
| [getShapes()](#getshapes) | Returns all drawing shapes in this worksheet. |
| [getShowDataTypeIcons()](#getshowdatatypeicons) |  |
| [getShowFormulas()](#getshowformulas) | Indicates whether to show formulas or their results. |
| [getSlicers()](#getslicers) | Get the Slicer collection in the worksheet |
| [getSmartTagSetting()](#getsmarttagsetting) | Gets all SmartTagCollection objects of the worksheet. |
| [getSparklineGroups()](#getsparklinegroups) | Gets the sparkline groups in the worksheet. |
| [getTabColor()](#gettabcolor) | Represents worksheet tab color. This feature is only supported in ExcelXP(Excel2002) and later versions. If you save fil |
| [getTabId()](#gettabid) | Specifies the internal identifier for the sheet. |
| [getTextBoxes()](#gettextboxes) | Gets a TextBox collection. |
| [getTimelines()](#gettimelines) | Get the Timeline collection in the worksheet |
| [getTransitionEntry()](#gettransitionentry) | Indicates whether the Transition Formula Entry (Lotus compatibility) option is enabled. |
| [getTransitionEvaluation()](#gettransitionevaluation) | Indicates whether the Transition Formula Evaluation (Lotus compatibility) option is enabled. |
| [getType()](#gettype) | Represents worksheet type. The value of the property is SheetType integer constant. |
| [getUniqueId()](#getuniqueid) | Gets and sets the unique id, it is same as {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. |
| [getValidations()](#getvalidations) | Gets the data validation setting collection in the worksheet. |
| [getVerticalPageBreaks()](#getverticalpagebreaks) | Gets the VerticalPageBreakCollection collection. |
| [getViewType()](#getviewtype) | Gets and sets the view type. The value of the property is ViewType integer constant. |
| [getVisibilityType()](#getvisibilitytype) | Indicates the visible state for this sheet. The value of the property is VisibilityType integer constant. |
| [getWorkbook()](#getworkbook) | Gets the workbook object which contains this sheet. |
| [getZoom()](#getzoom) | Represents the scaling factor in percentage. It should be between 10 and 400. Please set the view type first. |
| [hasAutofilter()](#hasautofilter) | Indicates whether this worksheet has auto filter. |
| [isGridlinesVisible()](#isgridlinesvisible) | Gets or sets a value indicating whether the gridlines are visible.Default is true. |
| [isOutlineShown()](#isoutlineshown) | Indicates whether to show outline. |
| [isPageBreakPreview()](#ispagebreakpreview) | Indicates whether the specified worksheet is shown in normal view or page break preview. |
| [isProtected()](#isprotected) | Indicates if the worksheet is protected. |
| [isRowColumnHeadersVisible()](#isrowcolumnheadersvisible) | Gets or sets a value indicating whether the worksheet will display row and column headers. Default is true. |
| [isRulerVisible()](#isrulervisible) | Indicates whether the ruler is visible. This property is only applied for page break preview. |
| [isSelected()](#isselected) | Indicates whether this worksheet is selected when the workbook is opened. |
| [isVisible()](#isvisible) | Represents if the worksheet is visible. |
| [moveTo(index)](#moveto) | Moves the sheet to another location in the spreadsheet. |
| [protect(type)](#protect) | Protects worksheet. This method protects worksheet without password. It can protect worksheet in all versions of Excel f |
| [protect(type, password, oldPassword)](#protect-1) | Protects worksheet. This method can protect worksheet in all versions of Excel file. |
| [refreshPivotTables()](#refreshpivottables) | Refreshes all the PivotTables in this Worksheet. |
| [refreshPivotTables(option)](#refreshpivottables-1) | Refreshes all the PivotTables in this Worksheet. |
| [removeAllDrawingObjects()](#removealldrawingobjects) | Removes all drawing objects in this worksheet. |
| [removeAutoFilter()](#removeautofilter) | Removes the auto filter of the worksheet. |
| [removeSplit()](#removesplit) | Removes split window. |
| [replace(oldString, newString)](#replace) | Replaces all cells' text with a new string. |
| [selectRange(startRow, startColumn, totalRows, totalColumns, removeOthers)](#selectrange) | Selects a range. |
| [setActiveCell()](#setactivecell) | Gets or sets the active cell in the worksheet. |
| [setBackgroundImage()](#setbackgroundimage) | Gets and sets worksheet background image. |
| [setCodeName()](#setcodename) | Gets worksheet code name. |
| [setDisplayRightToLeft()](#setdisplayrighttoleft) | Indicates if the specified worksheet is displayed from right to left instead of from left to right. Default is false. |
| [setDisplayZeros()](#setdisplayzeros) | True if zero values are displayed. |
| [setFirstVisibleColumn()](#setfirstvisiblecolumn) | Represents first visible column index. |
| [setFirstVisibleRow()](#setfirstvisiblerow) | Represents first visible row index. |
| [setGridlineColor()](#setgridlinecolor) |  |
| [setGridlinesVisible()](#setgridlinesvisible) | Gets or sets a value indicating whether the gridlines are visible.Default is true. |
| [setName()](#setname) | Gets or sets the name of the worksheet. The max length of sheet name is 31. And you cannot assign same name(case insensi |
| [setOutlineShown()](#setoutlineshown) | Indicates whether to show outline. |
| [setPageBreakPreview()](#setpagebreakpreview) | Indicates whether the specified worksheet is shown in normal view or page break preview. |
| [setRowColumnHeadersVisible()](#setrowcolumnheadersvisible) | Gets or sets a value indicating whether the worksheet will display row and column headers. Default is true. |
| [setRulerVisible()](#setrulervisible) | Indicates whether the ruler is visible. This property is only applied for page break preview. |
| [setSelected()](#setselected) | Indicates whether this worksheet is selected when the workbook is opened. |
| [setShowDataTypeIcons()](#setshowdatatypeicons) |  |
| [setShowFormulas()](#setshowformulas) | Indicates whether to show formulas or their results. |
| [setTabColor()](#settabcolor) | Represents worksheet tab color. This feature is only supported in ExcelXP(Excel2002) and later versions. If you save fil |
| [setTabId()](#settabid) | Specifies the internal identifier for the sheet. |
| [setTransitionEntry()](#settransitionentry) | Indicates whether the Transition Formula Entry (Lotus compatibility) option is enabled. |
| [setTransitionEvaluation()](#settransitionevaluation) | Indicates whether the Transition Formula Evaluation (Lotus compatibility) option is enabled. |
| [setType()](#settype) | Represents worksheet type. The value of the property is SheetType integer constant. |
| [setUniqueId()](#setuniqueid) | Gets and sets the unique id, it is same as {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. |
| [setViewType()](#setviewtype) | Gets and sets the view type. The value of the property is ViewType integer constant. |
| [setVisibilityType()](#setvisibilitytype) | Indicates the visible state for this sheet. The value of the property is VisibilityType integer constant. |
| [setVisible()](#setvisible) | Represents if the worksheet is visible. |
| [setVisible(isVisible, ignoreError)](#setvisible-1) | Sets the visible options. |
| [setZoom()](#setzoom) | Represents the scaling factor in percentage. It should be between 10 and 400. Please set the view type first. |
| [split()](#split) | Splits window. |
| [startAccessCache(opts)](#startaccesscache) | Starts the session that uses caches to access the data in this worksheet. After finishing the access to the data, closeA |
| [toString()](#tostring) | Returns a string represents the current Worksheet object. |
| [unFreezePanes()](#unfreezepanes) | Unfreezes panes in the worksheet. |
| [unprotect()](#unprotect) | Unprotects worksheet. This method unprotects worksheet which is protected without password. |
| [unprotect(password)](#unprotect-1) | Unprotects worksheet. If the worksheet is protected without a password, you can set a null value or blank string to pass |
| [xmlMapQuery(path, xmlMap)](#xmlmapquery) | Query cell areas that mapped/linked to the specific path of xml map. e.g. A xml map element structure: -RootElement \|-At |

### addPageBreaks(cellName) {#addpagebreaks}

Adds page break.

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String |  |

### advancedFilter(isFilter, listRange, criteriaRange, copyTo, uniqueRecordOnly) {#advancedfilter}

Filters data using complex criteria.

| Parameter | Type | Description |
| --- | --- | --- |
| isFilter | boolean | Indicates whether filtering the list in place. |
| listRange | String | The list range. |
| criteriaRange | String | The criteria range. |
| copyTo | String | The range where copying data to. |
| uniqueRecordOnly | boolean | Only displaying or copying unique rows. |

### autoFitColumn(columnIndex, firstRow, lastRow) {#autofitcolumn}

Autofits the column width. This method autofits a row based on content in a range of cells within the row.

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Number | Column index. |
| firstRow | Number | First row index. |
| lastRow | Number | Last row index. |

### autoFitColumn(columnIndex) {#autofitcolumn-1}

Autofits the column width. AutoFitColumn is an imprecise function.

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Number | Column index. |

### autoFitColumns() {#autofitcolumns}

Autofits all columns in this worksheet.

### autoFitColumns(options) {#autofitcolumns-1}

Autofits all columns in this worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| options | AutoFitterOptions | The auto fitting options |

### autoFitColumns(firstColumn, lastColumn) {#autofitcolumns-2}

Autofits the columns width. AutoFitColumn is an imprecise function.

| Parameter | Type | Description |
| --- | --- | --- |
| firstColumn | Number | First column index. |
| lastColumn | Number | Last column index. |

### autoFitColumns(firstColumn, lastColumn, options) {#autofitcolumns-3}

Autofits the columns width. AutoFitColumn is an imprecise function.

| Parameter | Type | Description |
| --- | --- | --- |
| firstColumn | Number | First column index. |
| lastColumn | Number | Last column index. |
| options | AutoFitterOptions | The auto fitting options |

### autoFitColumns(firstRow, firstColumn, lastRow, lastColumn) {#autofitcolumns-4}

Autofits the columns width. AutoFitColumn is an imprecise function.

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Number | First row index. |
| firstColumn | Number | First column index. |
| lastRow | Number | Last row index. |
| lastColumn | Number | Last column index. |

### autoFitColumns(firstRow, firstColumn, lastRow, lastColumn, options) {#autofitcolumns-5}

Autofits the columns width. AutoFitColumn is an imprecise function.

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Number | First row index. |
| firstColumn | Number | First column index. |
| lastRow | Number | Last row index. |
| lastColumn | Number | Last column index. |
| options | AutoFitterOptions | The auto fitting options |

### autoFitRow(rowIndex, firstColumn, lastColumn) {#autofitrow}

Autofits the row height. This method autofits a row based on content in a range of cells within the row.

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Number | Row index. |
| firstColumn | Number | First column index. |
| lastColumn | Number | Last column index. |

### autoFitRow(rowIndex, firstColumn, lastColumn, options) {#autofitrow-1}

Autofits the row height. This method autofits a row based on content in a range of cells within the row.

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Number | Row index. |
| firstColumn | Number | First column index. |
| lastColumn | Number | Last column index. |
| options | AutoFitterOptions | The auto fitter options |

### autoFitRow(startRow, endRow, startColumn, endColumn) {#autofitrow-2}

Autofits row height in a rectangle range.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Number | Start row index. |
| endRow | Number | End row index. |
| startColumn | Number | Start column index. |
| endColumn | Number | End column index. |

### autoFitRow(rowIndex) {#autofitrow-3}

Autofits the row height. AutoFitRow is an imprecise function.

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Number | Row index. |

### autoFitRows() {#autofitrows}

Autofits all rows in this worksheet.

### autoFitRows(onlyAuto) {#autofitrows-1}

Autofits all rows in this worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| onlyAuto | boolean | True,only autofits the row height when row height is not customed. |

### autoFitRows(options) {#autofitrows-2}

Autofits all rows in this worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| options | AutoFitterOptions | The auto fitter options |

### autoFitRows(startRow, endRow) {#autofitrows-3}

Autofits row height in a range.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Number | Start row index. |
| endRow | Number | End row index. |

### autoFitRows(startRow, endRow, options) {#autofitrows-4}

Autofits row height in a range.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Number | Start row index. |
| endRow | Number | End row index. |
| options | AutoFitterOptions | The options of auto fitter. |

### calculateArrayFormula(formula, opts) {#calculatearrayformula}

Calculates a formula as array formula.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | Formula to be calculated. |
| opts | CalculationOptions | Options for calculating formula |

### calculateArrayFormula(formula, opts, maxRowCount, maxColumnCount) {#calculatearrayformula-1}

Calculates a formula as array formula. The formula will be taken as dynamic array formula to calculate the dimension and result. User specified maximum dimension is used for cases that the calculated result is large data set (for example, the calculated result may correspond to a whole row or column data) but user does not need so large an array according to business requirement or for performance consideration.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | Formula to be calculated. |
| opts | CalculationOptions | Options for calculating formula |
| maxRowCount | Number | the maximum row count of resultant data. If it is non-positive or greater than the actual row count, then actual row count will be used. |
| maxColumnCount | Number | the maximum column count of resultant data. If it is non-positive or greater than the actual row count, then actual column count will be used. |

**Returns:** Array of Array of Object — `Array of Array of Object` Calculated formula result.

### calculateArrayFormula(formula, pOpts, cOpts, baseCellRow, baseCellColumn, maxRowCount, maxColumnCount, calculationData) {#calculatearrayformula-2}

Calculates a formula as array formula. The formula will be taken as dynamic array formula to calculate the dimension and result. User specified maximum dimension is used for cases that the calculated result is large data set (for example, the calculated result may correspond to a whole row or column data) but user does not need so large an array according to business requirement or for performance consideration.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | Formula to be calculated. |
| pOpts | FormulaParseOptions | Options for parsing formula |
| cOpts | CalculationOptions | Options for calculating formula |
| baseCellRow | Number | The row index of the base cell. |
| baseCellColumn | Number | The column index of the base cell. |
| maxRowCount | Number | The maximum row count of resultant data. If it is non-positive or greater than the actual row count, then actual row count will be used. |
| maxColumnCount | Number | The maximum column count of resultant data. If it is non-positive or greater than the actual row count, then actual column count will be used. |
| calculationData | CalculationData | The calculation data. It is used for the situation that user needs to calculate some static formulas when implementing custom calculation engine. For such kind of situation, user needs to specify it with the calculation data provided for |

**Returns:** Array of Array of Object — `Array of Array of Object` Calculated formula result.

### calculateFormula(formula) {#calculateformula}

Calculates a formula.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | Formula to be calculated. |

**Returns:** Object — `Object` Calculated formula result.

### calculateFormula(formula, opts) {#calculateformula-1}

Calculates a formula expression directly. The formula will be calculated just like it has been set to cell A1. And the formula will be taken as normal formula. If you need the formula be calculated as an array formula and to get an array for the calculated result, please use calculateArrayFormula(java.lang.String, com.aspose.cells.CalculationOptions) instead.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | Formula to be calculated. |
| opts | CalculationOptions | Options for calculating formula |

**Returns:** Object — `Object` Calculated result of given formula. The returned object may be of possible types of Cell.Value, or ReferredArea.

### calculateFormula(formula, pOpts, cOpts, baseCellRow, baseCellColumn, calculationData) {#calculateformula-2}

Calculates a formula expression directly. The formula will be calculated just like it has been set to the specified base cell. And the formula will be taken as normal formula. If you need the formula be calculated as an array formula and to get an array for the calculated result, please use calculateArrayFormula(java.lang.String, com.aspose.cells.FormulaParseOptions, com.aspose.cells.CalculationOptions, int, int, int, int, com.aspose.cells.CalculationData) instead.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | Formula to be calculated. |
| pOpts | FormulaParseOptions | Options for parsing formula. |
| cOpts | CalculationOptions | Options for calculating formula. |
| baseCellRow | Number | The row index of the base cell. |
| baseCellColumn | Number | The column index of the base cell. |
| calculationData | CalculationData | The calculation data. It is used for the situation that user needs to calculate some static formulas when implementing custom calculation engine. For such kind of situation, user needs to specify it with the calculation data provided for |

**Returns:** Object — `Object` Calculated result of given formula. The returned object may be of possible types of Cell.Value, or ReferredArea.

### calculateFormula(options, recursive) {#calculateformula-3}

Calculates all formulas in this worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| options | CalculationOptions | Options for calculation |
| recursive | boolean | True means if the worksheet' cells depend on the cells of other worksheets, the dependent cells in other worksheets will be calculated too. False means all the formulas in the worksheet have been calculated and the values are right. |

### clearComments() {#clearcomments}

Clears all comments in designer spreadsheet.

### closeAccessCache(opts) {#closeaccesscache}

Closes the session that uses caches to access the data in this worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| opts | Number | AccessCacheOptions |

### convertFormulaReferenceStyle(formula, toR1C1, baseCellRow, baseCellColumn) {#convertformulareferencestyle}

Converts the formula reference style.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The formula to be converted. |
| toR1C1 | boolean | Which reference style to convert the formula to. If the original formula is of A1 reference style, then this value should be true so the formula will be converted from A1 to R1C1 reference style; If the original formula is of R1C1 reference style, then this value should be false so the formula will be converted from R1C1 to A1 reference style; |
| baseCellRow | Number | The row index of the base cell. |
| baseCellColumn | Number | The column index of the base cell. |

**Returns:** String — `String` The converted formula.

### copy(sourceSheet) {#copy}

Copies contents and formats from another worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceSheet | Worksheet | Source worksheet. |

### copy(sourceSheet, copyOptions) {#copy-1}

Copies contents and formats from another worksheet. You can copy data from another worksheet in the same file or another file. However, this method does not support to copy drawing objects, such as comments, images and charts.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceSheet | Worksheet | Source worksheet. |
| copyOptions | CopyOptions |  |

### dispose() {#dispose}

Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources.

### filter() {#filter}

### freezePanes(row, column, freezedRows, freezedColumns) {#freezepanes}

Freezes panes at the specified cell in the worksheet. Row index and column index cannot all be zero. Number of rows and number of columns also cannot all be zero.The first two parameters specify the froze position and the last two parameters specify the area frozen on the left top pane.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index. |
| column | Number | Column index. |
| freezedRows | Number | Number of visible rows in top pane, no more than row index. |
| freezedColumns | Number | Number of visible columns in left pane, no more than column index. |

### freezePanes(cellName, freezedRows, freezedColumns) {#freezepanes-1}

Freezes panes at the specified cell in the worksheet. Row index and column index cannot all be zero. Number of rows and number of columns also cannot all be zero.

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Cell name. |
| freezedRows | Number | Number of visible rows in top pane, no more than row index. |
| freezedColumns | Number | Number of visible columns in left pane, no more than column index. |

### getActiveCell() {#getactivecell}

Gets or sets the active cell in the worksheet.

### getAdvancedFilter() {#getadvancedfilter}

Gets the settings of advanced filter.

**Returns:** AdvancedFilter — `AdvancedFilter`

### getAllPictures() {#getallpictures}

### getAllowEditRanges() {#getalloweditranges}

Gets the allow edit range collection in the worksheet.

### getAutoFilter() {#getautofilter}

Represents auto filter for the specified worksheet.

### getBackgroundImage() {#getbackgroundimage}

Gets and sets worksheet background image.

### getCellWatches() {#getcellwatches}

Gets collection of cells on this worksheet being watched in the 'watch window'.

### getCells() {#getcells}

Gets the Cells collection.

### getCharts() {#getcharts}

Gets a Chart collection

### getCheckBoxes() {#getcheckboxes}

Gets a CheckBox collection.

### getCodeName() {#getcodename}

Gets worksheet code name.

### getComments() {#getcomments}

Gets the Comment collection.

### getConditionalFormattings() {#getconditionalformattings}

Gets the ConditionalFormattings in the worksheet.

### getCustomProperties() {#getcustomproperties}

Gets an object representing the identifier information associated with a worksheet. Worksheet.CustomProperties provide a preferred mechanism for storing arbitrary data. It supports legacy third-party document components, as well as those situations that have a stringent need for binary parts.

### getDisplayRightToLeft() {#getdisplayrighttoleft}

Indicates if the specified worksheet is displayed from right to left instead of from left to right. Default is false.

### getDisplayZeros() {#getdisplayzeros}

True if zero values are displayed.

### getErrorCheckOptions() {#geterrorcheckoptions}

Gets error check setting applied on certain ranges.

### getFirstVisibleColumn() {#getfirstvisiblecolumn}

Represents first visible column index.

### getFirstVisibleRow() {#getfirstvisiblerow}

Represents first visible row index.

### getFreezedPanes() {#getfreezedpanes}

Gets the freeze panes.

**Returns:** Array of Number — `Array of Number` Return null means the worksheet is not frozen 0:Row index;1:column;2:freezedRows;3:freezedRows

### getGridlineColor() {#getgridlinecolor}

### getHorizontalPageBreaks() {#gethorizontalpagebreaks}

Gets the HorizontalPageBreakCollection collection.

### getHyperlinks() {#gethyperlinks}

Gets the HyperlinkCollection collection.

### getIndex() {#getindex}

Gets the index of sheet in the worksheet collection.

### getListObjects() {#getlistobjects}

Gets all ListObjects in this worksheet.

### getName() {#getname}

Gets or sets the name of the worksheet. The max length of sheet name is 31. And you cannot assign same name(case insensitive) to two worksheets. For example, you cannot set "SheetName1" to the first worksheet and set "SHEETNAME1" to the second worksheet.

### getOleObjects() {#getoleobjects}

Represents a collection of OleObject in a worksheet.

### getOutline() {#getoutline}

Gets the outline on this worksheet.

### getPageSetup() {#getpagesetup}

Represents the page setup description in this sheet.

### getPaneState() {#getpanestate}

Indicates whether the pane has horizontal or vertical splits, and whether those splits are frozen. The value of the property is PaneStateType integer constant.

### getPanes() {#getpanes}

Gets the window panes. If the window is not split or frozen.

### getPictures() {#getpictures}

Gets a Picture collection.

### getPivotTables() {#getpivottables}

Gets all pivot tables in this worksheet.

### getPrintingPageBreaks(options) {#getprintingpagebreaks}

Gets automatic page breaks. Each cell area represents a paper.

| Parameter | Type | Description |
| --- | --- | --- |
| options | ImageOrPrintOptions | The print options |

**Returns:** Array ofCellArea — `Array ofCellArea` The automatic page breaks areas.

### getProtection() {#getprotection}

Represents the various types of protection options available for a worksheet. Supports advanced protection options in ExcelXP and above version. This property can protect worksheet in all versions of Excel file and support advanced protection options in ExcelXP and above version.

### getQueryTables() {#getquerytables}

Gets QueryTableCollection in the worksheet.

### getScenarios() {#getscenarios}

Gets the collection of Scenario.

### getSelectedAreas() {#getselectedareas}

### getSelectedRanges() {#getselectedranges}

Gets selected ranges of cells in the designer spreadsheet.

**Returns:** ArrayList — `ArrayList` An java.util.ArrayList which contains selected ranges.

### getShapes() {#getshapes}

Returns all drawing shapes in this worksheet.

### getShowDataTypeIcons() {#getshowdatatypeicons}

### getShowFormulas() {#getshowformulas}

Indicates whether to show formulas or their results.

### getSlicers() {#getslicers}

Get the Slicer collection in the worksheet

### getSmartTagSetting() {#getsmarttagsetting}

Gets all SmartTagCollection objects of the worksheet.

### getSparklineGroups() {#getsparklinegroups}

Gets the sparkline groups in the worksheet.

### getTabColor() {#gettabcolor}

Represents worksheet tab color. This feature is only supported in ExcelXP(Excel2002) and later versions. If you save file as Excel97 or Excel2000 format, it will be omitted.

### getTabId() {#gettabid}

Specifies the internal identifier for the sheet.

### getTextBoxes() {#gettextboxes}

Gets a TextBox collection.

### getTimelines() {#gettimelines}

Get the Timeline collection in the worksheet

### getTransitionEntry() {#gettransitionentry}

Indicates whether the Transition Formula Entry (Lotus compatibility) option is enabled.

### getTransitionEvaluation() {#gettransitionevaluation}

Indicates whether the Transition Formula Evaluation (Lotus compatibility) option is enabled.

### getType() {#gettype}

Represents worksheet type. The value of the property is SheetType integer constant.

### getUniqueId() {#getuniqueid}

Gets and sets the unique id, it is same as {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}.

### getValidations() {#getvalidations}

Gets the data validation setting collection in the worksheet.

### getVerticalPageBreaks() {#getverticalpagebreaks}

Gets the VerticalPageBreakCollection collection.

### getViewType() {#getviewtype}

Gets and sets the view type. The value of the property is ViewType integer constant.

### getVisibilityType() {#getvisibilitytype}

Indicates the visible state for this sheet. The value of the property is VisibilityType integer constant.

### getWorkbook() {#getworkbook}

Gets the workbook object which contains this sheet.

### getZoom() {#getzoom}

Represents the scaling factor in percentage. It should be between 10 and 400. Please set the view type first.

### hasAutofilter() {#hasautofilter}

Indicates whether this worksheet has auto filter.

### isGridlinesVisible() {#isgridlinesvisible}

Gets or sets a value indicating whether the gridlines are visible.Default is true.

### isOutlineShown() {#isoutlineshown}

Indicates whether to show outline.

### isPageBreakPreview() {#ispagebreakpreview}

Indicates whether the specified worksheet is shown in normal view or page break preview.

### isProtected() {#isprotected}

Indicates if the worksheet is protected.

### isRowColumnHeadersVisible() {#isrowcolumnheadersvisible}

Gets or sets a value indicating whether the worksheet will display row and column headers. Default is true.

### isRulerVisible() {#isrulervisible}

Indicates whether the ruler is visible. This property is only applied for page break preview.

### isSelected() {#isselected}

Indicates whether this worksheet is selected when the workbook is opened.

### isVisible() {#isvisible}

Represents if the worksheet is visible.

### moveTo(index) {#moveto}

Moves the sheet to another location in the spreadsheet.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | Destination sheet index. |

### protect(type) {#protect}

Protects worksheet. This method protects worksheet without password. It can protect worksheet in all versions of Excel file.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | ProtectionType |

### protect(type, password, oldPassword) {#protect-1}

Protects worksheet. This method can protect worksheet in all versions of Excel file.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | ProtectionType |
| password | String | Password. |
| oldPassword | String | If the worksheet is already protected by a password, please supply the old password. Otherwise, you can set a null value or blank string to this parameter. |

**Example:**

```js
//Instantiating a Workbook object
var excel = new aspose.cells.Workbook("Book2.xls");
//Accessing the first worksheet in the Excel file
var worksheet = excel.getWorksheets().get(0);
//Protecting the worksheet with a password
worksheet.protect(aspose.cells.ProtectionType.ALL, "aspose", null);
//Saving the modified Excel file in default (that is Excel 20003) format
excel.save("Book1.xls");
```

### refreshPivotTables() {#refreshpivottables}

Refreshes all the PivotTables in this Worksheet.

### refreshPivotTables(option) {#refreshpivottables-1}

Refreshes all the PivotTables in this Worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| option | PivotTableRefreshOption | The option for refreshing data source of pivot table. |

### removeAllDrawingObjects() {#removealldrawingobjects}

Removes all drawing objects in this worksheet.

### removeAutoFilter() {#removeautofilter}

Removes the auto filter of the worksheet.

### removeSplit() {#removesplit}

Removes split window.

### replace(oldString, newString) {#replace}

Replaces all cells' text with a new string.

| Parameter | Type | Description |
| --- | --- | --- |
| oldString | String | Old string value. |
| newString | String | New string value. |

### selectRange(startRow, startColumn, totalRows, totalColumns, removeOthers) {#selectrange}

Selects a range.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Number | The start row. |
| startColumn | Number | The start column |
| totalRows | Number | The number of rows. |
| totalColumns | Number | The number of columns |
| removeOthers | boolean | True means removing other selected range and only select this range. |

### setActiveCell() {#setactivecell}

Gets or sets the active cell in the worksheet.

### setBackgroundImage() {#setbackgroundimage}

Gets and sets worksheet background image.

### setCodeName() {#setcodename}

Gets worksheet code name.

### setDisplayRightToLeft() {#setdisplayrighttoleft}

Indicates if the specified worksheet is displayed from right to left instead of from left to right. Default is false.

### setDisplayZeros() {#setdisplayzeros}

True if zero values are displayed.

### setFirstVisibleColumn() {#setfirstvisiblecolumn}

Represents first visible column index.

### setFirstVisibleRow() {#setfirstvisiblerow}

Represents first visible row index.

### setGridlineColor() {#setgridlinecolor}

### setGridlinesVisible() {#setgridlinesvisible}

Gets or sets a value indicating whether the gridlines are visible.Default is true.

### setName() {#setname}

Gets or sets the name of the worksheet. The max length of sheet name is 31. And you cannot assign same name(case insensitive) to two worksheets. For example, you cannot set "SheetName1" to the first worksheet and set "SHEETNAME1" to the second worksheet.

### setOutlineShown() {#setoutlineshown}

Indicates whether to show outline.

### setPageBreakPreview() {#setpagebreakpreview}

Indicates whether the specified worksheet is shown in normal view or page break preview.

### setRowColumnHeadersVisible() {#setrowcolumnheadersvisible}

Gets or sets a value indicating whether the worksheet will display row and column headers. Default is true.

### setRulerVisible() {#setrulervisible}

Indicates whether the ruler is visible. This property is only applied for page break preview.

### setSelected() {#setselected}

Indicates whether this worksheet is selected when the workbook is opened.

### setShowDataTypeIcons() {#setshowdatatypeicons}

### setShowFormulas() {#setshowformulas}

Indicates whether to show formulas or their results.

### setTabColor() {#settabcolor}

Represents worksheet tab color. This feature is only supported in ExcelXP(Excel2002) and later versions. If you save file as Excel97 or Excel2000 format, it will be omitted.

### setTabId() {#settabid}

Specifies the internal identifier for the sheet.

### setTransitionEntry() {#settransitionentry}

Indicates whether the Transition Formula Entry (Lotus compatibility) option is enabled.

### setTransitionEvaluation() {#settransitionevaluation}

Indicates whether the Transition Formula Evaluation (Lotus compatibility) option is enabled.

### setType() {#settype}

Represents worksheet type. The value of the property is SheetType integer constant.

### setUniqueId() {#setuniqueid}

Gets and sets the unique id, it is same as {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}.

### setViewType() {#setviewtype}

Gets and sets the view type. The value of the property is ViewType integer constant.

### setVisibilityType() {#setvisibilitytype}

Indicates the visible state for this sheet. The value of the property is VisibilityType integer constant.

### setVisible() {#setvisible}

Represents if the worksheet is visible.

### setVisible(isVisible, ignoreError) {#setvisible-1}

Sets the visible options.

| Parameter | Type | Description |
| --- | --- | --- |
| isVisible | boolean | Whether the worksheet is visible |
| ignoreError | boolean | Whether to ignore error if this option is not valid. |

### setZoom() {#setzoom}

Represents the scaling factor in percentage. It should be between 10 and 400. Please set the view type first.

### split() {#split}

Splits window.

### startAccessCache(opts) {#startaccesscache}

Starts the session that uses caches to access the data in this worksheet. After finishing the access to the data, closeAccessCache(int) should be invoked with same options to clear all caches and recover normal access mode.

| Parameter | Type | Description |
| --- | --- | --- |
| opts | Number | AccessCacheOptions |

### toString() {#tostring}

Returns a string represents the current Worksheet object.

**Returns:** String — `String`

### unFreezePanes() {#unfreezepanes}

Unfreezes panes in the worksheet.

### unprotect() {#unprotect}

Unprotects worksheet. This method unprotects worksheet which is protected without password.

### unprotect(password) {#unprotect-1}

Unprotects worksheet. If the worksheet is protected without a password, you can set a null value or blank string to password parameter.

| Parameter | Type | Description |
| --- | --- | --- |
| password | String | Password |

### xmlMapQuery(path, xmlMap) {#xmlmapquery}

Query cell areas that mapped/linked to the specific path of xml map. e.g. A xml map element structure: -RootElement |-Attribute1 |-SubElement |-Attribute2 |-Attribute3 To query "Attribute1", path is "/RootElement/@Attribute1" To query "Attribute2", path is "/RootElement/SubElement/@Attribute2" To query whole "SubElement", path is "/RootElement/SubElement"

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | xml element path |
| xmlMap | XmlMap | Specify an xml map if you want to query for the specific path within a specific map |

**Returns:** ArrayList — `ArrayList` CellArea list that mapped/linked to the specific path of xml map, an empty list is returned if nothing is mapped/linked.
