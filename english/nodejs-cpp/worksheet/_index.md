---
title: Worksheet
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates the object that represents a single worksheet.
type: docs
url: /nodejs-cpp/worksheet/
---

## Worksheet class

Encapsulates the object that represents a single worksheet.

```javascript
class Worksheet;
```


## Methods

| Method | Description |
| --- | --- |
| [getProtection()](#getProtection--)| Represents the various types of protection options available for a worksheet. Supports advanced protection options in ExcelXP and above version. |
| [getUniqueId()](#getUniqueId--)| Gets and sets the unique id, it is same as {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. |
| [setUniqueId(string)](#setUniqueId-string-)| Gets and sets the unique id, it is same as {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. |
| [getWorkbook()](#getWorkbook--)| Gets the workbook object which contains this sheet. |
| [getCells()](#getCells--)| Gets the [Cells](./cells/) collection. |
| [getQueryTables()](#getQueryTables--)| Gets [QueryTableCollection](./querytablecollection/) in the worksheet. |
| [getPivotTables()](#getPivotTables--)| Gets all pivot tables in this worksheet. |
| [getType()](#getType--)| Represents worksheet type. |
| [setType(SheetType)](#setType-sheettype-)| Represents worksheet type. |
| [getName()](#getName--)| Gets or sets the name of the worksheet. |
| [setName(string)](#setName-string-)| Gets or sets the name of the worksheet. |
| [getShowFormulas()](#getShowFormulas--)| Indicates whether to show formulas or their results. |
| [setShowFormulas(boolean)](#setShowFormulas-boolean-)| Indicates whether to show formulas or their results. |
| [isGridlinesVisible()](#isGridlinesVisible--)| Gets or sets a value indicating whether the gridlines are visible.Default is true. |
| [setIsGridlinesVisible(boolean)](#setIsGridlinesVisible-boolean-)| Gets or sets a value indicating whether the gridlines are visible.Default is true. |
| [isRowColumnHeadersVisible()](#isRowColumnHeadersVisible--)| Gets or sets a value indicating whether the worksheet will display row and column headers. Default is true. |
| [setIsRowColumnHeadersVisible(boolean)](#setIsRowColumnHeadersVisible-boolean-)| Gets or sets a value indicating whether the worksheet will display row and column headers. Default is true. |
| [getPaneState()](#getPaneState--)| Indicates whether the pane has horizontal or vertical splits, and whether those splits are frozen. |
| [getDisplayZeros()](#getDisplayZeros--)| True if zero values are displayed. |
| [setDisplayZeros(boolean)](#setDisplayZeros-boolean-)| True if zero values are displayed. |
| [getDisplayRightToLeft()](#getDisplayRightToLeft--)| Indicates if the specified worksheet is displayed from right to left instead of from left to right. Default is false. |
| [setDisplayRightToLeft(boolean)](#setDisplayRightToLeft-boolean-)| Indicates if the specified worksheet is displayed from right to left instead of from left to right. Default is false. |
| [isOutlineShown()](#isOutlineShown--)| Indicates whether to show outline. |
| [setIsOutlineShown(boolean)](#setIsOutlineShown-boolean-)| Indicates whether to show outline. |
| [isSelected()](#isSelected--)| Indicates whether this worksheet is selected when the workbook is opened. |
| [setIsSelected(boolean)](#setIsSelected-boolean-)| Indicates whether this worksheet is selected when the workbook is opened. |
| [getListObjects()](#getListObjects--)| Gets all ListObjects in this worksheet. |
| [getTabId()](#getTabId--)| Specifies the internal identifier for the sheet. |
| [setTabId(number)](#setTabId-number-)| Specifies the internal identifier for the sheet. |
| [getHorizontalPageBreaks()](#getHorizontalPageBreaks--)| Gets the [HorizontalPageBreakCollection](./horizontalpagebreakcollection/) collection. |
| [getVerticalPageBreaks()](#getVerticalPageBreaks--)| Gets the [VerticalPageBreakCollection](./verticalpagebreakcollection/) collection. |
| [getHyperlinks()](#getHyperlinks--)| Gets the [HyperlinkCollection](./hyperlinkcollection/) collection. |
| [getPageSetup()](#getPageSetup--)| Represents the page setup description in this sheet. |
| [getAutoFilter()](#getAutoFilter--)| Represents auto filter for the specified worksheet. |
| [getHasAutofilter()](#getHasAutofilter--)| Indicates whether this worksheet has auto filter. |
| [getTransitionEvaluation()](#getTransitionEvaluation--)| Indicates whether the Transition Formula Evaluation (Lotus compatibility) option is enabled. |
| [setTransitionEvaluation(boolean)](#setTransitionEvaluation-boolean-)| Indicates whether the Transition Formula Evaluation (Lotus compatibility) option is enabled. |
| [getTransitionEntry()](#getTransitionEntry--)| Indicates whether the Transition Formula Entry (Lotus compatibility) option is enabled. |
| [setTransitionEntry(boolean)](#setTransitionEntry-boolean-)| Indicates whether the Transition Formula Entry (Lotus compatibility) option is enabled. |
| [getVisibilityType()](#getVisibilityType--)| Indicates the visible state for this sheet. |
| [setVisibilityType(VisibilityType)](#setVisibilityType-visibilitytype-)| Indicates the visible state for this sheet. |
| [isVisible()](#isVisible--)| Represents if the worksheet is visible. |
| [setIsVisible(boolean)](#setIsVisible-boolean-)| Represents if the worksheet is visible. |
| [getSparklineGroups()](#getSparklineGroups--)| Gets the sparkline groups in the worksheet. |
| [getCharts()](#getCharts--)| Gets a [Chart](./chart/) collection |
| [getComments()](#getComments--)| Gets the [Comment](./comment/) collection. |
| [getPictures()](#getPictures--)| Gets a [Picture](./picture/) collection. |
| [getTextBoxes()](#getTextBoxes--)| Gets a [TextBox](./textbox/) collection. |
| [getCheckBoxes()](#getCheckBoxes--)| Gets a [CheckBox](./checkbox/) collection. |
| [getOleObjects()](#getOleObjects--)| Represents a collection of [OleObject](./oleobject/) in a worksheet. |
| [getShapes()](#getShapes--)| Returns all drawing shapes in this worksheet. |
| [getSlicers()](#getSlicers--)| Get the Slicer collection in the worksheet |
| [getTimelines()](#getTimelines--)| Get the Timeline collection in the worksheet |
| [getIndex()](#getIndex--)| Gets the index of sheet in the worksheet collection. |
| [isProtected()](#isProtected--)| Indicates if the worksheet is protected. |
| [getValidations()](#getValidations--)| Gets the data validation setting collection in the worksheet. |
| [getAllowEditRanges()](#getAllowEditRanges--)| Gets the allow edit range collection in the worksheet. |
| [getErrorCheckOptions()](#getErrorCheckOptions--)| Gets error check setting applied on certain ranges. |
| [getOutline()](#getOutline--)| Gets the outline on this worksheet. |
| [getFirstVisibleRow()](#getFirstVisibleRow--)| Represents first visible row index. |
| [setFirstVisibleRow(number)](#setFirstVisibleRow-number-)| Represents first visible row index. |
| [getFirstVisibleColumn()](#getFirstVisibleColumn--)| Represents first visible column index. |
| [setFirstVisibleColumn(number)](#setFirstVisibleColumn-number-)| Represents first visible column index. |
| [getZoom()](#getZoom--)| Represents the scaling factor in percentage. It should be between 10 and 400. |
| [setZoom(number)](#setZoom-number-)| Represents the scaling factor in percentage. It should be between 10 and 400. |
| [getViewType()](#getViewType--)| Gets and sets the view type. |
| [setViewType(ViewType)](#setViewType-viewtype-)| Gets and sets the view type. |
| [isPageBreakPreview()](#isPageBreakPreview--)| Indicates whether the specified worksheet is shown in normal view or page break preview. |
| [setIsPageBreakPreview(boolean)](#setIsPageBreakPreview-boolean-)| Indicates whether the specified worksheet is shown in normal view or page break preview. |
| [isRulerVisible()](#isRulerVisible--)| Indicates whether the ruler is visible. This property is only applied for page break preview. |
| [setIsRulerVisible(boolean)](#setIsRulerVisible-boolean-)| Indicates whether the ruler is visible. This property is only applied for page break preview. |
| [getTabColor()](#getTabColor--)| Represents worksheet tab color. |
| [setTabColor(Color)](#setTabColor-color-)| Represents worksheet tab color. |
| [getCodeName()](#getCodeName--)| Gets worksheet code name. |
| [setCodeName(string)](#setCodeName-string-)| Gets worksheet code name. |
| [getBackgroundImage()](#getBackgroundImage--)| Gets and sets worksheet background image. |
| [setBackgroundImage(number[])](#setBackgroundImage-number[]-)| Gets and sets worksheet background image. |
| [getConditionalFormattings()](#getConditionalFormattings--)| Gets the ConditionalFormattings in the worksheet. |
| [getActiveCell()](#getActiveCell--)| Gets or sets the active cell in the worksheet. |
| [setActiveCell(string)](#setActiveCell-string-)| Gets or sets the active cell in the worksheet. |
| [getCustomProperties()](#getCustomProperties--)| Gets an object representing the identifier information associated with a worksheet. |
| [getSmartTagSetting()](#getSmartTagSetting--)| Gets all [SmartTagCollection](./smarttagcollection/) objects of the worksheet. |
| [getScenarios()](#getScenarios--)| Gets the collection of [Scenario](./scenario/). |
| [getCellWatches()](#getCellWatches--)| Gets collection of cells on this worksheet being watched in the 'watch window'. |
| [dispose()](#dispose--)| Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [getPanes()](#getPanes--)| Gets the window panes. |
| [freezePanes(number, number, number, number)](#freezePanes-number-number-number-number-)| Freezes panes at the specified cell in the worksheet. |
| [freezePanes(string, number, number)](#freezePanes-string-number-number-)| Freezes panes at the specified cell in the worksheet. |
| [getFreezedPanes(number, number, number, number)](#getFreezedPanes-number-number-number-number-)| Gets the freeze panes. |
| [split()](#split--)| Splits window. |
| [unFreezePanes()](#unFreezePanes--)| Unfreezes panes in the worksheet. |
| [removeSplit()](#removeSplit--)| Removes split window. |
| [addPageBreaks(string)](#addPageBreaks-string-)| Adds page break. |
| [copy(Worksheet)](#copy-worksheet-)| Copies contents and formats from another worksheet. |
| [copy(Worksheet, CopyOptions)](#copy-worksheet-copyoptions-)| Copies contents and formats from another worksheet. |
| [autoFitColumn(number, number, number)](#autoFitColumn-number-number-number-)| Autofits the column width. |
| [autoFitColumn(number)](#autoFitColumn-number-)| Autofits the column width. |
| [autoFitColumns()](#autoFitColumns--)| Autofits all columns in this worksheet. |
| [autoFitColumns(AutoFitterOptions)](#autoFitColumns-autofitteroptions-)| Autofits all columns in this worksheet. |
| [autoFitColumns(number, number)](#autoFitColumns-number-number-)| Autofits the columns width. |
| [autoFitColumns(number, number, AutoFitterOptions)](#autoFitColumns-number-number-autofitteroptions-)| Autofits the columns width. |
| [autoFitColumns(number, number, number, number)](#autoFitColumns-number-number-number-number-)| Autofits the columns width. |
| [autoFitColumns(number, number, number, number, AutoFitterOptions)](#autoFitColumns-number-number-number-number-autofitteroptions-)| Autofits the columns width. |
| [autoFitRow(number, number, number)](#autoFitRow-number-number-number-)| Autofits the row height. |
| [autoFitRow(number, number, number, AutoFitterOptions)](#autoFitRow-number-number-number-autofitteroptions-)| Autofits the row height. |
| [autoFitRow(number, number, number, number)](#autoFitRow-number-number-number-number-)| Autofits row height in a rectangle range. |
| [autoFitRow(number)](#autoFitRow-number-)| Autofits the row height. |
| [autoFitRows()](#autoFitRows--)| Autofits all rows in this worksheet. |
| [autoFitRows(boolean)](#autoFitRows-boolean-)| Autofits all rows in this worksheet. |
| [autoFitRows(AutoFitterOptions)](#autoFitRows-autofitteroptions-)| Autofits all rows in this worksheet. |
| [autoFitRows(number, number)](#autoFitRows-number-number-)| Autofits row height in a range. |
| [autoFitRows(number, number, AutoFitterOptions)](#autoFitRows-number-number-autofitteroptions-)| Autofits row height in a range. |
| [getAdvancedFilter()](#getAdvancedFilter--)| Gets the settings of advanced filter. |
| [advanced_Filter(boolean, string, string, string, boolean)](#advanced_Filter-boolean-string-string-string-boolean-)| Filters data using complex criteria. |
| [removeAutoFilter()](#removeAutoFilter--)| Removes the auto filter of the worksheet. |
| [setVisible(boolean, boolean)](#setVisible-boolean-boolean-)| Sets the visible options. |
| [selectRange(number, number, number, number, boolean)](#selectRange-number-number-number-number-boolean-)| Selects a range. |
| [removeAllDrawingObjects()](#removeAllDrawingObjects--)| Removes all drawing objects in this worksheet. |
| [clearComments()](#clearComments--)| Clears all comments in designer spreadsheet. |
| [protect(ProtectionType)](#protect-protectiontype-)| Protects worksheet. |
| [protect(ProtectionType, string, string)](#protect-protectiontype-string-string-)| Protects worksheet. |
| [unprotect()](#unprotect--)| Unprotects worksheet. |
| [unprotect(string)](#unprotect-string-)| Unprotects worksheet. |
| [moveTo(number)](#moveTo-number-)| Moves the sheet to another location in the spreadsheet. |
| [replace(string, string)](#replace-string-string-)| Replaces all cells' text with a new string. |
| [getPrintingPageBreaks(ImageOrPrintOptions)](#getPrintingPageBreaks-imageorprintoptions-)| Gets automatic page breaks. |
| [toString()](#toString--)| Returns a string represents the current Worksheet object. |
| [startAccessCache(AccessCacheOptions)](#startAccessCache-accesscacheoptions-)| Starts the session that uses caches to access the data in this worksheet. |
| [closeAccessCache(AccessCacheOptions)](#closeAccessCache-accesscacheoptions-)| Closes the session that uses caches to access the data in this worksheet. |
| [convertFormulaReferenceStyle(string, boolean, number, number)](#convertFormulaReferenceStyle-string-boolean-number-number-)| Converts the formula reference style. |
| [calculateFormula(CalculationOptions, boolean)](#calculateFormula-calculationoptions-boolean-)| Calculates all formulas in this worksheet. |
| [refreshPivotTables()](#refreshPivotTables--)| Refreshes all the PivotTables in this Worksheet. |
| [refreshPivotTables(PivotTableRefreshOption)](#refreshPivotTables-pivottablerefreshoption-)| Refreshes all the PivotTables in this Worksheet. |


### getProtection() {#getProtection--}

Represents the various types of protection options available for a worksheet. Supports advanced protection options in ExcelXP and above version.

```javascript
getProtection() : Protection;
```


**Returns**

[Protection](./protection/)

**Remarks**

This property can protect worksheet in all versions of Excel file and support advanced protection options in ExcelXP and above version.

### getUniqueId() {#getUniqueId--}

Gets and sets the unique id, it is same as {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}.

```javascript
getUniqueId() : string;
```


### setUniqueId(string) {#setUniqueId-string-}

Gets and sets the unique id, it is same as {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}.

```javascript
setUniqueId(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getWorkbook() {#getWorkbook--}

Gets the workbook object which contains this sheet.

```javascript
getWorkbook() : Workbook;
```


**Returns**

[Workbook](./workbook/)

### getCells() {#getCells--}

Gets the [Cells](./cells/) collection.

```javascript
getCells() : Cells;
```


**Returns**

[Cells](./cells/)

### getQueryTables() {#getQueryTables--}

Gets [QueryTableCollection](./querytablecollection/) in the worksheet.

```javascript
getQueryTables() : QueryTableCollection;
```


**Returns**

[QueryTableCollection](./querytablecollection/)

### getPivotTables() {#getPivotTables--}

Gets all pivot tables in this worksheet.

```javascript
getPivotTables() : PivotTableCollection;
```


**Returns**

[PivotTableCollection](./pivottablecollection/)

### getType() {#getType--}

Represents worksheet type.

```javascript
getType() : SheetType;
```


**Returns**

[SheetType](./sheettype/)

### setType(SheetType) {#setType-sheettype-}

Represents worksheet type.

```javascript
setType(value: SheetType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SheetType](./sheettype/) | The value to set. |

### getName() {#getName--}

Gets or sets the name of the worksheet.

```javascript
getName() : string;
```


**Remarks**

The max length of sheet name is 31. And you cannot assign same name(case insensitive) to two worksheets. For example, you cannot set "SheetName1" to the first worksheet and set "SHEETNAME1" to the second worksheet.

### setName(string) {#setName-string-}

Gets or sets the name of the worksheet.

```javascript
setName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

The max length of sheet name is 31. And you cannot assign same name(case insensitive) to two worksheets. For example, you cannot set "SheetName1" to the first worksheet and set "SHEETNAME1" to the second worksheet.

### getShowFormulas() {#getShowFormulas--}

Indicates whether to show formulas or their results.

```javascript
getShowFormulas() : boolean;
```


### setShowFormulas(boolean) {#setShowFormulas-boolean-}

Indicates whether to show formulas or their results.

```javascript
setShowFormulas(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isGridlinesVisible() {#isGridlinesVisible--}

Gets or sets a value indicating whether the gridlines are visible.Default is true.

```javascript
isGridlinesVisible() : boolean;
```


### setIsGridlinesVisible(boolean) {#setIsGridlinesVisible-boolean-}

Gets or sets a value indicating whether the gridlines are visible.Default is true.

```javascript
setIsGridlinesVisible(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isRowColumnHeadersVisible() {#isRowColumnHeadersVisible--}

Gets or sets a value indicating whether the worksheet will display row and column headers. Default is true.

```javascript
isRowColumnHeadersVisible() : boolean;
```


### setIsRowColumnHeadersVisible(boolean) {#setIsRowColumnHeadersVisible-boolean-}

Gets or sets a value indicating whether the worksheet will display row and column headers. Default is true.

```javascript
setIsRowColumnHeadersVisible(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getPaneState() {#getPaneState--}

Indicates whether the pane has horizontal or vertical splits, and whether those splits are frozen.

```javascript
getPaneState() : PaneStateType;
```


**Returns**

[PaneStateType](./panestatetype/)

### getDisplayZeros() {#getDisplayZeros--}

True if zero values are displayed.

```javascript
getDisplayZeros() : boolean;
```


### setDisplayZeros(boolean) {#setDisplayZeros-boolean-}

True if zero values are displayed.

```javascript
setDisplayZeros(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getDisplayRightToLeft() {#getDisplayRightToLeft--}

Indicates if the specified worksheet is displayed from right to left instead of from left to right. Default is false.

```javascript
getDisplayRightToLeft() : boolean;
```


### setDisplayRightToLeft(boolean) {#setDisplayRightToLeft-boolean-}

Indicates if the specified worksheet is displayed from right to left instead of from left to right. Default is false.

```javascript
setDisplayRightToLeft(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isOutlineShown() {#isOutlineShown--}

Indicates whether to show outline.

```javascript
isOutlineShown() : boolean;
```


### setIsOutlineShown(boolean) {#setIsOutlineShown-boolean-}

Indicates whether to show outline.

```javascript
setIsOutlineShown(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isSelected() {#isSelected--}

Indicates whether this worksheet is selected when the workbook is opened.

```javascript
isSelected() : boolean;
```


### setIsSelected(boolean) {#setIsSelected-boolean-}

Indicates whether this worksheet is selected when the workbook is opened.

```javascript
setIsSelected(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getListObjects() {#getListObjects--}

Gets all ListObjects in this worksheet.

```javascript
getListObjects() : ListObjectCollection;
```


**Returns**

[ListObjectCollection](./listobjectcollection/)

### getTabId() {#getTabId--}

Specifies the internal identifier for the sheet.

```javascript
getTabId() : number;
```


### setTabId(number) {#setTabId-number-}

Specifies the internal identifier for the sheet.

```javascript
setTabId(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getHorizontalPageBreaks() {#getHorizontalPageBreaks--}

Gets the [HorizontalPageBreakCollection](./horizontalpagebreakcollection/) collection.

```javascript
getHorizontalPageBreaks() : HorizontalPageBreakCollection;
```


**Returns**

[HorizontalPageBreakCollection](./horizontalpagebreakcollection/)

### getVerticalPageBreaks() {#getVerticalPageBreaks--}

Gets the [VerticalPageBreakCollection](./verticalpagebreakcollection/) collection.

```javascript
getVerticalPageBreaks() : VerticalPageBreakCollection;
```


**Returns**

[VerticalPageBreakCollection](./verticalpagebreakcollection/)

### getHyperlinks() {#getHyperlinks--}

Gets the [HyperlinkCollection](./hyperlinkcollection/) collection.

```javascript
getHyperlinks() : HyperlinkCollection;
```


**Returns**

[HyperlinkCollection](./hyperlinkcollection/)

### getPageSetup() {#getPageSetup--}

Represents the page setup description in this sheet.

```javascript
getPageSetup() : PageSetup;
```


**Returns**

[PageSetup](./pagesetup/)

### getAutoFilter() {#getAutoFilter--}

Represents auto filter for the specified worksheet.

```javascript
getAutoFilter() : AutoFilter;
```


**Returns**

[AutoFilter](./autofilter/)

### getHasAutofilter() {#getHasAutofilter--}

Indicates whether this worksheet has auto filter.

```javascript
getHasAutofilter() : boolean;
```


### getTransitionEvaluation() {#getTransitionEvaluation--}

Indicates whether the Transition Formula Evaluation (Lotus compatibility) option is enabled.

```javascript
getTransitionEvaluation() : boolean;
```


### setTransitionEvaluation(boolean) {#setTransitionEvaluation-boolean-}

Indicates whether the Transition Formula Evaluation (Lotus compatibility) option is enabled.

```javascript
setTransitionEvaluation(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getTransitionEntry() {#getTransitionEntry--}

Indicates whether the Transition Formula Entry (Lotus compatibility) option is enabled.

```javascript
getTransitionEntry() : boolean;
```


### setTransitionEntry(boolean) {#setTransitionEntry-boolean-}

Indicates whether the Transition Formula Entry (Lotus compatibility) option is enabled.

```javascript
setTransitionEntry(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getVisibilityType() {#getVisibilityType--}

Indicates the visible state for this sheet.

```javascript
getVisibilityType() : VisibilityType;
```


**Returns**

[VisibilityType](./visibilitytype/)

### setVisibilityType(VisibilityType) {#setVisibilityType-visibilitytype-}

Indicates the visible state for this sheet.

```javascript
setVisibilityType(value: VisibilityType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [VisibilityType](./visibilitytype/) | The value to set. |

### isVisible() {#isVisible--}

Represents if the worksheet is visible.

```javascript
isVisible() : boolean;
```


### setIsVisible(boolean) {#setIsVisible-boolean-}

Represents if the worksheet is visible.

```javascript
setIsVisible(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getSparklineGroups() {#getSparklineGroups--}

Gets the sparkline groups in the worksheet.

```javascript
getSparklineGroups() : SparklineGroupCollection;
```


**Returns**

[SparklineGroupCollection](./sparklinegroupcollection/)

### getCharts() {#getCharts--}

Gets a [Chart](./chart/) collection

```javascript
getCharts() : ChartCollection;
```


**Returns**

[ChartCollection](./chartcollection/)

### getComments() {#getComments--}

Gets the [Comment](./comment/) collection.

```javascript
getComments() : CommentCollection;
```


**Returns**

[CommentCollection](./commentcollection/)

### getPictures() {#getPictures--}

Gets a [Picture](./picture/) collection.

```javascript
getPictures() : PictureCollection;
```


**Returns**

[PictureCollection](./picturecollection/)

### getTextBoxes() {#getTextBoxes--}

Gets a [TextBox](./textbox/) collection.

```javascript
getTextBoxes() : TextBoxCollection;
```


**Returns**

[TextBoxCollection](./textboxcollection/)

### getCheckBoxes() {#getCheckBoxes--}

Gets a [CheckBox](./checkbox/) collection.

```javascript
getCheckBoxes() : CheckBoxCollection;
```


**Returns**

[CheckBoxCollection](./checkboxcollection/)

### getOleObjects() {#getOleObjects--}

Represents a collection of [OleObject](./oleobject/) in a worksheet.

```javascript
getOleObjects() : OleObjectCollection;
```


**Returns**

[OleObjectCollection](./oleobjectcollection/)

### getShapes() {#getShapes--}

Returns all drawing shapes in this worksheet.

```javascript
getShapes() : ShapeCollection;
```


**Returns**

[ShapeCollection](./shapecollection/)

### getSlicers() {#getSlicers--}

Get the Slicer collection in the worksheet

```javascript
getSlicers() : SlicerCollection;
```


**Returns**

[SlicerCollection](./slicercollection/)

### getTimelines() {#getTimelines--}

Get the Timeline collection in the worksheet

```javascript
getTimelines() : TimelineCollection;
```


**Returns**

[TimelineCollection](./timelinecollection/)

### getIndex() {#getIndex--}

Gets the index of sheet in the worksheet collection.

```javascript
getIndex() : number;
```


### isProtected() {#isProtected--}

Indicates if the worksheet is protected.

```javascript
isProtected() : boolean;
```


### getValidations() {#getValidations--}

Gets the data validation setting collection in the worksheet.

```javascript
getValidations() : ValidationCollection;
```


**Returns**

[ValidationCollection](./validationcollection/)

### getAllowEditRanges() {#getAllowEditRanges--}

Gets the allow edit range collection in the worksheet.

```javascript
getAllowEditRanges() : ProtectedRangeCollection;
```


**Returns**

[ProtectedRangeCollection](./protectedrangecollection/)

### getErrorCheckOptions() {#getErrorCheckOptions--}

Gets error check setting applied on certain ranges.

```javascript
getErrorCheckOptions() : ErrorCheckOptionCollection;
```


**Returns**

[ErrorCheckOptionCollection](./errorcheckoptioncollection/)

### getOutline() {#getOutline--}

Gets the outline on this worksheet.

```javascript
getOutline() : Outline;
```


**Returns**

[Outline](./outline/)

### getFirstVisibleRow() {#getFirstVisibleRow--}

Represents first visible row index.

```javascript
getFirstVisibleRow() : number;
```


### setFirstVisibleRow(number) {#setFirstVisibleRow-number-}

Represents first visible row index.

```javascript
setFirstVisibleRow(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getFirstVisibleColumn() {#getFirstVisibleColumn--}

Represents first visible column index.

```javascript
getFirstVisibleColumn() : number;
```


### setFirstVisibleColumn(number) {#setFirstVisibleColumn-number-}

Represents first visible column index.

```javascript
setFirstVisibleColumn(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getZoom() {#getZoom--}

Represents the scaling factor in percentage. It should be between 10 and 400.

```javascript
getZoom() : number;
```


**Remarks**

Please set the view type first.

### setZoom(number) {#setZoom-number-}

Represents the scaling factor in percentage. It should be between 10 and 400.

```javascript
setZoom(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

Please set the view type first.

### getViewType() {#getViewType--}

Gets and sets the view type.

```javascript
getViewType() : ViewType;
```


**Returns**

[ViewType](./viewtype/)

### setViewType(ViewType) {#setViewType-viewtype-}

Gets and sets the view type.

```javascript
setViewType(value: ViewType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ViewType](./viewtype/) | The value to set. |

### isPageBreakPreview() {#isPageBreakPreview--}

Indicates whether the specified worksheet is shown in normal view or page break preview.

```javascript
isPageBreakPreview() : boolean;
```


### setIsPageBreakPreview(boolean) {#setIsPageBreakPreview-boolean-}

Indicates whether the specified worksheet is shown in normal view or page break preview.

```javascript
setIsPageBreakPreview(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isRulerVisible() {#isRulerVisible--}

Indicates whether the ruler is visible. This property is only applied for page break preview.

```javascript
isRulerVisible() : boolean;
```


### setIsRulerVisible(boolean) {#setIsRulerVisible-boolean-}

Indicates whether the ruler is visible. This property is only applied for page break preview.

```javascript
setIsRulerVisible(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getTabColor() {#getTabColor--}

Represents worksheet tab color.

```javascript
getTabColor() : Color;
```


**Returns**

[Color](./color/)

**Remarks**

This feature is only supported in ExcelXP(Excel2002) and later versions. If you save file as Excel97 or Excel2000 format, it will be omitted.

### setTabColor(Color) {#setTabColor-color-}

Represents worksheet tab color.

```javascript
setTabColor(value: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](./color/) | The value to set. |

**Remarks**

This feature is only supported in ExcelXP(Excel2002) and later versions. If you save file as Excel97 or Excel2000 format, it will be omitted.

### getCodeName() {#getCodeName--}

Gets worksheet code name.

```javascript
getCodeName() : string;
```


### setCodeName(string) {#setCodeName-string-}

Gets worksheet code name.

```javascript
setCodeName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getBackgroundImage() {#getBackgroundImage--}

Gets and sets worksheet background image.

```javascript
getBackgroundImage() : number[];
```


**Returns**

number[]

### setBackgroundImage(number[]) {#setBackgroundImage-number[]-}

Gets and sets worksheet background image.

```javascript
setBackgroundImage(value: number[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number[] | The value to set. |

### getConditionalFormattings() {#getConditionalFormattings--}

Gets the ConditionalFormattings in the worksheet.

```javascript
getConditionalFormattings() : ConditionalFormattingCollection;
```


**Returns**

[ConditionalFormattingCollection](./conditionalformattingcollection/)

### getActiveCell() {#getActiveCell--}

Gets or sets the active cell in the worksheet.

```javascript
getActiveCell() : string;
```


### setActiveCell(string) {#setActiveCell-string-}

Gets or sets the active cell in the worksheet.

```javascript
setActiveCell(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getCustomProperties() {#getCustomProperties--}

Gets an object representing the identifier information associated with a worksheet.

```javascript
getCustomProperties() : CustomPropertyCollection;
```


**Returns**

[CustomPropertyCollection](./custompropertycollection/)

**Remarks**

Worksheet.CustomProperties provide a preferred mechanism for storing arbitrary data. It supports legacy third-party document components, as well as those situations that have a stringent need for binary parts.

### getSmartTagSetting() {#getSmartTagSetting--}

Gets all [SmartTagCollection](./smarttagcollection/) objects of the worksheet.

```javascript
getSmartTagSetting() : SmartTagSetting;
```


**Returns**

[SmartTagSetting](./smarttagsetting/)

### getScenarios() {#getScenarios--}

Gets the collection of [Scenario](./scenario/).

```javascript
getScenarios() : ScenarioCollection;
```


**Returns**

[ScenarioCollection](./scenariocollection/)

### getCellWatches() {#getCellWatches--}

Gets collection of cells on this worksheet being watched in the 'watch window'.

```javascript
getCellWatches() : CellWatchCollection;
```


**Returns**

[CellWatchCollection](./cellwatchcollection/)

### dispose() {#dispose--}

Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources.

```javascript
dispose() : void;
```


### getPanes() {#getPanes--}

Gets the window panes.

```javascript
getPanes() : PaneCollection;
```


**Returns**

[PaneCollection](./panecollection/)

**Remarks**

If the window is not split or frozen.

### freezePanes(number, number, number, number) {#freezePanes-number-number-number-number-}

Freezes panes at the specified cell in the worksheet.

```javascript
freezePanes(row: number, column: number, freezedRows: number, freezedColumns: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | Row index. |
| column | number | Column index. |
| freezedRows | number | Number of visible rows in top pane, no more than row index. |
| freezedColumns | number | Number of visible columns in left pane, no more than column index. |

**Remarks**

<p>Row index and column index cannot all be zero. Number of rows and number of columns also cannot all be zero.</p> <p>The first two parameters specify the froze position and the last two parameters specify the area frozen on the left top pane.</p>

### freezePanes(string, number, number) {#freezePanes-string-number-number-}

Freezes panes at the specified cell in the worksheet.

```javascript
freezePanes(cellName: string, freezedRows: number, freezedColumns: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | string | Cell name. |
| freezedRows | number | Number of visible rows in top pane, no more than row index. |
| freezedColumns | number | Number of visible columns in left pane, no more than column index. |

**Remarks**

Row index and column index cannot all be zero. Number of rows and number of columns also cannot all be zero.

### getFreezedPanes(number, number, number, number) {#getFreezedPanes-number-number-number-number-}

Gets the freeze panes.

```javascript
getFreezedPanes(row: number, column: number, freezedRows: number, freezedColumns: number) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | Row index. |
| column | number | Column index. |
| freezedRows | number | Number of visible rows in top pane, no more than row index. |
| freezedColumns | number | Number of visible columns in left pane, no more than column index. |

**Returns**

Return whether the worksheet is frozen

### split() {#split--}

Splits window.

```javascript
split() : void;
```


### unFreezePanes() {#unFreezePanes--}

Unfreezes panes in the worksheet.

```javascript
unFreezePanes() : void;
```


### removeSplit() {#removeSplit--}

Removes split window.

```javascript
removeSplit() : void;
```


### addPageBreaks(string) {#addPageBreaks-string-}

Adds page break.

```javascript
addPageBreaks(cellName: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | string |  |

### copy(Worksheet) {#copy-worksheet-}

Copies contents and formats from another worksheet.

```javascript
copy(sourceSheet: Worksheet) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceSheet | [Worksheet](./worksheet/) | Source worksheet. |

### copy(Worksheet, CopyOptions) {#copy-worksheet-copyoptions-}

Copies contents and formats from another worksheet.

```javascript
copy(sourceSheet: Worksheet, copyOptions: CopyOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceSheet | [Worksheet](./worksheet/) | Source worksheet. |
| copyOptions | [CopyOptions](./copyoptions/) |  |

**Remarks**

You can copy data from another worksheet in the same file or another file. However, this method does not support to copy drawing objects, such as comments, images and charts.

### autoFitColumn(number, number, number) {#autoFitColumn-number-number-number-}

Autofits the column width.

```javascript
autoFitColumn(columnIndex: number, firstRow: number, lastRow: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | number | Column index. |
| firstRow | number | First row index. |
| lastRow | number | Last row index. |

**Remarks**

This method autofits a row based on content in a range of cells within the row.

### autoFitColumn(number) {#autoFitColumn-number-}

Autofits the column width.

```javascript
autoFitColumn(columnIndex: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | number | Column index. |

**Remarks**

AutoFitColumn is an imprecise function.

### autoFitColumns() {#autoFitColumns--}

Autofits all columns in this worksheet.

```javascript
autoFitColumns() : void;
```


### autoFitColumns(AutoFitterOptions) {#autoFitColumns-autofitteroptions-}

Autofits all columns in this worksheet.

```javascript
autoFitColumns(options: AutoFitterOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [AutoFitterOptions](./autofitteroptions/) | The auto fitting options |

### autoFitColumns(number, number) {#autoFitColumns-number-number-}

Autofits the columns width.

```javascript
autoFitColumns(firstColumn: number, lastColumn: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstColumn | number | First column index. |
| lastColumn | number | Last column index. |

**Remarks**

AutoFitColumn is an imprecise function.

### autoFitColumns(number, number, AutoFitterOptions) {#autoFitColumns-number-number-autofitteroptions-}

Autofits the columns width.

```javascript
autoFitColumns(firstColumn: number, lastColumn: number, options: AutoFitterOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstColumn | number | First column index. |
| lastColumn | number | Last column index. |
| options | [AutoFitterOptions](./autofitteroptions/) | The auto fitting options |

**Remarks**

AutoFitColumn is an imprecise function.

### autoFitColumns(number, number, number, number) {#autoFitColumns-number-number-number-number-}

Autofits the columns width.

```javascript
autoFitColumns(firstRow: number, firstColumn: number, lastRow: number, lastColumn: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | number | First row index. |
| firstColumn | number | First column index. |
| lastRow | number | Last row index. |
| lastColumn | number | Last column index. |

**Remarks**

AutoFitColumn is an imprecise function.

### autoFitColumns(number, number, number, number, AutoFitterOptions) {#autoFitColumns-number-number-number-number-autofitteroptions-}

Autofits the columns width.

```javascript
autoFitColumns(firstRow: number, firstColumn: number, lastRow: number, lastColumn: number, options: AutoFitterOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | number | First row index. |
| firstColumn | number | First column index. |
| lastRow | number | Last row index. |
| lastColumn | number | Last column index. |
| options | [AutoFitterOptions](./autofitteroptions/) | The auto fitting options |

**Remarks**

AutoFitColumn is an imprecise function.

### autoFitRow(number, number, number) {#autoFitRow-number-number-number-}

Autofits the row height.

```javascript
autoFitRow(rowIndex: number, firstColumn: number, lastColumn: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | number | Row index. |
| firstColumn | number | First column index. |
| lastColumn | number | Last column index. |

**Remarks**

This method autofits a row based on content in a range of cells within the row.

### autoFitRow(number, number, number, AutoFitterOptions) {#autoFitRow-number-number-number-autofitteroptions-}

Autofits the row height.

```javascript
autoFitRow(rowIndex: number, firstColumn: number, lastColumn: number, options: AutoFitterOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | number | Row index. |
| firstColumn | number | First column index. |
| lastColumn | number | Last column index. |
| options | [AutoFitterOptions](./autofitteroptions/) | The auto fitter options |

**Remarks**

This method autofits a row based on content in a range of cells within the row.

### autoFitRow(number, number, number, number) {#autoFitRow-number-number-number-number-}

Autofits row height in a rectangle range.

```javascript
autoFitRow(startRow: number, endRow: number, startColumn: number, endColumn: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | number | Start row index. |
| endRow | number | End row index. |
| startColumn | number | Start column index. |
| endColumn | number | End column index. |

### autoFitRow(number) {#autoFitRow-number-}

Autofits the row height.

```javascript
autoFitRow(rowIndex: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | number | Row index. |

**Remarks**

AutoFitRow is an imprecise function.

### autoFitRows() {#autoFitRows--}

Autofits all rows in this worksheet.

```javascript
autoFitRows() : void;
```


### autoFitRows(boolean) {#autoFitRows-boolean-}

Autofits all rows in this worksheet.

```javascript
autoFitRows(onlyAuto: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| onlyAuto | boolean | True,only autofits the row height when row height is not customed. |

### autoFitRows(AutoFitterOptions) {#autoFitRows-autofitteroptions-}

Autofits all rows in this worksheet.

```javascript
autoFitRows(options: AutoFitterOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [AutoFitterOptions](./autofitteroptions/) | The auto fitter options |

### autoFitRows(number, number) {#autoFitRows-number-number-}

Autofits row height in a range.

```javascript
autoFitRows(startRow: number, endRow: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | number | Start row index. |
| endRow | number | End row index. |

### autoFitRows(number, number, AutoFitterOptions) {#autoFitRows-number-number-autofitteroptions-}

Autofits row height in a range.

```javascript
autoFitRows(startRow: number, endRow: number, options: AutoFitterOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | number | Start row index. |
| endRow | number | End row index. |
| options | [AutoFitterOptions](./autofitteroptions/) | The options of auto fitter. |

### getAdvancedFilter() {#getAdvancedFilter--}

Gets the settings of advanced filter.

```javascript
getAdvancedFilter() : AdvancedFilter;
```


**Returns**

[AdvancedFilter](./advancedfilter/)

### advanced_Filter(boolean, string, string, string, boolean) {#advanced_Filter-boolean-string-string-string-boolean-}

Filters data using complex criteria.

```javascript
advanced_Filter(isFilter: boolean, listRange: string, criteriaRange: string, copyTo: string, uniqueRecordOnly: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isFilter | boolean | Indicates whether filtering the list in place. |
| listRange | string | The list range. |
| criteriaRange | string | The criteria range. |
| copyTo | string | The range where copying data to. |
| uniqueRecordOnly | boolean | Only displaying or copying unique rows. |

### removeAutoFilter() {#removeAutoFilter--}

Removes the auto filter of the worksheet.

```javascript
removeAutoFilter() : void;
```


### setVisible(boolean, boolean) {#setVisible-boolean-boolean-}

Sets the visible options.

```javascript
setVisible(isVisible: boolean, ignoreError: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isVisible | boolean | Whether the worksheet is visible |
| ignoreError | boolean | Whether to ignore error if this option is not valid. |

### selectRange(number, number, number, number, boolean) {#selectRange-number-number-number-number-boolean-}

Selects a range.

```javascript
selectRange(startRow: number, startColumn: number, totalRows: number, totalColumns: number, removeOthers: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | number | The start row. |
| startColumn | number | The start column |
| totalRows | number | The number of rows. |
| totalColumns | number | The number of columns |
| removeOthers | boolean | True means removing other selected range and only select this range. |

### removeAllDrawingObjects() {#removeAllDrawingObjects--}

Removes all drawing objects in this worksheet.

```javascript
removeAllDrawingObjects() : void;
```


### clearComments() {#clearComments--}

Clears all comments in designer spreadsheet.

```javascript
clearComments() : void;
```


### protect(ProtectionType) {#protect-protectiontype-}

Protects worksheet.

```javascript
protect(type: ProtectionType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [ProtectionType](./protectiontype/) | Protection type. |

**Remarks**

This method protects worksheet without password. It can protect worksheet in all versions of Excel file.

### protect(ProtectionType, string, string) {#protect-protectiontype-string-string-}

Protects worksheet.

```javascript
protect(type: ProtectionType, password: string, oldPassword: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [ProtectionType](./protectiontype/) | Protection type. |
| password | string | Password. |
| oldPassword | string | If the worksheet is already protected by a password, please supply the old password. 		/// Otherwise, you can set a null value or blank string to this parameter. |

**Remarks**

This method can protect worksheet in all versions of Excel file.

### unprotect() {#unprotect--}

Unprotects worksheet.

```javascript
unprotect() : void;
```


**Remarks**

This method unprotects worksheet which is protected without password.

### unprotect(string) {#unprotect-string-}

Unprotects worksheet.

```javascript
unprotect(password: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | string | Password |

**Remarks**

If the worksheet is protected without a password, you can set a null value or blank string to password parameter.

### moveTo(number) {#moveTo-number-}

Moves the sheet to another location in the spreadsheet.

```javascript
moveTo(index: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | Destination sheet index. |

### replace(string, string) {#replace-string-string-}

Replaces all cells' text with a new string.

```javascript
replace(oldString: string, newString: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| oldString | string | Old string value. |
| newString | string | New string value. |

### getPrintingPageBreaks(ImageOrPrintOptions) {#getPrintingPageBreaks-imageorprintoptions-}

Gets automatic page breaks.

```javascript
getPrintingPageBreaks(options: ImageOrPrintOptions) : CellArea[];
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [ImageOrPrintOptions](./imageorprintoptions/) | The print options |

**Returns**

The automatic page breaks areas.

**Remarks**

Each cell area represents a paper.

### toString() {#toString--}

Returns a string represents the current Worksheet object.

```javascript
toString() : string;
```


### startAccessCache(AccessCacheOptions) {#startAccessCache-accesscacheoptions-}

Starts the session that uses caches to access the data in this worksheet.

```javascript
startAccessCache(opts: AccessCacheOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| opts | [AccessCacheOptions](./accesscacheoptions/) | options of data access |

**Remarks**

After finishing the access to the data, [CloseAccessCache(AccessCacheOptions)](./closeaccesscache(accesscacheoptions)/) should be invoked with same options to clear all caches and recover normal access mode.

### closeAccessCache(AccessCacheOptions) {#closeAccessCache-accesscacheoptions-}

Closes the session that uses caches to access the data in this worksheet.

```javascript
closeAccessCache(opts: AccessCacheOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| opts | [AccessCacheOptions](./accesscacheoptions/) | options of data access |

### convertFormulaReferenceStyle(string, boolean, number, number) {#convertFormulaReferenceStyle-string-boolean-number-number-}

Converts the formula reference style.

```javascript
convertFormulaReferenceStyle(formula: string, toR1C1: boolean, baseCellRow: number, baseCellColumn: number) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | string | The formula to be converted. |
| toR1C1 | boolean | Which reference style to convert the formula to.         /// If the original formula is of A1 reference style,         /// then this value should be true so the formula will be converted from A1 to R1C1 reference style;         /// If the original formula is of R1C1 reference style,         /// then this value should be false so the formula will be converted from R1C1 to A1 reference style; |
| baseCellRow | number | The row index of the base cell. |
| baseCellColumn | number | The column index of the base cell. |

**Returns**

The converted formula.

### calculateFormula(CalculationOptions, boolean) {#calculateFormula-calculationoptions-boolean-}

Calculates all formulas in this worksheet.

```javascript
calculateFormula(options: CalculationOptions, recursive: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [CalculationOptions](./calculationoptions/) | Options for calculation |
| recursive | boolean | True means if the worksheet' cells depend on the cells of other worksheets,         ///  the dependent cells in other worksheets will be calculated too.         ///  False means all the formulas in the worksheet have been calculated and the values are right. |

### refreshPivotTables() {#refreshPivotTables--}

Refreshes all the PivotTables in this Worksheet.

```javascript
refreshPivotTables() : void;
```


### refreshPivotTables(PivotTableRefreshOption) {#refreshPivotTables-pivottablerefreshoption-}

Refreshes all the PivotTables in this Worksheet.

```javascript
refreshPivotTables(option: PivotTableRefreshOption) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| option | [PivotTableRefreshOption](./pivottablerefreshoption/) | The option for refreshing data source of pivot table. |


