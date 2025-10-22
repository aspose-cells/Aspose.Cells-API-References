##Worksheet
Encapsulates the object that represents a single worksheet.
## Worksheet class
Encapsulates the object that represents a single worksheet.
```javascript
class Worksheet;
```
### Example
```javascript
const { Workbook } = AsposeCells;
var workbook = new Workbook();
var sheet = workbook.worksheets.get(0);
//Freeze panes at "AS40" with 10 rows and 10 columns
sheet.freezePanes("AS40", 10, 10);
//Add a hyperlink in Cell A1
sheet.hyperlinks.add("A1", 1, 1, "https://www.aspose.com");
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [protection](#protection--)| Protection | Readonly. Represents the various types of protection options available for a worksheet. Supports advanced protection options in ExcelXP and above version. |
| [uniqueId](#uniqueId--)| string | Gets and sets the unique id, it is same as {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. |
| [workbook](#workbook--)| Workbook | Readonly. Gets the workbook object which contains this sheet. |
| [cells](#cells--)| Cells | Readonly. Gets the [Cells](../cells/) collection. |
| [queryTables](#queryTables--)| QueryTableCollection | Readonly. Gets [QueryTableCollection](../querytablecollection/) in the worksheet. |
| [type](#type--)| SheetType | Represents worksheet type. |
| [name](#name--)| string | Gets or sets the name of the worksheet. |
| [showFormulas](#showFormulas--)| boolean | Indicates whether to show formulas or their results. |
| [isGridlinesVisible](#isGridlinesVisible--)| boolean | Gets or sets a value indicating whether the gridlines are visible.Default is true. |
| [isRowColumnHeadersVisible](#isRowColumnHeadersVisible--)| boolean | Gets or sets a value indicating whether the worksheet will display row and column headers. Default is true. |
| [paneState](#paneState--)| PaneStateType | Readonly. Indicates whether the pane has horizontal or vertical splits, and whether those splits are frozen. |
| [displayZeros](#displayZeros--)| boolean | True if zero values are displayed. |
| [displayRightToLeft](#displayRightToLeft--)| boolean | Indicates if the specified worksheet is displayed from right to left instead of from left to right. Default is false. |
| [isOutlineShown](#isOutlineShown--)| boolean | Indicates whether to show outline. |
| [isSelected](#isSelected--)| boolean | Indicates whether this worksheet is selected when the workbook is opened. |
| [pivotTables](#pivotTables--)| PivotTableCollection | Readonly. Gets all pivot tables in this worksheet. |
| [listObjects](#listObjects--)| ListObjectCollection | Readonly. Gets all ListObjects in this worksheet. |
| [tabId](#tabId--)| number | Specifies the internal identifier for the sheet. |
| [horizontalPageBreaks](#horizontalPageBreaks--)| HorizontalPageBreakCollection | Readonly. Gets the [HorizontalPageBreakCollection](../horizontalpagebreakcollection/) collection. |
| [verticalPageBreaks](#verticalPageBreaks--)| VerticalPageBreakCollection | Readonly. Gets the [VerticalPageBreakCollection](../verticalpagebreakcollection/) collection. |
| [hyperlinks](#hyperlinks--)| HyperlinkCollection | Readonly. Gets the [HyperlinkCollection](../hyperlinkcollection/) collection. |
| [pageSetup](#pageSetup--)| PageSetup | Readonly. Represents the page setup description in this sheet. |
| [autoFilter](#autoFilter--)| AutoFilter | Readonly. Represents auto filter for the specified worksheet. |
| [hasAutofilter](#hasAutofilter--)| boolean | Readonly. Indicates whether this worksheet has auto filter. |
| [transitionEvaluation](#transitionEvaluation--)| boolean | Indicates whether the Transition Formula Evaluation (Lotus compatibility) option is enabled. |
| [transitionEntry](#transitionEntry--)| boolean | Indicates whether the Transition Formula Entry (Lotus compatibility) option is enabled. |
| [visibilityType](#visibilityType--)| VisibilityType | Indicates the visible state for this sheet. |
| [isVisible](#isVisible--)| boolean | Represents if the worksheet is visible. |
| [sparklineGroups](#sparklineGroups--)| SparklineGroupCollection | Readonly. Gets the sparkline groups in the worksheet. |
| [charts](#charts--)| ChartCollection | Readonly. Gets a [Chart](../chart/) collection |
| [comments](#comments--)| CommentCollection | Readonly. Gets the [Comment](../comment/) collection. |
| [pictures](#pictures--)| PictureCollection | Readonly. Gets a [Picture](../picture/) collection. |
| [textBoxes](#textBoxes--)| TextBoxCollection | Readonly. Gets a [TextBox](../textbox/) collection. |
| [checkBoxes](#checkBoxes--)| CheckBoxCollection | Readonly. Gets a [CheckBox](../checkbox/) collection. |
| [oleObjects](#oleObjects--)| OleObjectCollection | Readonly. Represents a collection of [OleObject](../oleobject/) in a worksheet. |
| [shapes](#shapes--)| ShapeCollection | Readonly. Returns all drawing shapes in this worksheet. |
| [slicers](#slicers--)| SlicerCollection | Readonly. Get the Slicer collection in the worksheet |
| [timelines](#timelines--)| TimelineCollection | Readonly. Get the Timeline collection in the worksheet |
| [index](#index--)| number | Readonly. Gets the index of sheet in the worksheet collection. |
| [isProtected](#isProtected--)| boolean | Readonly. Indicates if the worksheet is protected. |
| [validations](#validations--)| ValidationCollection | Readonly. Gets the data validation setting collection in the worksheet. |
| [allowEditRanges](#allowEditRanges--)| ProtectedRangeCollection | Readonly. Gets the allow edit range collection in the worksheet. |
| [errorCheckOptions](#errorCheckOptions--)| ErrorCheckOptionCollection | Readonly. Gets error check setting applied on certain ranges. |
| [outline](#outline--)| Outline | Readonly. Gets the outline on this worksheet. |
| [firstVisibleRow](#firstVisibleRow--)| number | Represents first visible row index. |
| [firstVisibleColumn](#firstVisibleColumn--)| number | Represents first visible column index. |
| [zoom](#zoom--)| number | Represents the scaling factor in percentage. It should be between 10 and 400. |
| [viewType](#viewType--)| ViewType | Gets and sets the view type. |
| [isPageBreakPreview](#isPageBreakPreview--)| boolean | Indicates whether the specified worksheet is shown in normal view or page break preview. |
| [isRulerVisible](#isRulerVisible--)| boolean | Indicates whether the ruler is visible. This property is only applied for page break preview. |
| [tabColor](#tabColor--)| Color | Represents worksheet tab color. |
| [gridlineColor](#gridlineColor--)| Color | Gets and sets the color of gridline |
| [codeName](#codeName--)| string | Gets worksheet code name. |
| [backgroundImage](#backgroundImage--)| Uint8Array | Gets and sets worksheet background image. |
| [conditionalFormattings](#conditionalFormattings--)| ConditionalFormattingCollection | Readonly. Gets the ConditionalFormattings in the worksheet. |
| [activeCell](#activeCell--)| string | Gets or sets the active cell in the worksheet. |
| [customProperties](#customProperties--)| CustomPropertyCollection | Readonly. Gets an object representing the identifier information associated with a worksheet. |
| [smartTagSetting](#smartTagSetting--)| SmartTagSetting | Readonly. Gets all [SmartTagCollection](../smarttagcollection/) objects of the worksheet. |
| [scenarios](#scenarios--)| ScenarioCollection | Readonly. Gets the collection of [Scenario](../scenario/). |
| [cellWatches](#cellWatches--)| CellWatchCollection | Readonly. Gets collection of cells on this worksheet being watched in the 'watch window'. |
## Methods
| Method | Description |
| --- | --- |
| [dispose()](#dispose--)| Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [getPanes()](#getPanes--)| Gets the window panes. |
| [freezePanes(number, number, number, number)](#freezePanes-number-number-number-number-)| Freezes panes at the specified cell in the worksheet. |
| [freezePanes(string, number, number)](#freezePanes-string-number-number-)| Freezes panes at the specified cell in the worksheet. |
| [getFreezedPanes()](#getFreezedPanes--)| Gets the freeze panes. |
| [split()](#split--)| Splits window. |
| [unFreezePanes()](#unFreezePanes--)| Unfreezes panes in the worksheet. |
| [removeSplit()](#removeSplit--)| Removes split window. |
| [addPageBreaks(string)](#addPageBreaks-string-)| Adds page break. |
| [copy(Worksheet)](#copy-worksheet-)| Copies contents and formats from another worksheet. |
| [copy(Worksheet, CopyOptions)](#copy-worksheet-copyoptions-)| Copies contents and formats from another worksheet. |
| [autoFitColumnAsync(number, number, number)](#autoFitColumnAsync-number-number-number-)| Autofits the column width. |
| [autoFitColumnAsync(number)](#autoFitColumnAsync-number-)| Autofits the column width. |
| [autoFitColumn(number, number, number)](#autoFitColumn-number-number-number-)| Autofits the column width. |
| [autoFitColumn(number)](#autoFitColumn-number-)| Autofits the column width. |
| [autoFitColumnsAsync()](#autoFitColumnsAsync--)| Autofits all columns in this worksheet. |
| [autoFitColumnsAsync(AutoFitterOptions)](#autoFitColumnsAsync-autofitteroptions-)| Autofits all columns in this worksheet. |
| [autoFitColumnsAsync(number, number)](#autoFitColumnsAsync-number-number-)| Autofits the columns width. |
| [autoFitColumnsAsync(number, number, AutoFitterOptions)](#autoFitColumnsAsync-number-number-autofitteroptions-)| Autofits the columns width. |
| [autoFitColumnsAsync(number, number, number, number)](#autoFitColumnsAsync-number-number-number-number-)| Autofits the columns width. |
| [autoFitColumnsAsync(number, number, number, number, AutoFitterOptions)](#autoFitColumnsAsync-number-number-number-number-autofitteroptions-)| Autofits the columns width. |
| [autoFitColumns()](#autoFitColumns--)| Autofits all columns in this worksheet. |
| [autoFitColumns(AutoFitterOptions)](#autoFitColumns-autofitteroptions-)| Autofits all columns in this worksheet. |
| [autoFitColumns(number, number)](#autoFitColumns-number-number-)| Autofits the columns width. |
| [autoFitColumns(number, number, AutoFitterOptions)](#autoFitColumns-number-number-autofitteroptions-)| Autofits the columns width. |
| [autoFitColumns(number, number, number, number)](#autoFitColumns-number-number-number-number-)| Autofits the columns width. |
| [autoFitColumns(number, number, number, number, AutoFitterOptions)](#autoFitColumns-number-number-number-number-autofitteroptions-)| Autofits the columns width. |
| [autoFitRowAsync(number, number, number)](#autoFitRowAsync-number-number-number-)| Autofits the row height. |
| [autoFitRowAsync(number, number, number, AutoFitterOptions)](#autoFitRowAsync-number-number-number-autofitteroptions-)| Autofits the row height. |
| [autoFitRowAsync(number, number, number, number)](#autoFitRowAsync-number-number-number-number-)| Autofits row height in a rectangle range. |
| [autoFitRowAsync(number)](#autoFitRowAsync-number-)| Autofits the row height. |
| [autoFitRow(number, number, number)](#autoFitRow-number-number-number-)| Autofits the row height. |
| [autoFitRow(number, number, number, AutoFitterOptions)](#autoFitRow-number-number-number-autofitteroptions-)| Autofits the row height. |
| [autoFitRow(number, number, number, number)](#autoFitRow-number-number-number-number-)| Autofits row height in a rectangle range. |
| [autoFitRow(number)](#autoFitRow-number-)| Autofits the row height. |
| [autoFitRowsAsync()](#autoFitRowsAsync--)| Autofits all rows in this worksheet. |
| [autoFitRowsAsync(boolean)](#autoFitRowsAsync-boolean-)| Autofits all rows in this worksheet. |
| [autoFitRowsAsync(AutoFitterOptions)](#autoFitRowsAsync-autofitteroptions-)| Autofits all rows in this worksheet. |
| [autoFitRowsAsync(number, number)](#autoFitRowsAsync-number-number-)| Autofits row height in a range. |
| [autoFitRowsAsync(number, number, AutoFitterOptions)](#autoFitRowsAsync-number-number-autofitteroptions-)| Autofits row height in a range. |
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
| [getSelectedAreas()](#getSelectedAreas--)| Gets selected ranges of cells in the designer spreadsheet. |
| [getPrintingPageBreaks(ImageOrPrintOptions)](#getPrintingPageBreaks-imageorprintoptions-)| Gets automatic page breaks. |
| [startAccessCache(AccessCacheOptions)](#startAccessCache-accesscacheoptions-)| Starts the session that uses caches to access the data in this worksheet. |
| [closeAccessCache(AccessCacheOptions)](#closeAccessCache-accesscacheoptions-)| Closes the session that uses caches to access the data in this worksheet. |
| [convertFormulaReferenceStyle(string, boolean, number, number)](#convertFormulaReferenceStyle-string-boolean-number-number-)| Converts the formula reference style. |
| [calculateFormulaAsync(string)](#calculateFormulaAsync-string-)| Calculates a formula. |
| [calculateFormulaAsync(string, CalculationOptions)](#calculateFormulaAsync-string-calculationoptions-)| Calculates a formula expression directly. |
| [calculateFormulaAsync(string, FormulaParseOptions, CalculationOptions, number, number, CalculationData)](#calculateFormulaAsync-string-formulaparseoptions-calculationoptions-number-number-calculationdata-)| Calculates a formula expression directly. |
| [calculateFormulaAsync(CalculationOptions, boolean)](#calculateFormulaAsync-calculationoptions-boolean-)| Calculates all formulas in this worksheet. |
| [calculateFormula(string)](#calculateFormula-string-)| Calculates a formula. |
| [calculateFormula(string, CalculationOptions)](#calculateFormula-string-calculationoptions-)| Calculates a formula expression directly. |
| [calculateFormula(string, FormulaParseOptions, CalculationOptions, number, number, CalculationData)](#calculateFormula-string-formulaparseoptions-calculationoptions-number-number-calculationdata-)| Calculates a formula expression directly. |
| [calculateFormula(CalculationOptions, boolean)](#calculateFormula-calculationoptions-boolean-)| Calculates all formulas in this worksheet. |
| [calculateArrayFormulaAsync(string, CalculationOptions)](#calculateArrayFormulaAsync-string-calculationoptions-)| Calculates a formula as array formula. |
| [calculateArrayFormulaAsync(string, CalculationOptions, number, number)](#calculateArrayFormulaAsync-string-calculationoptions-number-number-)| Calculates a formula as array formula. |
| [calculateArrayFormulaAsync(string, FormulaParseOptions, CalculationOptions, number, number, number, number, CalculationData)](#calculateArrayFormulaAsync-string-formulaparseoptions-calculationoptions-number-number-number-number-calculationdata-)| Calculates a formula as array formula. |
| [calculateArrayFormula(string, CalculationOptions)](#calculateArrayFormula-string-calculationoptions-)| Calculates a formula as array formula. |
| [calculateArrayFormula(string, CalculationOptions, number, number)](#calculateArrayFormula-string-calculationoptions-number-number-)| Calculates a formula as array formula. |
| [calculateArrayFormula(string, FormulaParseOptions, CalculationOptions, number, number, number, number, CalculationData)](#calculateArrayFormula-string-formulaparseoptions-calculationoptions-number-number-number-number-calculationdata-)| Calculates a formula as array formula. |
| [refreshPivotTablesAsync()](#refreshPivotTablesAsync--)| Refreshes all the PivotTables in this Worksheet. |
| [refreshPivotTablesAsync(PivotTableRefreshOption)](#refreshPivotTablesAsync-pivottablerefreshoption-)| Refreshes all the PivotTables in this Worksheet. |
| [refreshPivotTables()](#refreshPivotTables--)| Refreshes all the PivotTables in this Worksheet. |
| [refreshPivotTables(PivotTableRefreshOption)](#refreshPivotTables-pivottablerefreshoption-)| Refreshes all the PivotTables in this Worksheet. |
| [toString()](#toString--)| Returns a string represents the current Worksheet object. |
### protection {#protection--}
Readonly. Represents the various types of protection options available for a worksheet. Supports advanced protection options in ExcelXP and above version.
```javascript
protection : Protection;
```
**Remarks**
This property can protect worksheet in all versions of Excel file and support advanced protection options in ExcelXP and above version.
### uniqueId {#uniqueId--}
Gets and sets the unique id, it is same as {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}.
```javascript
uniqueId : string;
```
### workbook {#workbook--}
Readonly. Gets the workbook object which contains this sheet.
```javascript
workbook : Workbook;
```
### cells {#cells--}
Readonly. Gets the [Cells](../cells/) collection.
```javascript
cells : Cells;
```
### queryTables {#queryTables--}
Readonly. Gets [QueryTableCollection](../querytablecollection/) in the worksheet.
```javascript
queryTables : QueryTableCollection;
```
### type {#type--}
Represents worksheet type.
```javascript
type : SheetType;
```
### name {#name--}
Gets or sets the name of the worksheet.
```javascript
name : string;
```
**Remarks**
The max length of sheet name is 31. And you cannot assign same name(case insensitive) to two worksheets. For example, you cannot set "SheetName1" to the first worksheet and set "SHEETNAME1" to the second worksheet.
### showFormulas {#showFormulas--}
Indicates whether to show formulas or their results.
```javascript
showFormulas : boolean;
```
### isGridlinesVisible {#isGridlinesVisible--}
Gets or sets a value indicating whether the gridlines are visible.Default is true.
```javascript
isGridlinesVisible : boolean;
```
### isRowColumnHeadersVisible {#isRowColumnHeadersVisible--}
Gets or sets a value indicating whether the worksheet will display row and column headers. Default is true.
```javascript
isRowColumnHeadersVisible : boolean;
```
### paneState {#paneState--}
Readonly. Indicates whether the pane has horizontal or vertical splits, and whether those splits are frozen.
```javascript
paneState : PaneStateType;
```
### displayZeros {#displayZeros--}
True if zero values are displayed.
```javascript
displayZeros : boolean;
```
### displayRightToLeft {#displayRightToLeft--}
Indicates if the specified worksheet is displayed from right to left instead of from left to right. Default is false.
```javascript
displayRightToLeft : boolean;
```
### isOutlineShown {#isOutlineShown--}
Indicates whether to show outline.
```javascript
isOutlineShown : boolean;
```
### isSelected {#isSelected--}
Indicates whether this worksheet is selected when the workbook is opened.
```javascript
isSelected : boolean;
```
### pivotTables {#pivotTables--}
Readonly. Gets all pivot tables in this worksheet.
```javascript
pivotTables : PivotTableCollection;
```
### listObjects {#listObjects--}
Readonly. Gets all ListObjects in this worksheet.
```javascript
listObjects : ListObjectCollection;
```
### tabId {#tabId--}
Specifies the internal identifier for the sheet.
```javascript
tabId : number;
```
### horizontalPageBreaks {#horizontalPageBreaks--}
Readonly. Gets the [HorizontalPageBreakCollection](../horizontalpagebreakcollection/) collection.
```javascript
horizontalPageBreaks : HorizontalPageBreakCollection;
```
### verticalPageBreaks {#verticalPageBreaks--}
Readonly. Gets the [VerticalPageBreakCollection](../verticalpagebreakcollection/) collection.
```javascript
verticalPageBreaks : VerticalPageBreakCollection;
```
### hyperlinks {#hyperlinks--}
Readonly. Gets the [HyperlinkCollection](../hyperlinkcollection/) collection.
```javascript
hyperlinks : HyperlinkCollection;
```
### pageSetup {#pageSetup--}
Readonly. Represents the page setup description in this sheet.
```javascript
pageSetup : PageSetup;
```
### autoFilter {#autoFilter--}
Readonly. Represents auto filter for the specified worksheet.
```javascript
autoFilter : AutoFilter;
```
### hasAutofilter {#hasAutofilter--}
Readonly. Indicates whether this worksheet has auto filter.
```javascript
hasAutofilter : boolean;
```
### transitionEvaluation {#transitionEvaluation--}
Indicates whether the Transition Formula Evaluation (Lotus compatibility) option is enabled.
```javascript
transitionEvaluation : boolean;
```
### transitionEntry {#transitionEntry--}
Indicates whether the Transition Formula Entry (Lotus compatibility) option is enabled.
```javascript
transitionEntry : boolean;
```
### visibilityType {#visibilityType--}
Indicates the visible state for this sheet.
```javascript
visibilityType : VisibilityType;
```
### isVisible {#isVisible--}
Represents if the worksheet is visible.
```javascript
isVisible : boolean;
```
### sparklineGroups {#sparklineGroups--}
Readonly. Gets the sparkline groups in the worksheet.
```javascript
sparklineGroups : SparklineGroupCollection;
```
### charts {#charts--}
Readonly. Gets a [Chart](../chart/) collection
```javascript
charts : ChartCollection;
```
### comments {#comments--}
Readonly. Gets the [Comment](../comment/) collection.
```javascript
comments : CommentCollection;
```
### pictures {#pictures--}
Readonly. Gets a [Picture](../picture/) collection.
```javascript
pictures : PictureCollection;
```
### textBoxes {#textBoxes--}
Readonly. Gets a [TextBox](../textbox/) collection.
```javascript
textBoxes : TextBoxCollection;
```
### checkBoxes {#checkBoxes--}
Readonly. Gets a [CheckBox](../checkbox/) collection.
```javascript
checkBoxes : CheckBoxCollection;
```
### oleObjects {#oleObjects--}
Readonly. Represents a collection of [OleObject](../oleobject/) in a worksheet.
```javascript
oleObjects : OleObjectCollection;
```
### shapes {#shapes--}
Readonly. Returns all drawing shapes in this worksheet.
```javascript
shapes : ShapeCollection;
```
### slicers {#slicers--}
Readonly. Get the Slicer collection in the worksheet
```javascript
slicers : SlicerCollection;
```
### timelines {#timelines--}
Readonly. Get the Timeline collection in the worksheet
```javascript
timelines : TimelineCollection;
```
### index {#index--}
Readonly. Gets the index of sheet in the worksheet collection.
```javascript
index : number;
```
### isProtected {#isProtected--}
Readonly. Indicates if the worksheet is protected.
```javascript
isProtected : boolean;
```
### validations {#validations--}
Readonly. Gets the data validation setting collection in the worksheet.
```javascript
validations : ValidationCollection;
```
### allowEditRanges {#allowEditRanges--}
Readonly. Gets the allow edit range collection in the worksheet.
```javascript
allowEditRanges : ProtectedRangeCollection;
```
### errorCheckOptions {#errorCheckOptions--}
Readonly. Gets error check setting applied on certain ranges.
```javascript
errorCheckOptions : ErrorCheckOptionCollection;
```
### outline {#outline--}
Readonly. Gets the outline on this worksheet.
```javascript
outline : Outline;
```
### firstVisibleRow {#firstVisibleRow--}
Represents first visible row index.
```javascript
firstVisibleRow : number;
```
### firstVisibleColumn {#firstVisibleColumn--}
Represents first visible column index.
```javascript
firstVisibleColumn : number;
```
### zoom {#zoom--}
Represents the scaling factor in percentage. It should be between 10 and 400.
```javascript
zoom : number;
```
**Remarks**
Please set the view type first.
### viewType {#viewType--}
Gets and sets the view type.
```javascript
viewType : ViewType;
```
### isPageBreakPreview {#isPageBreakPreview--}
Indicates whether the specified worksheet is shown in normal view or page break preview.
```javascript
isPageBreakPreview : boolean;
```
### isRulerVisible {#isRulerVisible--}
Indicates whether the ruler is visible. This property is only applied for page break preview.
```javascript
isRulerVisible : boolean;
```
### tabColor {#tabColor--}
Represents worksheet tab color.
```javascript
tabColor : Color;
```
**Remarks**
This feature is only supported in ExcelXP(Excel2002) and later versions. If you save file as Excel97 or Excel2000 format, it will be omitted.
### gridlineColor {#gridlineColor--}
Gets and sets the color of gridline
```javascript
gridlineColor : Color;
```
### codeName {#codeName--}
Gets worksheet code name.
```javascript
codeName : string;
```
### backgroundImage {#backgroundImage--}
Gets and sets worksheet background image.
```javascript
backgroundImage : Uint8Array;
```
### conditionalFormattings {#conditionalFormattings--}
Readonly. Gets the ConditionalFormattings in the worksheet.
```javascript
conditionalFormattings : ConditionalFormattingCollection;
```
### activeCell {#activeCell--}
Gets or sets the active cell in the worksheet.
```javascript
activeCell : string;
```
### customProperties {#customProperties--}
Readonly. Gets an object representing the identifier information associated with a worksheet.
```javascript
customProperties : CustomPropertyCollection;
```
**Remarks**
Worksheet.CustomProperties provide a preferred mechanism for storing arbitrary data. It supports legacy third-party document components, as well as those situations that have a stringent need for binary parts.
### smartTagSetting {#smartTagSetting--}
Readonly. Gets all [SmartTagCollection](../smarttagcollection/) objects of the worksheet.
```javascript
smartTagSetting : SmartTagSetting;
```
### scenarios {#scenarios--}
Readonly. Gets the collection of [Scenario](../scenario/).
```javascript
scenarios : ScenarioCollection;
```
### cellWatches {#cellWatches--}
Readonly. Gets collection of cells on this worksheet being watched in the 'watch window'.
```javascript
cellWatches : CellWatchCollection;
```
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
[PaneCollection](../panecollection/)
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
Row index and column index cannot all be zero. Number of rows and number of columns also cannot all be zero.</p> <p>The first two parameters specify the froze position and the last two parameters specify the area frozen on the left top pane.
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
### getFreezedPanes() {#getFreezedPanes--}
Gets the freeze panes.
```javascript
getFreezedPanes() : number[];
```
**Returns**
Return null means the worksheet is not frozen 0:Row index;1:column;2:freezedRows;3:freezedRows
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
| sourceSheet | [Worksheet](../worksheet/) | Source worksheet. |
### copy(Worksheet, CopyOptions) {#copy-worksheet-copyoptions-}
Copies contents and formats from another worksheet.
```javascript
copy(sourceSheet: Worksheet, copyOptions: CopyOptions) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceSheet | [Worksheet](../worksheet/) | Source worksheet. |
| copyOptions | [CopyOptions](../copyoptions/) |  |
**Remarks**
You can copy data from another worksheet in the same file or another file. However, this method does not support to copy drawing objects, such as comments, images and charts.
### autoFitColumnAsync(number, number, number) {#autoFitColumnAsync-number-number-number-}
Autofits the column width.
```javascript
autoFitColumnAsync(columnIndex: number, firstRow: number, lastRow: number) : Promise<void>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | number | Column index. |
| firstRow | number | First row index. |
| lastRow | number | Last row index. |
**Returns**
[Promise<void>](../promise<void>/)
**Remarks**
This method autofits a row based on content in a range of cells within the row.
### autoFitColumnAsync(number) {#autoFitColumnAsync-number-}
Autofits the column width.
```javascript
autoFitColumnAsync(columnIndex: number) : Promise<void>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | number | Column index. |
**Returns**
[Promise<void>](../promise<void>/)
**Remarks**
AutoFitColumn is an imprecise function.
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
### autoFitColumnsAsync() {#autoFitColumnsAsync--}
Autofits all columns in this worksheet.
```javascript
autoFitColumnsAsync() : Promise<void>;
```
**Returns**
[Promise<void>](../promise<void>/)
### autoFitColumnsAsync(AutoFitterOptions) {#autoFitColumnsAsync-autofitteroptions-}
Autofits all columns in this worksheet.
```javascript
autoFitColumnsAsync(options: AutoFitterOptions) : Promise<void>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [AutoFitterOptions](../autofitteroptions/) | The auto fitting options |
**Returns**
[Promise<void>](../promise<void>/)
### autoFitColumnsAsync(number, number) {#autoFitColumnsAsync-number-number-}
Autofits the columns width.
```javascript
autoFitColumnsAsync(firstColumn: number, lastColumn: number) : Promise<void>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstColumn | number | First column index. |
| lastColumn | number | Last column index. |
**Returns**
[Promise<void>](../promise<void>/)
**Remarks**
AutoFitColumn is an imprecise function.
### autoFitColumnsAsync(number, number, AutoFitterOptions) {#autoFitColumnsAsync-number-number-autofitteroptions-}
Autofits the columns width.
```javascript
autoFitColumnsAsync(firstColumn: number, lastColumn: number, options: AutoFitterOptions) : Promise<void>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstColumn | number | First column index. |
| lastColumn | number | Last column index. |
| options | [AutoFitterOptions](../autofitteroptions/) | The auto fitting options |
**Returns**
[Promise<void>](../promise<void>/)
**Remarks**
AutoFitColumn is an imprecise function.
### autoFitColumnsAsync(number, number, number, number) {#autoFitColumnsAsync-number-number-number-number-}
Autofits the columns width.
```javascript
autoFitColumnsAsync(firstRow: number, firstColumn: number, lastRow: number, lastColumn: number) : Promise<void>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | number | First row index. |
| firstColumn | number | First column index. |
| lastRow | number | Last row index. |
| lastColumn | number | Last column index. |
**Returns**
[Promise<void>](../promise<void>/)
**Remarks**
AutoFitColumn is an imprecise function.
### autoFitColumnsAsync(number, number, number, number, AutoFitterOptions) {#autoFitColumnsAsync-number-number-number-number-autofitteroptions-}
Autofits the columns width.
```javascript
autoFitColumnsAsync(firstRow: number, firstColumn: number, lastRow: number, lastColumn: number, options: AutoFitterOptions) : Promise<void>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | number | First row index. |
| firstColumn | number | First column index. |
| lastRow | number | Last row index. |
| lastColumn | number | Last column index. |
| options | [AutoFitterOptions](../autofitteroptions/) | The auto fitting options |
**Returns**
[Promise<void>](../promise<void>/)
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
| options | [AutoFitterOptions](../autofitteroptions/) | The auto fitting options |
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
| options | [AutoFitterOptions](../autofitteroptions/) | The auto fitting options |
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
| options | [AutoFitterOptions](../autofitteroptions/) | The auto fitting options |
**Remarks**
AutoFitColumn is an imprecise function.
### autoFitRowAsync(number, number, number) {#autoFitRowAsync-number-number-number-}
Autofits the row height.
```javascript
autoFitRowAsync(rowIndex: number, firstColumn: number, lastColumn: number) : Promise<void>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | number | Row index. |
| firstColumn | number | First column index. |
| lastColumn | number | Last column index. |
**Returns**
[Promise<void>](../promise<void>/)
**Remarks**
This method autofits a row based on content in a range of cells within the row.
### autoFitRowAsync(number, number, number, AutoFitterOptions) {#autoFitRowAsync-number-number-number-autofitteroptions-}
Autofits the row height.
```javascript
autoFitRowAsync(rowIndex: number, firstColumn: number, lastColumn: number, options: AutoFitterOptions) : Promise<void>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | number | Row index. |
| firstColumn | number | First column index. |
| lastColumn | number | Last column index. |
| options | [AutoFitterOptions](../autofitteroptions/) | The auto fitter options |
**Returns**
[Promise<void>](../promise<void>/)
**Remarks**
This method autofits a row based on content in a range of cells within the row.
### autoFitRowAsync(number, number, number, number) {#autoFitRowAsync-number-number-number-number-}
Autofits row height in a rectangle range.
```javascript
autoFitRowAsync(startRow: number, endRow: number, startColumn: number, endColumn: number) : Promise<void>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | number | Start row index. |
| endRow | number | End row index. |
| startColumn | number | Start column index. |
| endColumn | number | End column index. |
**Returns**
[Promise<void>](../promise<void>/)
### autoFitRowAsync(number) {#autoFitRowAsync-number-}
Autofits the row height.
```javascript
autoFitRowAsync(rowIndex: number) : Promise<void>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | number | Row index. |
**Returns**
[Promise<void>](../promise<void>/)
**Remarks**
AutoFitRow is an imprecise function.
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
| options | [AutoFitterOptions](../autofitteroptions/) | The auto fitter options |
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
### autoFitRowsAsync() {#autoFitRowsAsync--}
Autofits all rows in this worksheet.
```javascript
autoFitRowsAsync() : Promise<void>;
```
**Returns**
[Promise<void>](../promise<void>/)
### autoFitRowsAsync(boolean) {#autoFitRowsAsync-boolean-}
Autofits all rows in this worksheet.
```javascript
autoFitRowsAsync(onlyAuto: boolean) : Promise<void>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| onlyAuto | boolean | True,only autofits the row height when row height is not customed. |
**Returns**
[Promise<void>](../promise<void>/)
### autoFitRowsAsync(AutoFitterOptions) {#autoFitRowsAsync-autofitteroptions-}
Autofits all rows in this worksheet.
```javascript
autoFitRowsAsync(options: AutoFitterOptions) : Promise<void>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [AutoFitterOptions](../autofitteroptions/) | The auto fitter options |
**Returns**
[Promise<void>](../promise<void>/)
### autoFitRowsAsync(number, number) {#autoFitRowsAsync-number-number-}
Autofits row height in a range.
```javascript
autoFitRowsAsync(startRow: number, endRow: number) : Promise<void>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | number | Start row index. |
| endRow | number | End row index. |
**Returns**
[Promise<void>](../promise<void>/)
### autoFitRowsAsync(number, number, AutoFitterOptions) {#autoFitRowsAsync-number-number-autofitteroptions-}
Autofits row height in a range.
```javascript
autoFitRowsAsync(startRow: number, endRow: number, options: AutoFitterOptions) : Promise<void>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | number | Start row index. |
| endRow | number | End row index. |
| options | [AutoFitterOptions](../autofitteroptions/) | The options of auto fitter. |
**Returns**
[Promise<void>](../promise<void>/)
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
| options | [AutoFitterOptions](../autofitteroptions/) | The auto fitter options |
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
| options | [AutoFitterOptions](../autofitteroptions/) | The options of auto fitter. |
### getAdvancedFilter() {#getAdvancedFilter--}
Gets the settings of advanced filter.
```javascript
getAdvancedFilter() : AdvancedFilter;
```
**Returns**
[AdvancedFilter](../advancedfilter/)
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
| type | [ProtectionType](../protectiontype/) | Protection type. |
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
| type | [ProtectionType](../protectiontype/) | Protection type. |
| password | string | Password. |
| oldPassword | string | If the worksheet is already protected by a password, please supply the old password. 		/// Otherwise, you can set a null value or blank string to this parameter. |
**Remarks**
This method can protect worksheet in all versions of Excel file.
**Example**
```javascript
const { Workbook, ProtectionType, SaveFormat } = AsposeCells;
//Instantiating a Workbook object
var excel = new Workbook(data);
//Accessing the first worksheet in the Excel file
var worksheet = excel.worksheets.get(0);
//Protecting the worksheet with a password
worksheet.protect(ProtectionType.All, "aspose", null);
//Saving the modified Excel file in default (that is Excel 20003) format
var uint8Array = excel.save(SaveFormat.Xlsx);
```
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
### getSelectedAreas() {#getSelectedAreas--}
Gets selected ranges of cells in the designer spreadsheet.
```javascript
getSelectedAreas() : Range[];
```
**Returns**
Returns all selected ranges.
### getPrintingPageBreaks(ImageOrPrintOptions) {#getPrintingPageBreaks-imageorprintoptions-}
Gets automatic page breaks.
```javascript
getPrintingPageBreaks(options: ImageOrPrintOptions) : CellArea[];
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [ImageOrPrintOptions](../imageorprintoptions/) | The print options |
**Returns**
The automatic page breaks areas.
**Remarks**
Each cell area represents a paper.
### startAccessCache(AccessCacheOptions) {#startAccessCache-accesscacheoptions-}
Starts the session that uses caches to access the data in this worksheet.
```javascript
startAccessCache(opts: AccessCacheOptions) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| opts | [AccessCacheOptions](../accesscacheoptions/) | options of data access |
**Remarks**
After finishing the access to the data, [CloseAccessCache(AccessCacheOptions)](../closeaccesscache(accesscacheoptions)/) should be invoked with same options to clear all caches and recover normal access mode.
### closeAccessCache(AccessCacheOptions) {#closeAccessCache-accesscacheoptions-}
Closes the session that uses caches to access the data in this worksheet.
```javascript
closeAccessCache(opts: AccessCacheOptions) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| opts | [AccessCacheOptions](../accesscacheoptions/) | options of data access |
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
### calculateFormulaAsync(string) {#calculateFormulaAsync-string-}
Calculates a formula.
```javascript
calculateFormulaAsync(formula: string) : Promise<VObject>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | string | Formula to be calculated. |
**Returns**
Calculated formula result.
### calculateFormulaAsync(string, CalculationOptions) {#calculateFormulaAsync-string-calculationoptions-}
Calculates a formula expression directly.
```javascript
calculateFormulaAsync(formula: string, opts: CalculationOptions) : Promise<VObject>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | string | Formula to be calculated. |
| opts | [CalculationOptions](../calculationoptions/) | Options for calculating formula |
**Returns**
Calculated result of given formula. The returned object may be of possible types of [Cell.Value](../cell.value/), or ReferredArea.
**Remarks**
The formula will be calculated just like it has been set to cell A1. And the formula will be taken as normal formula. If you need the formula be calculated as an array formula and to get an array for the calculated result, please use [CalculateArrayFormula(string, CalculationOptions)](../calculatearrayformula(string, calculationoptions)/) instead.
### calculateFormulaAsync(string, FormulaParseOptions, CalculationOptions, number, number, CalculationData) {#calculateFormulaAsync-string-formulaparseoptions-calculationoptions-number-number-calculationdata-}
Calculates a formula expression directly.
```javascript
calculateFormulaAsync(formula: string, pOpts: FormulaParseOptions, cOpts: CalculationOptions, baseCellRow: number, baseCellColumn: number, calculationData: CalculationData) : Promise<VObject>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | string | Formula to be calculated. |
| pOpts | [FormulaParseOptions](../formulaparseoptions/) | Options for parsing formula. |
| cOpts | [CalculationOptions](../calculationoptions/) | Options for calculating formula. |
| baseCellRow | number | The row index of the base cell. |
| baseCellColumn | number | The column index of the base cell. |
| calculationData | [CalculationData](../calculationdata/) | The calculation data. It is used for the situation         /// that user needs to calculate some static formulas when implementing custom calculation engine.         /// For such kind of situation, user needs to specify it with the calculation data provided         /// for [AbstractCalculationEngine.Calculate(CalculationData)](../abstractcalculationengine.calculate(calculationdata)/). |
**Returns**
Calculated result of given formula. The returned object may be of possible types of [Cell.Value](../cell.value/), or ReferredArea.
**Remarks**
The formula will be calculated just like it has been set to the specified base cell. And the formula will be taken as normal formula. If you need the formula be calculated as an array formula and to get an array for the calculated result, please use [CalculateArrayFormula(string, FormulaParseOptions, CalculationOptions, int, int, int, int, CalculationData)](../calculatearrayformula(string, formulaparseoptions, calculationoptions, int, int, int, int, calculationdata)/) instead.
### calculateFormulaAsync(CalculationOptions, boolean) {#calculateFormulaAsync-calculationoptions-boolean-}
Calculates all formulas in this worksheet.
```javascript
calculateFormulaAsync(options: CalculationOptions, recursive: boolean) : Promise<void>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [CalculationOptions](../calculationoptions/) | Options for calculation |
| recursive | boolean | True means if the worksheet' cells depend on the cells of other worksheets,         ///  the dependent cells in other worksheets will be calculated too.         ///  False means all the formulas in the worksheet have been calculated and the values are right. |
**Returns**
[Promise<void>](../promise<void>/)
### calculateFormula(string) {#calculateFormula-string-}
Calculates a formula.
```javascript
calculateFormula(formula: string) : VObject;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | string | Formula to be calculated. |
**Returns**
Calculated formula result.
### calculateFormula(string, CalculationOptions) {#calculateFormula-string-calculationoptions-}
Calculates a formula expression directly.
```javascript
calculateFormula(formula: string, opts: CalculationOptions) : VObject;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | string | Formula to be calculated. |
| opts | [CalculationOptions](../calculationoptions/) | Options for calculating formula |
**Returns**
Calculated result of given formula. The returned object may be of possible types of [Cell.Value](../cell.value/), or ReferredArea.
**Remarks**
The formula will be calculated just like it has been set to cell A1. And the formula will be taken as normal formula. If you need the formula be calculated as an array formula and to get an array for the calculated result, please use [CalculateArrayFormula(string, CalculationOptions)](../calculatearrayformula(string, calculationoptions)/) instead.
### calculateFormula(string, FormulaParseOptions, CalculationOptions, number, number, CalculationData) {#calculateFormula-string-formulaparseoptions-calculationoptions-number-number-calculationdata-}
Calculates a formula expression directly.
```javascript
calculateFormula(formula: string, pOpts: FormulaParseOptions, cOpts: CalculationOptions, baseCellRow: number, baseCellColumn: number, calculationData: CalculationData) : VObject;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | string | Formula to be calculated. |
| pOpts | [FormulaParseOptions](../formulaparseoptions/) | Options for parsing formula. |
| cOpts | [CalculationOptions](../calculationoptions/) | Options for calculating formula. |
| baseCellRow | number | The row index of the base cell. |
| baseCellColumn | number | The column index of the base cell. |
| calculationData | [CalculationData](../calculationdata/) | The calculation data. It is used for the situation         /// that user needs to calculate some static formulas when implementing custom calculation engine.         /// For such kind of situation, user needs to specify it with the calculation data provided         /// for [AbstractCalculationEngine.Calculate(CalculationData)](../abstractcalculationengine.calculate(calculationdata)/). |
**Returns**
Calculated result of given formula. The returned object may be of possible types of [Cell.Value](../cell.value/), or ReferredArea.
**Remarks**
The formula will be calculated just like it has been set to the specified base cell. And the formula will be taken as normal formula. If you need the formula be calculated as an array formula and to get an array for the calculated result, please use [CalculateArrayFormula(string, FormulaParseOptions, CalculationOptions, int, int, int, int, CalculationData)](../calculatearrayformula(string, formulaparseoptions, calculationoptions, int, int, int, int, calculationdata)/) instead.
### calculateFormula(CalculationOptions, boolean) {#calculateFormula-calculationoptions-boolean-}
Calculates all formulas in this worksheet.
```javascript
calculateFormula(options: CalculationOptions, recursive: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [CalculationOptions](../calculationoptions/) | Options for calculation |
| recursive | boolean | True means if the worksheet' cells depend on the cells of other worksheets,         ///  the dependent cells in other worksheets will be calculated too.         ///  False means all the formulas in the worksheet have been calculated and the values are right. |
### calculateArrayFormulaAsync(string, CalculationOptions) {#calculateArrayFormulaAsync-string-calculationoptions-}
Calculates a formula as array formula.
```javascript
calculateArrayFormulaAsync(formula: string, opts: CalculationOptions) : Promise<VObject[][]>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | string | Formula to be calculated. |
| opts | [CalculationOptions](../calculationoptions/) | Options for calculating formula |
**Returns**
[Promise<VObject[][]>](../promise<vobject[][]>/)
### calculateArrayFormulaAsync(string, CalculationOptions, number, number) {#calculateArrayFormulaAsync-string-calculationoptions-number-number-}
Calculates a formula as array formula.
```javascript
calculateArrayFormulaAsync(formula: string, opts: CalculationOptions, maxRowCount: number, maxColumnCount: number) : Promise<VObject[][]>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | string | Formula to be calculated. |
| opts | [CalculationOptions](../calculationoptions/) | Options for calculating formula |
| maxRowCount | number | the maximum row count of resultant data.         /// If it is non-positive or greater than the actual row count, then actual row count will be used. |
| maxColumnCount | number | the maximum column count of resultant data.         /// If it is non-positive or greater than the actual row count, then actual column count will be used. |
**Returns**
Calculated formula result.
**Remarks**
The formula will be taken as dynamic array formula to calculate the dimension and result. User specified maximum dimension is used for cases that the calculated result is large data set (for example, the calculated result may correspond to a whole row or column data) but user does not need so large an array according to business requirement or for performance consideration.
### calculateArrayFormulaAsync(string, FormulaParseOptions, CalculationOptions, number, number, number, number, CalculationData) {#calculateArrayFormulaAsync-string-formulaparseoptions-calculationoptions-number-number-number-number-calculationdata-}
Calculates a formula as array formula.
```javascript
calculateArrayFormulaAsync(formula: string, pOpts: FormulaParseOptions, cOpts: CalculationOptions, baseCellRow: number, baseCellColumn: number, maxRowCount: number, maxColumnCount: number, calculationData: CalculationData) : Promise<VObject[][]>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | string | Formula to be calculated. |
| pOpts | [FormulaParseOptions](../formulaparseoptions/) | Options for parsing formula |
| cOpts | [CalculationOptions](../calculationoptions/) | Options for calculating formula |
| baseCellRow | number | The row index of the base cell. |
| baseCellColumn | number | The column index of the base cell. |
| maxRowCount | number | The maximum row count of resultant data.         /// If it is non-positive or greater than the actual row count, then actual row count will be used. |
| maxColumnCount | number | The maximum column count of resultant data.         /// If it is non-positive or greater than the actual row count, then actual column count will be used. |
| calculationData | [CalculationData](../calculationdata/) | The calculation data. It is used for the situation         /// that user needs to calculate some static formulas when implementing custom calculation engine.         /// For such kind of situation, user needs to specify it with the calculation data provided         /// for [AbstractCalculationEngine.Calculate(CalculationData)](../abstractcalculationengine.calculate(calculationdata)/). |
**Returns**
Calculated formula result.
**Remarks**
The formula will be taken as dynamic array formula to calculate the dimension and result. User specified maximum dimension is used for cases that the calculated result is large data set (for example, the calculated result may correspond to a whole row or column data) but user does not need so large an array according to business requirement or for performance consideration.
### calculateArrayFormula(string, CalculationOptions) {#calculateArrayFormula-string-calculationoptions-}
Calculates a formula as array formula.
```javascript
calculateArrayFormula(formula: string, opts: CalculationOptions) : VObject[][];
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | string | Formula to be calculated. |
| opts | [CalculationOptions](../calculationoptions/) | Options for calculating formula |
**Returns**
[VObject[]](../vobject[]/)[]
### calculateArrayFormula(string, CalculationOptions, number, number) {#calculateArrayFormula-string-calculationoptions-number-number-}
Calculates a formula as array formula.
```javascript
calculateArrayFormula(formula: string, opts: CalculationOptions, maxRowCount: number, maxColumnCount: number) : VObject[][];
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | string | Formula to be calculated. |
| opts | [CalculationOptions](../calculationoptions/) | Options for calculating formula |
| maxRowCount | number | the maximum row count of resultant data.         /// If it is non-positive or greater than the actual row count, then actual row count will be used. |
| maxColumnCount | number | the maximum column count of resultant data.         /// If it is non-positive or greater than the actual row count, then actual column count will be used. |
**Returns**
Calculated formula result.
**Remarks**
The formula will be taken as dynamic array formula to calculate the dimension and result. User specified maximum dimension is used for cases that the calculated result is large data set (for example, the calculated result may correspond to a whole row or column data) but user does not need so large an array according to business requirement or for performance consideration.
### calculateArrayFormula(string, FormulaParseOptions, CalculationOptions, number, number, number, number, CalculationData) {#calculateArrayFormula-string-formulaparseoptions-calculationoptions-number-number-number-number-calculationdata-}
Calculates a formula as array formula.
```javascript
calculateArrayFormula(formula: string, pOpts: FormulaParseOptions, cOpts: CalculationOptions, baseCellRow: number, baseCellColumn: number, maxRowCount: number, maxColumnCount: number, calculationData: CalculationData) : VObject[][];
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | string | Formula to be calculated. |
| pOpts | [FormulaParseOptions](../formulaparseoptions/) | Options for parsing formula |
| cOpts | [CalculationOptions](../calculationoptions/) | Options for calculating formula |
| baseCellRow | number | The row index of the base cell. |
| baseCellColumn | number | The column index of the base cell. |
| maxRowCount | number | The maximum row count of resultant data.         /// If it is non-positive or greater than the actual row count, then actual row count will be used. |
| maxColumnCount | number | The maximum column count of resultant data.         /// If it is non-positive or greater than the actual row count, then actual column count will be used. |
| calculationData | [CalculationData](../calculationdata/) | The calculation data. It is used for the situation         /// that user needs to calculate some static formulas when implementing custom calculation engine.         /// For such kind of situation, user needs to specify it with the calculation data provided         /// for [AbstractCalculationEngine.Calculate(CalculationData)](../abstractcalculationengine.calculate(calculationdata)/). |
**Returns**
Calculated formula result.
**Remarks**
The formula will be taken as dynamic array formula to calculate the dimension and result. User specified maximum dimension is used for cases that the calculated result is large data set (for example, the calculated result may correspond to a whole row or column data) but user does not need so large an array according to business requirement or for performance consideration.
### refreshPivotTablesAsync() {#refreshPivotTablesAsync--}
Refreshes all the PivotTables in this Worksheet.
```javascript
refreshPivotTablesAsync() : Promise<void>;
```
**Returns**
[Promise<void>](../promise<void>/)
### refreshPivotTablesAsync(PivotTableRefreshOption) {#refreshPivotTablesAsync-pivottablerefreshoption-}
Refreshes all the PivotTables in this Worksheet.
```javascript
refreshPivotTablesAsync(option: PivotTableRefreshOption) : Promise<boolean>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../pivottablerefreshoption/) | The option for refreshing data source of pivot table. |
**Returns**
[Promise<boolean>](../promise<boolean>/)
### refreshPivotTables() {#refreshPivotTables--}
Refreshes all the PivotTables in this Worksheet.
```javascript
refreshPivotTables() : void;
```
### refreshPivotTables(PivotTableRefreshOption) {#refreshPivotTables-pivottablerefreshoption-}
Refreshes all the PivotTables in this Worksheet.
```javascript
refreshPivotTables(option: PivotTableRefreshOption) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../pivottablerefreshoption/) | The option for refreshing data source of pivot table. |
### toString() {#toString--}
Returns a string represents the current Worksheet object.
```javascript
toString() : string;
```
