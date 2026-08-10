---
title: "Worksheet Class"
linktitle: "Worksheet"
articleTitle: "Worksheet"
second_title: "Aspose.Cells for PHP via Java"
description: "Encapsulates the object that represents a single worksheet."
type: docs
weight: 7600
url: /php/aspose.cells/worksheet/
---

## Worksheet class

Encapsulates the object that represents a single worksheet.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Protection](#protection) | Protection | Represents the various types of protection options available for a worksheet. Supports advanced protection options in Ex |
| [UniqueId](#uniqueid) | String | Gets and sets the unique id, it is same as {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. |
| [Workbook](#workbook) | Workbook | Gets the workbook object which contains this sheet. |
| [Cells](#cells) | Cells | Gets the Cells collection. |
| [QueryTables](#querytables) | QueryTableCollection | Gets QueryTableCollection in the worksheet. |
| [Type](#type) | Number | Represents worksheet type. The value of the property is SheetType integer constant. |
| [Name](#name) | String | Gets or sets the name of the worksheet. The max length of sheet name is 31. And you cannot assign same name(case insensi |
| [ShowFormulas](#showformulas) | boolean | Indicates whether to show formulas or their results. |
| [ShowDataTypeIcons](#showdatatypeicons) | boolean |  |
| [IsGridlinesVisible](#isgridlinesvisible) | boolean | Gets or sets a value indicating whether the gridlines are visible.Default is true. |
| [IsRowColumnHeadersVisible](#isrowcolumnheadersvisible) | boolean | Gets or sets a value indicating whether the worksheet will display row and column headers. Default is true. |
| [PaneState](#panestate) | Number | Indicates whether the pane has horizontal or vertical splits, and whether those splits are frozen. The value of the prop |
| [DisplayZeros](#displayzeros) | boolean | True if zero values are displayed. |
| [DisplayRightToLeft](#displayrighttoleft) | boolean | Indicates if the specified worksheet is displayed from right to left instead of from left to right. Default is false. |
| [IsOutlineShown](#isoutlineshown) | boolean | Indicates whether to show outline. |
| [IsSelected](#isselected) | boolean | Indicates whether this worksheet is selected when the workbook is opened. |
| [PivotTables](#pivottables) | PivotTableCollection | Gets all pivot tables in this worksheet. |
| [ListObjects](#listobjects) | ListObjectCollection | Gets all ListObjects in this worksheet. |
| [TabId](#tabid) | Number | Specifies the internal identifier for the sheet. |
| [HorizontalPageBreaks](#horizontalpagebreaks) | HorizontalPageBreakCollection | Gets the HorizontalPageBreakCollection collection. |
| [VerticalPageBreaks](#verticalpagebreaks) | VerticalPageBreakCollection | Gets the VerticalPageBreakCollection collection. |
| [Hyperlinks](#hyperlinks) | HyperlinkCollection | Gets the HyperlinkCollection collection. |
| [PageSetup](#pagesetup) | PageSetup | Represents the page setup description in this sheet. |
| [AutoFilter](#autofilter) | AutoFilter | Represents auto filter for the specified worksheet. |
| [HasAutofilter](#hasautofilter) | boolean | Indicates whether this worksheet has auto filter. |
| [TransitionEvaluation](#transitionevaluation) | boolean | Indicates whether the Transition Formula Evaluation (Lotus compatibility) option is enabled. |
| [TransitionEntry](#transitionentry) | boolean | Indicates whether the Transition Formula Entry (Lotus compatibility) option is enabled. |
| [VisibilityType](#visibilitytype) | Number | Indicates the visible state for this sheet. The value of the property is VisibilityType integer constant. |
| [IsVisible](#isvisible) | boolean | Represents if the worksheet is visible. |
| [SparklineGroups](#sparklinegroups) | SparklineGroupCollection | Gets the sparkline groups in the worksheet. |
| [Charts](#charts) | ChartCollection | Gets a Chart collection |
| [Comments](#comments) | CommentCollection | Gets the Comment collection. |
| [Pictures](#pictures) | PictureCollection | Gets a Picture collection. |
| [TextBoxes](#textboxes) | TextBoxCollection | Gets a TextBox collection. |
| [CheckBoxes](#checkboxes) | CheckBoxCollection | Gets a CheckBox collection. |
| [OleObjects](#oleobjects) | OleObjectCollection | Represents a collection of OleObject in a worksheet. |
| [Shapes](#shapes) | ShapeCollection | Returns all drawing shapes in this worksheet. |
| [Slicers](#slicers) | SlicerCollection | Get the Slicer collection in the worksheet |
| [Timelines](#timelines) | TimelineCollection | Get the Timeline collection in the worksheet |
| [Index](#index) | Number | Gets the index of sheet in the worksheet collection. |
| [IsProtected](#isprotected) | boolean | Indicates if the worksheet is protected. |
| [Validations](#validations) | ValidationCollection | Gets the data validation setting collection in the worksheet. |
| [AllowEditRanges](#alloweditranges) | ProtectedRangeCollection | Gets the allow edit range collection in the worksheet. |
| [ErrorCheckOptions](#errorcheckoptions) | ErrorCheckOptionCollection | Gets error check setting applied on certain ranges. |
| [Outline](#outline) | Outline | Gets the outline on this worksheet. |
| [FirstVisibleRow](#firstvisiblerow) | Number | Represents first visible row index. |
| [FirstVisibleColumn](#firstvisiblecolumn) | Number | Represents first visible column index. |
| [Zoom](#zoom) | Number | Represents the scaling factor in percentage. It should be between 10 and 400. Please set the view type first. |
| [ViewType](#viewtype) | Number | Gets and sets the view type. The value of the property is ViewType integer constant. |
| [IsPageBreakPreview](#ispagebreakpreview) | boolean | Indicates whether the specified worksheet is shown in normal view or page break preview. |
| [IsRulerVisible](#isrulervisible) | boolean | Indicates whether the ruler is visible. This property is only applied for page break preview. |
| [TabColor](#tabcolor) | Color | Represents worksheet tab color. This feature is only supported in ExcelXP(Excel2002) and later versions. If you save fil |
| [GridlineColor](#gridlinecolor) | Color |  |
| [CodeName](#codename) | String | Gets worksheet code name. |
| [BackgroundImage](#backgroundimage) | byte[] | Gets and sets worksheet background image. |
| [ConditionalFormattings](#conditionalformattings) | ConditionalFormattingCollection | Gets the ConditionalFormattings in the worksheet. |
| [ActiveCell](#activecell) | String | Gets or sets the active cell in the worksheet. |
| [CustomProperties](#customproperties) | CustomPropertyCollection | Gets an object representing the identifier information associated with a worksheet. Worksheet.CustomProperties provide a |
| [SmartTagSetting](#smarttagsetting) | SmartTagSetting | Gets all SmartTagCollection objects of the worksheet. |
| [Scenarios](#scenarios) | ScenarioCollection | Gets the collection of Scenario . |
| [CellWatches](#cellwatches) | CellWatchCollection | Gets collection of cells on this worksheet being watched in the 'watch window'. |

## Methods

| Name | Description |
| --- | --- |
| [protect](#protect) | Protects worksheet.

This method protects worksheet without password. It can protect worksheet in all versions of Excel  |
| [unprotect](#unprotect) | Unprotects worksheet.

This method unprotects worksheet which is protected without password. |
| [moveTo](#moveto) | Moves the sheet to another location in the spreadsheet. |
| [replace](#replace) | Replaces all cells' text with a new string. |
| [getSelectedRanges](#getselectedranges) | Gets selected ranges of cells in the designer spreadsheet. |
| [getSelectedAreas](#getselectedareas) |  |
| [getPrintingPageBreaks](#getprintingpagebreaks) | Gets automatic page breaks.

Each cell area represents a paper. |
| [toString](#tostring) | Returns a string represents the current Worksheet object. |
| [startAccessCache](#startaccesscache) | Starts the session that uses caches to access the data in this worksheet.

After finishing the access to the data, close |
| [closeAccessCache](#closeaccesscache) | Closes the session that uses caches to access the data in this worksheet. |
| [convertFormulaReferenceStyle](#convertformulareferencestyle) | Converts the formula reference style. |
| [calculateFormula](#calculateformula) | Calculates a formula. |
| [calculateArrayFormula](#calculatearrayformula) | Calculates a formula as array formula. |
| [xmlMapQuery](#xmlmapquery) | Query cell areas that mapped/linked to the specific path of xml map. |
| [refreshPivotTables](#refreshpivottables) | Refreshes all the PivotTables in this Worksheet. |
| [dispose](#dispose) | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [getPanes](#getpanes) | Gets the window panes.

If the window is not split or frozen. |
| [freezePanes](#freezepanes) | Freezes panes at the specified cell in the worksheet.

Row index and column index cannot all be zero. Number of rows and |
| [getFreezedPanes](#getfreezedpanes) | Gets the freeze panes. |
| [split](#split) | Splits window. |
| [unFreezePanes](#unfreezepanes) | Unfreezes panes in the worksheet. |
| [removeSplit](#removesplit) | Removes split window. |
| [addPageBreaks](#addpagebreaks) | Adds page break. |
| [copy](#copy) | Copies contents and formats from another worksheet. |
| [autoFitColumn](#autofitcolumn) | Autofits the column width.

This method autofits a row based on content in a range of cells within the row. |
| [autoFitColumns](#autofitcolumns) | Autofits all columns in this worksheet. |
| [autoFitRow](#autofitrow) | Autofits the row height.

This method autofits a row based on content in a range of cells within the row. |
| [autoFitRows](#autofitrows) | Autofits all rows in this worksheet. |
| [filter](#filter) |  |
| [getAdvancedFilter](#getadvancedfilter) | Gets the settings of advanced filter. |
| [advancedFilter](#advancedfilter) | Filters data using complex criteria. |
| [removeAutoFilter](#removeautofilter) | Removes the auto filter of the worksheet. |
| [setVisible](#setvisible) | Sets the visible options. |
| [selectRange](#selectrange) | Selects a range. |
| [removeAllDrawingObjects](#removealldrawingobjects) | Removes all drawing objects in this worksheet. |
| [clearComments](#clearcomments) | Clears all comments in designer spreadsheet. |
| [getAllPictures](#getallpictures) |  |

### Worksheet.Protection property {#protection}

Represents the various types of protection options available for a worksheet. Supports advanced protection options in ExcelXP and above version. This property can protect worksheet in all versions of Excel file and support advanced protection options in ExcelXP and above version.

**Type:** Protection

### Worksheet.UniqueId property {#uniqueid}

Gets and sets the unique id, it is same as {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}.

**Type:** String

### Worksheet.Workbook property {#workbook}

Gets the workbook object which contains this sheet.

**Type:** Workbook

### Worksheet.Cells property {#cells}

Gets the Cells collection.

**Type:** Cells

### Worksheet.QueryTables property {#querytables}

Gets QueryTableCollection in the worksheet.

**Type:** QueryTableCollection

### Worksheet.Type property {#type}

Represents worksheet type. The value of the property is SheetType integer constant.

**Type:** Number

### Worksheet.Name property {#name}

Gets or sets the name of the worksheet. The max length of sheet name is 31. And you cannot assign same name(case insensitive) to two worksheets. For example, you cannot set "SheetName1" to the first worksheet and set "SHEETNAME1" to the second worksheet.

**Type:** String

### Worksheet.ShowFormulas property {#showformulas}

Indicates whether to show formulas or their results.

**Type:** boolean

### Worksheet.ShowDataTypeIcons property {#showdatatypeicons}

**Type:** boolean

### Worksheet.IsGridlinesVisible property {#isgridlinesvisible}

Gets or sets a value indicating whether the gridlines are visible.Default is true.

**Type:** boolean

### Worksheet.IsRowColumnHeadersVisible property {#isrowcolumnheadersvisible}

Gets or sets a value indicating whether the worksheet will display row and column headers. Default is true.

**Type:** boolean

### Worksheet.PaneState property {#panestate}

Indicates whether the pane has horizontal or vertical splits, and whether those splits are frozen. The value of the property is PaneStateType integer constant.

**Type:** Number

### Worksheet.DisplayZeros property {#displayzeros}

True if zero values are displayed.

**Type:** boolean

### Worksheet.DisplayRightToLeft property {#displayrighttoleft}

Indicates if the specified worksheet is displayed from right to left instead of from left to right. Default is false.

**Type:** boolean

### Worksheet.IsOutlineShown property {#isoutlineshown}

Indicates whether to show outline.

**Type:** boolean

### Worksheet.IsSelected property {#isselected}

Indicates whether this worksheet is selected when the workbook is opened.

**Type:** boolean

### Worksheet.PivotTables property {#pivottables}

Gets all pivot tables in this worksheet.

**Type:** PivotTableCollection

### Worksheet.ListObjects property {#listobjects}

Gets all ListObjects in this worksheet.

**Type:** ListObjectCollection

### Worksheet.TabId property {#tabid}

Specifies the internal identifier for the sheet.

**Type:** Number

### Worksheet.HorizontalPageBreaks property {#horizontalpagebreaks}

Gets the HorizontalPageBreakCollection collection.

**Type:** HorizontalPageBreakCollection

### Worksheet.VerticalPageBreaks property {#verticalpagebreaks}

Gets the VerticalPageBreakCollection collection.

**Type:** VerticalPageBreakCollection

### Worksheet.Hyperlinks property {#hyperlinks}

Gets the HyperlinkCollection collection.

**Type:** HyperlinkCollection

### Worksheet.PageSetup property {#pagesetup}

Represents the page setup description in this sheet.

**Type:** PageSetup

### Worksheet.AutoFilter property {#autofilter}

Represents auto filter for the specified worksheet.

**Type:** AutoFilter

### Worksheet.HasAutofilter property {#hasautofilter}

Indicates whether this worksheet has auto filter.

**Type:** boolean

### Worksheet.TransitionEvaluation property {#transitionevaluation}

Indicates whether the Transition Formula Evaluation (Lotus compatibility) option is enabled.

**Type:** boolean

### Worksheet.TransitionEntry property {#transitionentry}

Indicates whether the Transition Formula Entry (Lotus compatibility) option is enabled.

**Type:** boolean

### Worksheet.VisibilityType property {#visibilitytype}

Indicates the visible state for this sheet. The value of the property is VisibilityType integer constant.

**Type:** Number

### Worksheet.IsVisible property {#isvisible}

Represents if the worksheet is visible.

**Type:** boolean

### Worksheet.SparklineGroups property {#sparklinegroups}

Gets the sparkline groups in the worksheet.

**Type:** SparklineGroupCollection

### Worksheet.Charts property {#charts}

Gets a Chart collection

**Type:** ChartCollection

### Worksheet.Comments property {#comments}

Gets the Comment collection.

**Type:** CommentCollection

### Worksheet.Pictures property {#pictures}

Gets a Picture collection.

**Type:** PictureCollection

### Worksheet.TextBoxes property {#textboxes}

Gets a TextBox collection.

**Type:** TextBoxCollection

### Worksheet.CheckBoxes property {#checkboxes}

Gets a CheckBox collection.

**Type:** CheckBoxCollection

### Worksheet.OleObjects property {#oleobjects}

Represents a collection of OleObject in a worksheet.

**Type:** OleObjectCollection

### Worksheet.Shapes property {#shapes}

Returns all drawing shapes in this worksheet.

**Type:** ShapeCollection

### Worksheet.Slicers property {#slicers}

Get the Slicer collection in the worksheet

**Type:** SlicerCollection

### Worksheet.Timelines property {#timelines}

Get the Timeline collection in the worksheet

**Type:** TimelineCollection

### Worksheet.Index property {#index}

Gets the index of sheet in the worksheet collection.

**Type:** Number

### Worksheet.IsProtected property {#isprotected}

Indicates if the worksheet is protected.

**Type:** boolean

### Worksheet.Validations property {#validations}

Gets the data validation setting collection in the worksheet.

**Type:** ValidationCollection

### Worksheet.AllowEditRanges property {#alloweditranges}

Gets the allow edit range collection in the worksheet.

**Type:** ProtectedRangeCollection

### Worksheet.ErrorCheckOptions property {#errorcheckoptions}

Gets error check setting applied on certain ranges.

**Type:** ErrorCheckOptionCollection

### Worksheet.Outline property {#outline}

Gets the outline on this worksheet.

**Type:** Outline

### Worksheet.FirstVisibleRow property {#firstvisiblerow}

Represents first visible row index.

**Type:** Number

### Worksheet.FirstVisibleColumn property {#firstvisiblecolumn}

Represents first visible column index.

**Type:** Number

### Worksheet.Zoom property {#zoom}

Represents the scaling factor in percentage. It should be between 10 and 400. Please set the view type first.

**Type:** Number

### Worksheet.ViewType property {#viewtype}

Gets and sets the view type. The value of the property is ViewType integer constant.

**Type:** Number

### Worksheet.IsPageBreakPreview property {#ispagebreakpreview}

Indicates whether the specified worksheet is shown in normal view or page break preview.

**Type:** boolean

### Worksheet.IsRulerVisible property {#isrulervisible}

Indicates whether the ruler is visible. This property is only applied for page break preview.

**Type:** boolean

### Worksheet.TabColor property {#tabcolor}

Represents worksheet tab color. This feature is only supported in ExcelXP(Excel2002) and later versions. If you save file as Excel97 or Excel2000 format, it will be omitted.

**Type:** Color

### Worksheet.GridlineColor property {#gridlinecolor}

**Type:** Color

### Worksheet.CodeName property {#codename}

Gets worksheet code name.

**Type:** String

### Worksheet.BackgroundImage property {#backgroundimage}

Gets and sets worksheet background image.

**Type:** byte[]

### Worksheet.ConditionalFormattings property {#conditionalformattings}

Gets the ConditionalFormattings in the worksheet.

**Type:** ConditionalFormattingCollection

### Worksheet.ActiveCell property {#activecell}

Gets or sets the active cell in the worksheet.

**Type:** String

### Worksheet.CustomProperties property {#customproperties}

Gets an object representing the identifier information associated with a worksheet. Worksheet.CustomProperties provide a preferred mechanism for storing arbitrary data. It supports legacy third-party document components, as well as those situations that have a stringent need for binary parts.

**Type:** CustomPropertyCollection

### Worksheet.SmartTagSetting property {#smarttagsetting}

Gets all SmartTagCollection objects of the worksheet.

**Type:** SmartTagSetting

### Worksheet.Scenarios property {#scenarios}

Gets the collection of Scenario .

**Type:** ScenarioCollection

### Worksheet.CellWatches property {#cellwatches}

Gets collection of cells on this worksheet being watched in the 'watch window'.

**Type:** CellWatchCollection

### protect(type) (1 of 2) {#protect}

Protects worksheet.

This method protects worksheet without password. It can protect worksheet in all versions of Excel file.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | A ProtectionType value. Protection type. |

---

### protect(type, password, oldPassword) (2 of 2) {#protect-1}

Protects worksheet.

This method can protect worksheet in all versions of Excel file.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | A ProtectionType value. Protection type. |
| password | String | Password. |
| oldPassword | String | If the worksheet is already protected by a password, please supply the old password. Otherwise, you can set a null value or blank string to this parameter. |

**Example:**

```php
//Instantiating a Workbook object
$workbook = new cells\Workbook("Book1.xls");
//Accessing the first worksheet in the Excel file
$worksheet = $workbook->getWorksheets()->get(0);
//Protecting the worksheet with a password
$worksheet->protect(cells\ProtectionType::ALL, "aspose", null);
```

### unprotect() (1 of 2) {#unprotect}

Unprotects worksheet.

This method unprotects worksheet which is protected without password.

---

### unprotect(password) (2 of 2) {#unprotect-1}

Unprotects worksheet.

If the worksheet is protected without a password, you can set a null value or blank string to password parameter.

| Parameter | Type | Description |
| --- | --- | --- |
| password | String | Password |

### moveTo(index) {#moveto}

Moves the sheet to another location in the spreadsheet.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | Destination sheet index. |

### replace(oldString, newString) {#replace}

Replaces all cells' text with a new string.

| Parameter | Type | Description |
| --- | --- | --- |
| oldString | String | Old string value. |
| newString | String | New string value. |

### getSelectedRanges() {#getselectedranges}

Gets selected ranges of cells in the designer spreadsheet.

**Returns:** An java.util.ArrayList which contains selected ranges.

### getSelectedAreas() {#getselectedareas}

### getPrintingPageBreaks(options) {#getprintingpagebreaks}

Gets automatic page breaks.

Each cell area represents a paper.

| Parameter | Type | Description |
| --- | --- | --- |
| options | ImageOrPrintOptions | The print options |

**Returns:** The automatic page breaks areas.

### toString() {#tostring}

Returns a string represents the current Worksheet object.

### startAccessCache(opts) {#startaccesscache}

Starts the session that uses caches to access the data in this worksheet.

After finishing the access to the data, closeAccessCache(int) should be invoked with same options to clear all caches and recover normal access mode.

| Parameter | Type | Description |
| --- | --- | --- |
| opts | Number | A AccessCacheOptions value. options of data access |

### closeAccessCache(opts) {#closeaccesscache}

Closes the session that uses caches to access the data in this worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| opts | Number | A AccessCacheOptions value. options of data access |

### convertFormulaReferenceStyle(formula, toR1C1, baseCellRow, baseCellColumn) {#convertformulareferencestyle}

Converts the formula reference style.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The formula to be converted. |
| toR1C1 | boolean | Which reference style to convert the formula to. If the original formula is of A1 reference style, then this value should be true so the formula will be converted from A1 to R1C1 reference style; If the original formula is of R1C1 reference style, then this value should be false so the formula will be converted from R1C1 to A1 reference style; |
| baseCellRow | Number | The row index of the base cell. |
| baseCellColumn | Number | The column index of the base cell. |

**Returns:** The converted formula.

### calculateFormula(formula) (1 of 4) {#calculateformula}

Calculates a formula.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | Formula to be calculated. |

**Returns:** Calculated formula result.

---

### calculateFormula(formula, opts) (2 of 4) {#calculateformula-1}

Calculates a formula expression directly.

The formula will be calculated just like it has been set to cell A1. And the formula will be taken as normal formula. If you need the formula be calculated as an array formula and to get an array for the calculated result, please use calculateArrayFormula(java.lang.String, com.aspose.cells.CalculationOptions) instead.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | Formula to be calculated. |
| opts | CalculationOptions | Options for calculating formula |

**Returns:** Calculated result of given formula. The returned object may be of possible types of Cell.Value , or ReferredArea.

---

### calculateFormula(formula, pOpts, cOpts, baseCellRow, baseCellColumn, calculationData) (3 of 4) {#calculateformula-2}

Calculates a formula expression directly.

The formula will be calculated just like it has been set to the specified base cell. And the formula will be taken as normal formula. If you need the formula be calculated as an array formula and to get an array for the calculated result, please use calculateArrayFormula(java.lang.String, com.aspose.cells.FormulaParseOptions, com.aspose.cells.CalculationOptions, int, int, int, int, com.aspose.cells.CalculationData) instead.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | Formula to be calculated. |
| pOpts | FormulaParseOptions | Options for parsing formula. |
| cOpts | CalculationOptions | Options for calculating formula. |
| baseCellRow | Number | The row index of the base cell. |
| baseCellColumn | Number | The column index of the base cell. |
| calculationData | CalculationData | The calculation data. It is used for the situation that user needs to calculate some static formulas when implementing custom calculation engine. For such kind of situation, user needs to specify it with the calculation data provided for #Error Cref: M:Aspose.Cells.AbstractCalculationEngine.Calculate(Aspose.Cells.CalculationData) . |

**Returns:** Calculated result of given formula. The returned object may be of possible types of Cell.Value , or ReferredArea.

---

### calculateFormula(options, recursive) (4 of 4) {#calculateformula-3}

Calculates all formulas in this worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| options | CalculationOptions | Options for calculation |
| recursive | boolean | True means if the worksheet' cells depend on the cells of other worksheets, the dependent cells in other worksheets will be calculated too. False means all the formulas in the worksheet have been calculated and the values are right. |

### calculateArrayFormula(formula, opts) (1 of 3) {#calculatearrayformula}

Calculates a formula as array formula.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | Formula to be calculated. |
| opts | CalculationOptions | Options for calculating formula |

---

### calculateArrayFormula(formula, opts, maxRowCount, maxColumnCount) (2 of 3) {#calculatearrayformula-1}

Calculates a formula as array formula.

The formula will be taken as dynamic array formula to calculate the dimension and result. User specified maximum dimension is used for cases that the calculated result is large data set (for example, the calculated result may correspond to a whole row or column data) but user does not need so large an array according to business requirement or for performance consideration.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | Formula to be calculated. |
| opts | CalculationOptions | Options for calculating formula |
| maxRowCount | Number | the maximum row count of resultant data. If it is non-positive or greater than the actual row count, then actual row count will be used. |
| maxColumnCount | Number | the maximum column count of resultant data. If it is non-positive or greater than the actual row count, then actual column count will be used. |

**Returns:** Calculated formula result.

---

### calculateArrayFormula(formula, pOpts, cOpts, baseCellRow, baseCellColumn, maxRowCount, maxColumnCount, calculationData) (3 of 3) {#calculatearrayformula-2}

Calculates a formula as array formula.

The formula will be taken as dynamic array formula to calculate the dimension and result. User specified maximum dimension is used for cases that the calculated result is large data set (for example, the calculated result may correspond to a whole row or column data) but user does not need so large an array according to business requirement or for performance consideration.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | Formula to be calculated. |
| pOpts | FormulaParseOptions | Options for parsing formula |
| cOpts | CalculationOptions | Options for calculating formula |
| baseCellRow | Number | The row index of the base cell. |
| baseCellColumn | Number | The column index of the base cell. |
| maxRowCount | Number | The maximum row count of resultant data. If it is non-positive or greater than the actual row count, then actual row count will be used. |
| maxColumnCount | Number | The maximum column count of resultant data. If it is non-positive or greater than the actual row count, then actual column count will be used. |
| calculationData | CalculationData | The calculation data. It is used for the situation that user needs to calculate some static formulas when implementing custom calculation engine. For such kind of situation, user needs to specify it with the calculation data provided for #Error Cref: M:Aspose.Cells.AbstractCalculationEngine.Calculate(Aspose.Cells.CalculationData) . |

**Returns:** Calculated formula result.

### xmlMapQuery(path, xmlMap) {#xmlmapquery}

Query cell areas that mapped/linked to the specific path of xml map.

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | xml element path |
| xmlMap | XmlMap | Specify an xml map if you want to query for the specific path within a specific map |

**Returns:** CellArea list that mapped/linked to the specific path of xml map, an empty list is returned if nothing is mapped/linked.

### refreshPivotTables() (1 of 2) {#refreshpivottables}

Refreshes all the PivotTables in this Worksheet.

---

### refreshPivotTables(option) (2 of 2) {#refreshpivottables-1}

Refreshes all the PivotTables in this Worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| option | PivotTableRefreshOption | The option for refreshing data source of pivot table. |

### dispose() {#dispose}

Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources.

### getPanes() {#getpanes}

Gets the window panes.

If the window is not split or frozen.

### freezePanes(row, column, freezedRows, freezedColumns) (1 of 2) {#freezepanes}

Freezes panes at the specified cell in the worksheet.

Row index and column index cannot all be zero. Number of rows and number of columns also cannot all be zero. The first two parameters specify the froze position and the last two parameters specify the area frozen on the left top pane.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index. |
| column | Number | Column index. |
| freezedRows | Number | Number of visible rows in top pane, no more than row index. |
| freezedColumns | Number | Number of visible columns in left pane, no more than column index. |

---

### freezePanes(cellName, freezedRows, freezedColumns) (2 of 2) {#freezepanes-1}

Freezes panes at the specified cell in the worksheet.

Row index and column index cannot all be zero. Number of rows and number of columns also cannot all be zero.

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Cell name. |
| freezedRows | Number | Number of visible rows in top pane, no more than row index. |
| freezedColumns | Number | Number of visible columns in left pane, no more than column index. |

### getFreezedPanes() {#getfreezedpanes}

Gets the freeze panes.

**Returns:** Return null means the worksheet is not frozen 0:Row index;1:column;2:freezedRows;3:freezedRows

### split() {#split}

Splits window.

### unFreezePanes() {#unfreezepanes}

Unfreezes panes in the worksheet.

### removeSplit() {#removesplit}

Removes split window.

### addPageBreaks(cellName) {#addpagebreaks}

Adds page break.

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String |  |

### copy(sourceSheet) (1 of 2) {#copy}

Copies contents and formats from another worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceSheet | Worksheet | Source worksheet. |

---

### copy(sourceSheet, copyOptions) (2 of 2) {#copy-1}

Copies contents and formats from another worksheet.

You can copy data from another worksheet in the same file or another file. However, this method does not support to copy drawing objects, such as comments, images and charts.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceSheet | Worksheet | Source worksheet. |
| copyOptions | CopyOptions |  |

### autoFitColumn(columnIndex, firstRow, lastRow) (1 of 2) {#autofitcolumn}

Autofits the column width.

This method autofits a row based on content in a range of cells within the row.

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Number | Column index. |
| firstRow | Number | First row index. |
| lastRow | Number | Last row index. |

---

### autoFitColumn(columnIndex) (2 of 2) {#autofitcolumn-1}

Autofits the column width.

AutoFitColumn is an imprecise function.

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Number | Column index. |

### autoFitColumns() (1 of 6) {#autofitcolumns}

Autofits all columns in this worksheet.

---

### autoFitColumns(options) (2 of 6) {#autofitcolumns-1}

Autofits all columns in this worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| options | AutoFitterOptions | The auto fitting options |

---

### autoFitColumns(firstColumn, lastColumn) (3 of 6) {#autofitcolumns-2}

Autofits the columns width.

AutoFitColumn is an imprecise function.

| Parameter | Type | Description |
| --- | --- | --- |
| firstColumn | Number | First column index. |
| lastColumn | Number | Last column index. |

---

### autoFitColumns(firstColumn, lastColumn, options) (4 of 6) {#autofitcolumns-3}

Autofits the columns width.

AutoFitColumn is an imprecise function.

| Parameter | Type | Description |
| --- | --- | --- |
| firstColumn | Number | First column index. |
| lastColumn | Number | Last column index. |
| options | AutoFitterOptions | The auto fitting options |

---

### autoFitColumns(firstRow, firstColumn, lastRow, lastColumn) (5 of 6) {#autofitcolumns-4}

Autofits the columns width.

AutoFitColumn is an imprecise function.

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Number | First row index. |
| firstColumn | Number | First column index. |
| lastRow | Number | Last row index. |
| lastColumn | Number | Last column index. |

---

### autoFitColumns(firstRow, firstColumn, lastRow, lastColumn, options) (6 of 6) {#autofitcolumns-5}

Autofits the columns width.

AutoFitColumn is an imprecise function.

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Number | First row index. |
| firstColumn | Number | First column index. |
| lastRow | Number | Last row index. |
| lastColumn | Number | Last column index. |
| options | AutoFitterOptions | The auto fitting options |

### autoFitRow(rowIndex, firstColumn, lastColumn) (1 of 4) {#autofitrow}

Autofits the row height.

This method autofits a row based on content in a range of cells within the row.

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Number | Row index. |
| firstColumn | Number | First column index. |
| lastColumn | Number | Last column index. |

---

### autoFitRow(rowIndex, firstColumn, lastColumn, options) (2 of 4) {#autofitrow-1}

Autofits the row height.

This method autofits a row based on content in a range of cells within the row.

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Number | Row index. |
| firstColumn | Number | First column index. |
| lastColumn | Number | Last column index. |
| options | AutoFitterOptions | The auto fitter options |

---

### autoFitRow(startRow, endRow, startColumn, endColumn) (3 of 4) {#autofitrow-2}

Autofits row height in a rectangle range.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Number | Start row index. |
| endRow | Number | End row index. |
| startColumn | Number | Start column index. |
| endColumn | Number | End column index. |

---

### autoFitRow(rowIndex) (4 of 4) {#autofitrow-3}

Autofits the row height.

AutoFitRow is an imprecise function.

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Number | Row index. |

### autoFitRows() (1 of 5) {#autofitrows}

Autofits all rows in this worksheet.

---

### autoFitRows(onlyAuto) (2 of 5) {#autofitrows-1}

Autofits all rows in this worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| onlyAuto | boolean | True,only autofits the row height when row height is not customed. |

---

### autoFitRows(options) (3 of 5) {#autofitrows-2}

Autofits all rows in this worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| options | AutoFitterOptions | The auto fitter options |

---

### autoFitRows(startRow, endRow) (4 of 5) {#autofitrows-3}

Autofits row height in a range.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Number | Start row index. |
| endRow | Number | End row index. |

---

### autoFitRows(startRow, endRow, options) (5 of 5) {#autofitrows-4}

Autofits row height in a range.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Number | Start row index. |
| endRow | Number | End row index. |
| options | AutoFitterOptions | The options of auto fitter. |

### filter(ca) {#filter}

### getAdvancedFilter() {#getadvancedfilter}

Gets the settings of advanced filter.

### advancedFilter(isFilter, listRange, criteriaRange, copyTo, uniqueRecordOnly) {#advancedfilter}

Filters data using complex criteria.

| Parameter | Type | Description |
| --- | --- | --- |
| isFilter | boolean | Indicates whether filtering the list in place. |
| listRange | String | The list range. |
| criteriaRange | String | The criteria range. |
| copyTo | String | The range where copying data to. |
| uniqueRecordOnly | boolean | Only displaying or copying unique rows. |

### removeAutoFilter() {#removeautofilter}

Removes the auto filter of the worksheet.

### setVisible(isVisible, ignoreError) {#setvisible}

Sets the visible options.

| Parameter | Type | Description |
| --- | --- | --- |
| isVisible | boolean | Whether the worksheet is visible |
| ignoreError | boolean | Whether to ignore error if this option is not valid. |

### selectRange(startRow, startColumn, totalRows, totalColumns, removeOthers) {#selectrange}

Selects a range.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Number | The start row. |
| startColumn | Number | The start column |
| totalRows | Number | The number of rows. |
| totalColumns | Number | The number of columns |
| removeOthers | boolean | True means removing other selected range and only select this range. |

### removeAllDrawingObjects() {#removealldrawingobjects}

Removes all drawing objects in this worksheet.

### clearComments() {#clearcomments}

Clears all comments in designer spreadsheet.

### getAllPictures() {#getallpictures}
