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
| [addPageBreaks(cellName)](./addpagebreaks/) | Adds page break. |
| [advancedFilter(isFilter, listRange, criteriaRange, copyTo, uniqueRecordOnly)](./advancedfilter/) | Filters data using complex criteria. |
| [autoFitColumn(columnIndex, firstRow, lastRow)](./autofitcolumn/) | Autofits the column width. This method autofits a row based on content in a range of cells within the row. |
| [autoFitColumn(columnIndex)](./autofitcolumn-1/) | Autofits the column width. AutoFitColumn is an imprecise function. |
| [autoFitColumns()](./autofitcolumns/) | Autofits all columns in this worksheet. |
| [autoFitColumns(options)](./autofitcolumns-1/) | Autofits all columns in this worksheet. |
| [autoFitColumns(firstColumn, lastColumn)](./autofitcolumns-2/) | Autofits the columns width. AutoFitColumn is an imprecise function. |
| [autoFitColumns(firstColumn, lastColumn, options)](./autofitcolumns-3/) | Autofits the columns width. AutoFitColumn is an imprecise function. |
| [autoFitColumns(firstRow, firstColumn, lastRow, lastColumn)](./autofitcolumns-4/) | Autofits the columns width. AutoFitColumn is an imprecise function. |
| [autoFitColumns(firstRow, firstColumn, lastRow, lastColumn, options)](./autofitcolumns-5/) | Autofits the columns width. AutoFitColumn is an imprecise function. |
| [autoFitRow(rowIndex, firstColumn, lastColumn)](./autofitrow/) | Autofits the row height. This method autofits a row based on content in a range of cells within the row. |
| [autoFitRow(rowIndex, firstColumn, lastColumn, options)](./autofitrow-1/) | Autofits the row height. This method autofits a row based on content in a range of cells within the row. |
| [autoFitRow(startRow, endRow, startColumn, endColumn)](./autofitrow-2/) | Autofits row height in a rectangle range. |
| [autoFitRow(rowIndex)](./autofitrow-3/) | Autofits the row height. AutoFitRow is an imprecise function. |
| [autoFitRows()](./autofitrows/) | Autofits all rows in this worksheet. |
| [autoFitRows(onlyAuto)](./autofitrows-1/) | Autofits all rows in this worksheet. |
| [autoFitRows(options)](./autofitrows-2/) | Autofits all rows in this worksheet. |
| [autoFitRows(startRow, endRow)](./autofitrows-3/) | Autofits row height in a range. |
| [autoFitRows(startRow, endRow, options)](./autofitrows-4/) | Autofits row height in a range. |
| [calculateArrayFormula(formula, opts)](./calculatearrayformula/) | Calculates a formula as array formula. |
| [calculateArrayFormula(formula, opts, maxRowCount, maxColumnCount)](./calculatearrayformula-1/) | Calculates a formula as array formula. The formula will be taken as dynamic array formula to calculate the dimension and |
| [calculateArrayFormula(formula, pOpts, cOpts, baseCellRow, baseCellColumn, maxRowCount, maxColumnCount, calculationData)](./calculatearrayformula-2/) | Calculates a formula as array formula. The formula will be taken as dynamic array formula to calculate the dimension and |
| [calculateFormula(formula)](./calculateformula/) | Calculates a formula. |
| [calculateFormula(formula, opts)](./calculateformula-1/) | Calculates a formula expression directly. The formula will be calculated just like it has been set to cell A1. And the f |
| [calculateFormula(formula, pOpts, cOpts, baseCellRow, baseCellColumn, calculationData)](./calculateformula-2/) | Calculates a formula expression directly. The formula will be calculated just like it has been set to the specified base |
| [calculateFormula(options, recursive)](./calculateformula-3/) | Calculates all formulas in this worksheet. |
| [clearComments()](./clearcomments/) | Clears all comments in designer spreadsheet. |
| [closeAccessCache(opts)](./closeaccesscache/) | Closes the session that uses caches to access the data in this worksheet. |
| [convertFormulaReferenceStyle(formula, toR1C1, baseCellRow, baseCellColumn)](./convertformulareferencestyle/) | Converts the formula reference style. |
| [copy(sourceSheet)](./copy/) | Copies contents and formats from another worksheet. |
| [copy(sourceSheet, copyOptions)](./copy-1/) | Copies contents and formats from another worksheet. You can copy data from another worksheet in the same file or another |
| [dispose()](./dispose/) | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [filter()](./filter/) |  |
| [freezePanes(row, column, freezedRows, freezedColumns)](./freezepanes/) | Freezes panes at the specified cell in the worksheet. Row index and column index cannot all be zero. Number of rows and  |
| [freezePanes(cellName, freezedRows, freezedColumns)](./freezepanes-1/) | Freezes panes at the specified cell in the worksheet. Row index and column index cannot all be zero. Number of rows and  |
| [getActiveCell()](./getactivecell/) | Gets or sets the active cell in the worksheet. |
| [getAdvancedFilter()](./getadvancedfilter/) | Gets the settings of advanced filter. |
| [getAllPictures()](./getallpictures/) |  |
| [getAllowEditRanges()](./getalloweditranges/) | Gets the allow edit range collection in the worksheet. |
| [getAutoFilter()](./getautofilter/) | Represents auto filter for the specified worksheet. |
| [getBackgroundImage()](./getbackgroundimage/) | Gets and sets worksheet background image. |
| [getCellWatches()](./getcellwatches/) | Gets collection of cells on this worksheet being watched in the 'watch window'. |
| [getCells()](./getcells/) | Gets the Cells collection. |
| [getCharts()](./getcharts/) | Gets a Chart collection |
| [getCheckBoxes()](./getcheckboxes/) | Gets a CheckBox collection. |
| [getCodeName()](./getcodename/) | Gets worksheet code name. |
| [getComments()](./getcomments/) | Gets the Comment collection. |
| [getConditionalFormattings()](./getconditionalformattings/) | Gets the ConditionalFormattings in the worksheet. |
| [getCustomProperties()](./getcustomproperties/) | Gets an object representing the identifier information associated with a worksheet. Worksheet.CustomProperties provide a |
| [getDisplayRightToLeft()](./getdisplayrighttoleft/) | Indicates if the specified worksheet is displayed from right to left instead of from left to right. Default is false. |
| [getDisplayZeros()](./getdisplayzeros/) | True if zero values are displayed. |
| [getErrorCheckOptions()](./geterrorcheckoptions/) | Gets error check setting applied on certain ranges. |
| [getFirstVisibleColumn()](./getfirstvisiblecolumn/) | Represents first visible column index. |
| [getFirstVisibleRow()](./getfirstvisiblerow/) | Represents first visible row index. |
| [getFreezedPanes()](./getfreezedpanes/) | Gets the freeze panes. |
| [getGridlineColor()](./getgridlinecolor/) |  |
| [getHorizontalPageBreaks()](./gethorizontalpagebreaks/) | Gets the HorizontalPageBreakCollection collection. |
| [getHyperlinks()](./gethyperlinks/) | Gets the HyperlinkCollection collection. |
| [getIndex()](./getindex/) | Gets the index of sheet in the worksheet collection. |
| [getListObjects()](./getlistobjects/) | Gets all ListObjects in this worksheet. |
| [getName()](./getname/) | Gets or sets the name of the worksheet. The max length of sheet name is 31. And you cannot assign same name(case insensi |
| [getOleObjects()](./getoleobjects/) | Represents a collection of OleObject in a worksheet. |
| [getOutline()](./getoutline/) | Gets the outline on this worksheet. |
| [getPageSetup()](./getpagesetup/) | Represents the page setup description in this sheet. |
| [getPaneState()](./getpanestate/) | Indicates whether the pane has horizontal or vertical splits, and whether those splits are frozen. The value of the prop |
| [getPanes()](./getpanes/) | Gets the window panes. If the window is not split or frozen. |
| [getPictures()](./getpictures/) | Gets a Picture collection. |
| [getPivotTables()](./getpivottables/) | Gets all pivot tables in this worksheet. |
| [getPrintingPageBreaks(options)](./getprintingpagebreaks/) | Gets automatic page breaks. Each cell area represents a paper. |
| [getProtection()](./getprotection/) | Represents the various types of protection options available for a worksheet. Supports advanced protection options in Ex |
| [getQueryTables()](./getquerytables/) | Gets QueryTableCollection in the worksheet. |
| [getScenarios()](./getscenarios/) | Gets the collection of Scenario. |
| [getSelectedAreas()](./getselectedareas/) |  |
| [getSelectedRanges()](./getselectedranges/) | Gets selected ranges of cells in the designer spreadsheet. |
| [getShapes()](./getshapes/) | Returns all drawing shapes in this worksheet. |
| [getShowDataTypeIcons()](./getshowdatatypeicons/) |  |
| [getShowFormulas()](./getshowformulas/) | Indicates whether to show formulas or their results. |
| [getSlicers()](./getslicers/) | Get the Slicer collection in the worksheet |
| [getSmartTagSetting()](./getsmarttagsetting/) | Gets all SmartTagCollection objects of the worksheet. |
| [getSparklineGroups()](./getsparklinegroups/) | Gets the sparkline groups in the worksheet. |
| [getTabColor()](./gettabcolor/) | Represents worksheet tab color. This feature is only supported in ExcelXP(Excel2002) and later versions. If you save fil |
| [getTabId()](./gettabid/) | Specifies the internal identifier for the sheet. |
| [getTextBoxes()](./gettextboxes/) | Gets a TextBox collection. |
| [getTimelines()](./gettimelines/) | Get the Timeline collection in the worksheet |
| [getTransitionEntry()](./gettransitionentry/) | Indicates whether the Transition Formula Entry (Lotus compatibility) option is enabled. |
| [getTransitionEvaluation()](./gettransitionevaluation/) | Indicates whether the Transition Formula Evaluation (Lotus compatibility) option is enabled. |
| [getType()](./gettype/) | Represents worksheet type. The value of the property is SheetType integer constant. |
| [getUniqueId()](./getuniqueid/) | Gets and sets the unique id, it is same as {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. |
| [getValidations()](./getvalidations/) | Gets the data validation setting collection in the worksheet. |
| [getVerticalPageBreaks()](./getverticalpagebreaks/) | Gets the VerticalPageBreakCollection collection. |
| [getViewType()](./getviewtype/) | Gets and sets the view type. The value of the property is ViewType integer constant. |
| [getVisibilityType()](./getvisibilitytype/) | Indicates the visible state for this sheet. The value of the property is VisibilityType integer constant. |
| [getWorkbook()](./getworkbook/) | Gets the workbook object which contains this sheet. |
| [getZoom()](./getzoom/) | Represents the scaling factor in percentage. It should be between 10 and 400. Please set the view type first. |
| [hasAutofilter()](./hasautofilter/) | Indicates whether this worksheet has auto filter. |
| [isGridlinesVisible()](./isgridlinesvisible/) | Gets or sets a value indicating whether the gridlines are visible.Default is true. |
| [isOutlineShown()](./isoutlineshown/) | Indicates whether to show outline. |
| [isPageBreakPreview()](./ispagebreakpreview/) | Indicates whether the specified worksheet is shown in normal view or page break preview. |
| [isProtected()](./isprotected/) | Indicates if the worksheet is protected. |
| [isRowColumnHeadersVisible()](./isrowcolumnheadersvisible/) | Gets or sets a value indicating whether the worksheet will display row and column headers. Default is true. |
| [isRulerVisible()](./isrulervisible/) | Indicates whether the ruler is visible. This property is only applied for page break preview. |
| [isSelected()](./isselected/) | Indicates whether this worksheet is selected when the workbook is opened. |
| [isVisible()](./isvisible/) | Represents if the worksheet is visible. |
| [moveTo(index)](./moveto/) | Moves the sheet to another location in the spreadsheet. |
| [protect(type)](./protect/) | Protects worksheet. This method protects worksheet without password. It can protect worksheet in all versions of Excel f |
| [protect(type, password, oldPassword)](./protect-1/) | Protects worksheet. This method can protect worksheet in all versions of Excel file. |
| [refreshPivotTables()](./refreshpivottables/) | Refreshes all the PivotTables in this Worksheet. |
| [refreshPivotTables(option)](./refreshpivottables-1/) | Refreshes all the PivotTables in this Worksheet. |
| [removeAllDrawingObjects()](./removealldrawingobjects/) | Removes all drawing objects in this worksheet. |
| [removeAutoFilter()](./removeautofilter/) | Removes the auto filter of the worksheet. |
| [removeSplit()](./removesplit/) | Removes split window. |
| [replace(oldString, newString)](./replace/) | Replaces all cells' text with a new string. |
| [selectRange(startRow, startColumn, totalRows, totalColumns, removeOthers)](./selectrange/) | Selects a range. |
| [setActiveCell()](./setactivecell/) | Gets or sets the active cell in the worksheet. |
| [setBackgroundImage()](./setbackgroundimage/) | Gets and sets worksheet background image. |
| [setCodeName()](./setcodename/) | Gets worksheet code name. |
| [setDisplayRightToLeft()](./setdisplayrighttoleft/) | Indicates if the specified worksheet is displayed from right to left instead of from left to right. Default is false. |
| [setDisplayZeros()](./setdisplayzeros/) | True if zero values are displayed. |
| [setFirstVisibleColumn()](./setfirstvisiblecolumn/) | Represents first visible column index. |
| [setFirstVisibleRow()](./setfirstvisiblerow/) | Represents first visible row index. |
| [setGridlineColor()](./setgridlinecolor/) |  |
| [setGridlinesVisible()](./setgridlinesvisible/) | Gets or sets a value indicating whether the gridlines are visible.Default is true. |
| [setName()](./setname/) | Gets or sets the name of the worksheet. The max length of sheet name is 31. And you cannot assign same name(case insensi |
| [setOutlineShown()](./setoutlineshown/) | Indicates whether to show outline. |
| [setPageBreakPreview()](./setpagebreakpreview/) | Indicates whether the specified worksheet is shown in normal view or page break preview. |
| [setRowColumnHeadersVisible()](./setrowcolumnheadersvisible/) | Gets or sets a value indicating whether the worksheet will display row and column headers. Default is true. |
| [setRulerVisible()](./setrulervisible/) | Indicates whether the ruler is visible. This property is only applied for page break preview. |
| [setSelected()](./setselected/) | Indicates whether this worksheet is selected when the workbook is opened. |
| [setShowDataTypeIcons()](./setshowdatatypeicons/) |  |
| [setShowFormulas()](./setshowformulas/) | Indicates whether to show formulas or their results. |
| [setTabColor()](./settabcolor/) | Represents worksheet tab color. This feature is only supported in ExcelXP(Excel2002) and later versions. If you save fil |
| [setTabId()](./settabid/) | Specifies the internal identifier for the sheet. |
| [setTransitionEntry()](./settransitionentry/) | Indicates whether the Transition Formula Entry (Lotus compatibility) option is enabled. |
| [setTransitionEvaluation()](./settransitionevaluation/) | Indicates whether the Transition Formula Evaluation (Lotus compatibility) option is enabled. |
| [setType()](./settype/) | Represents worksheet type. The value of the property is SheetType integer constant. |
| [setUniqueId()](./setuniqueid/) | Gets and sets the unique id, it is same as {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. |
| [setViewType()](./setviewtype/) | Gets and sets the view type. The value of the property is ViewType integer constant. |
| [setVisibilityType()](./setvisibilitytype/) | Indicates the visible state for this sheet. The value of the property is VisibilityType integer constant. |
| [setVisible()](./setvisible/) | Represents if the worksheet is visible. |
| [setVisible(isVisible, ignoreError)](./setvisible-1/) | Sets the visible options. |
| [setZoom()](./setzoom/) | Represents the scaling factor in percentage. It should be between 10 and 400. Please set the view type first. |
| [split()](./split/) | Splits window. |
| [startAccessCache(opts)](./startaccesscache/) | Starts the session that uses caches to access the data in this worksheet. After finishing the access to the data, closeA |
| [toString()](./tostring/) | Returns a string represents the current Worksheet object. |
| [unFreezePanes()](./unfreezepanes/) | Unfreezes panes in the worksheet. |
| [unprotect()](./unprotect/) | Unprotects worksheet. This method unprotects worksheet which is protected without password. |
| [unprotect(password)](./unprotect-1/) | Unprotects worksheet. If the worksheet is protected without a password, you can set a null value or blank string to pass |
| [xmlMapQuery(path, xmlMap)](./xmlmapquery/) | Query cell areas that mapped/linked to the specific path of xml map. e.g. A xml map element structure: -RootElement \|-At |
