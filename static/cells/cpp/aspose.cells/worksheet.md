##Aspose::Cells::Worksheet class
'Aspose::Cells::Worksheet class. Encapsulates the object that represents a single worksheet in C++.'
## Worksheet class
Encapsulates the object that represents a single worksheet.
```cpp
class Worksheet
```
## Methods
| Method | Description |
| --- | --- |
| [AddPageBreaks(const U16String\& cellName)](./addpagebreaks/) | Adds page break. |
| [AddPageBreaks(const char16_t* cellName)](./addpagebreaks/) | Adds page break. |
| [Advanced_Filter(bool isFilter, const U16String\& listRange, const U16String\& criteriaRange, const U16String\& copyTo, bool uniqueRecordOnly)](./advanced_filter/) | Filters data using complex criteria. |
| [Advanced_Filter(bool isFilter, const char16_t* listRange, const char16_t* criteriaRange, const char16_t* copyTo, bool uniqueRecordOnly)](./advanced_filter/) | Filters data using complex criteria. |
| [AutoFitColumn(int32_t columnIndex, int32_t firstRow, int32_t lastRow)](./autofitcolumn/) | Autofits the column width. |
| [AutoFitColumn(int32_t columnIndex)](./autofitcolumn/) | Autofits the column width. |
| [AutoFitColumns()](./autofitcolumns/) | Autofits all columns in this worksheet. |
| [AutoFitColumns(const AutoFitterOptions\& options)](./autofitcolumns/) | Autofits all columns in this worksheet. |
| [AutoFitColumns(int32_t firstColumn, int32_t lastColumn)](./autofitcolumns/) | Autofits the columns width. |
| [AutoFitColumns(int32_t firstColumn, int32_t lastColumn, const AutoFitterOptions\& options)](./autofitcolumns/) | Autofits the columns width. |
| [AutoFitColumns(int32_t firstRow, int32_t firstColumn, int32_t lastRow, int32_t lastColumn)](./autofitcolumns/) | Autofits the columns width. |
| [AutoFitColumns(int32_t firstRow, int32_t firstColumn, int32_t lastRow, int32_t lastColumn, const AutoFitterOptions\& options)](./autofitcolumns/) | Autofits the columns width. |
| [AutoFitRow(int32_t rowIndex, int32_t firstColumn, int32_t lastColumn)](./autofitrow/) | Autofits the row height. |
| [AutoFitRow(int32_t rowIndex, int32_t firstColumn, int32_t lastColumn, const AutoFitterOptions\& options)](./autofitrow/) | Autofits the row height. |
| [AutoFitRow(int32_t startRow, int32_t endRow, int32_t startColumn, int32_t endColumn)](./autofitrow/) | Autofits row height in a rectangle range. |
| [AutoFitRow(int32_t rowIndex)](./autofitrow/) | Autofits the row height. |
| [AutoFitRows()](./autofitrows/) | Autofits all rows in this worksheet. |
| [AutoFitRows(bool onlyAuto)](./autofitrows/) | Autofits all rows in this worksheet. |
| [AutoFitRows(const AutoFitterOptions\& options)](./autofitrows/) | Autofits all rows in this worksheet. |
| [AutoFitRows(int32_t startRow, int32_t endRow)](./autofitrows/) | Autofits row height in a range. |
| [AutoFitRows(int32_t startRow, int32_t endRow, const AutoFitterOptions\& options)](./autofitrows/) | Autofits row height in a range. |
| [CalculateArrayFormula(const U16String\& formula, const CalculationOptions\& opts)](./calculatearrayformula/) | Calculates a formula as array formula. |
| [CalculateArrayFormula(const char16_t* formula, const CalculationOptions\& opts)](./calculatearrayformula/) | Calculates a formula as array formula. |
| [CalculateArrayFormula(const U16String\& formula, const CalculationOptions\& opts, int32_t maxRowCount, int32_t maxColumnCount)](./calculatearrayformula/) | Calculates a formula as array formula. |
| [CalculateArrayFormula(const char16_t* formula, const CalculationOptions\& opts, int32_t maxRowCount, int32_t maxColumnCount)](./calculatearrayformula/) | Calculates a formula as array formula. |
| [CalculateArrayFormula(const U16String\& formula, const FormulaParseOptions\& pOpts, const CalculationOptions\& cOpts, int32_t baseCellRow, int32_t baseCellColumn, int32_t maxRowCount, int32_t maxColumnCount, const CalculationData\& calculationData)](./calculatearrayformula/) | Calculates a formula as array formula. |
| [CalculateArrayFormula(const char16_t* formula, const FormulaParseOptions\& pOpts, const CalculationOptions\& cOpts, int32_t baseCellRow, int32_t baseCellColumn, int32_t maxRowCount, int32_t maxColumnCount, const CalculationData\& calculationData)](./calculatearrayformula/) | Calculates a formula as array formula. |
| [CalculateFormula(const U16String\& formula)](./calculateformula/) | Calculates a formula. |
| [CalculateFormula(const char16_t* formula)](./calculateformula/) | Calculates a formula. |
| [CalculateFormula(const U16String\& formula, const CalculationOptions\& opts)](./calculateformula/) | Calculates a formula expression directly. |
| [CalculateFormula(const char16_t* formula, const CalculationOptions\& opts)](./calculateformula/) | Calculates a formula expression directly. |
| [CalculateFormula(const U16String\& formula, const FormulaParseOptions\& pOpts, const CalculationOptions\& cOpts, int32_t baseCellRow, int32_t baseCellColumn, const CalculationData\& calculationData)](./calculateformula/) | Calculates a formula expression directly. |
| [CalculateFormula(const char16_t* formula, const FormulaParseOptions\& pOpts, const CalculationOptions\& cOpts, int32_t baseCellRow, int32_t baseCellColumn, const CalculationData\& calculationData)](./calculateformula/) | Calculates a formula expression directly. |
| [CalculateFormula(const CalculationOptions\& options, bool recursive)](./calculateformula/) | Calculates all formulas in this worksheet. |
| [ClearComments()](./clearcomments/) | Clears all comments in designer spreadsheet. |
| [CloseAccessCache(AccessCacheOptions opts)](./closeaccesscache/) | Closes the session that uses caches to access the data in this worksheet. |
| [ConvertFormulaReferenceStyle(const U16String\& formula, bool toR1C1, int32_t baseCellRow, int32_t baseCellColumn)](./convertformulareferencestyle/) | Converts the formula reference style. |
| [ConvertFormulaReferenceStyle(const char16_t* formula, bool toR1C1, int32_t baseCellRow, int32_t baseCellColumn)](./convertformulareferencestyle/) | Converts the formula reference style. |
| [Copy(const Worksheet\& sourceSheet)](./copy/) | Copies contents and formats from another worksheet. |
| [Copy(const Worksheet\& sourceSheet, const CopyOptions\& copyOptions)](./copy/) | Copies contents and formats from another worksheet. |
| [Dispose()](./dispose/) | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [FreezePanes(int32_t row, int32_t column, int32_t freezedRows, int32_t freezedColumns)](./freezepanes/) | Freezes panes at the specified cell in the worksheet. |
| [FreezePanes(const U16String\& cellName, int32_t freezedRows, int32_t freezedColumns)](./freezepanes/) | Freezes panes at the specified cell in the worksheet. |
| [FreezePanes(const char16_t* cellName, int32_t freezedRows, int32_t freezedColumns)](./freezepanes/) | Freezes panes at the specified cell in the worksheet. |
| [GetActiveCell()](./getactivecell/) | Gets or sets the active cell in the worksheet. |
| [GetAdvancedFilter()](./getadvancedfilter/) | Gets the settings of advanced filter. |
| [GetAllowEditRanges()](./getalloweditranges/) | Gets the allow edit range collection in the worksheet. |
| [GetAutoFilter()](./getautofilter/) | Represents auto filter for the specified worksheet. |
| [GetBackgroundImage()](./getbackgroundimage/) | Gets and sets worksheet background image. |
| [GetCells()](./getcells/) | Gets the [Cells](../cells/) collection. |
| [GetCellWatches()](./getcellwatches/) | Gets collection of cells on this worksheet being watched in the 'watch window'. |
| [GetCharts()](./getcharts/) | Gets a Chart collection. |
| [GetCheckBoxes()](./getcheckboxes/) | Gets a CheckBox collection. |
| [GetCodeName()](./getcodename/) | Gets worksheet code name. |
| [GetComments()](./getcomments/) | Gets the [Comment](../comment/) collection. |
| [GetConditionalFormattings()](./getconditionalformattings/) | Gets the ConditionalFormattings in the worksheet. |
| [GetCustomProperties()](./getcustomproperties/) | Gets an object representing the identifier information associated with a worksheet. |
| [GetDisplayRightToLeft()](./getdisplayrighttoleft/) | Indicates if the specified worksheet is displayed from right to left instead of from left to right. Default is false. |
| [GetDisplayZeros()](./getdisplayzeros/) | True if zero values are displayed. |
| [GetErrorCheckOptions()](./geterrorcheckoptions/) | Gets error check setting applied on certain ranges. |
| [GetFirstVisibleColumn()](./getfirstvisiblecolumn/) | Represents first visible column index. |
| [GetFirstVisibleRow()](./getfirstvisiblerow/) | Represents first visible row index. |
| [GetFreezedPanes(int32_t\& row, int32_t\& column, int32_t\& freezedRows, int32_t\& freezedColumns)](./getfreezedpanes/) | Gets the freeze panes. |
| [GetGridlineColor()](./getgridlinecolor/) | Gets and sets the color of gridline. |
| [GetHasAutofilter()](./gethasautofilter/) | Indicates whether this worksheet has auto filter. |
| [GetHorizontalPageBreaks()](./gethorizontalpagebreaks/) | Gets the [HorizontalPageBreakCollection](../horizontalpagebreakcollection/) collection. |
| [GetHyperlinks()](./gethyperlinks/) | Gets the [HyperlinkCollection](../hyperlinkcollection/) collection. |
| [GetIndex()](./getindex/) | Gets the index of sheet in the worksheet collection. |
| [GetListObjects()](./getlistobjects/) | Gets all ListObjects in this worksheet. |
| [GetName()](./getname/) | Gets or sets the name of the worksheet. |
| [GetOleObjects()](./getoleobjects/) | Represents a collection of OleObject in a worksheet. |
| [GetOutline()](./getoutline/) | Gets the outline on this worksheet. |
| [GetPageSetup()](./getpagesetup/) | Represents the page setup description in this sheet. |
| [GetPanes()](./getpanes/) | Gets the window panes. |
| [GetPaneState()](./getpanestate/) | Indicates whether the pane has horizontal or vertical splits, and whether those splits are frozen. |
| [GetPictures()](./getpictures/) | Gets a Picture collection. |
| [GetPivotTables()](./getpivottables/) | Gets all pivot tables in this worksheet. |
| [GetPrintingPageBreaks(const ImageOrPrintOptions\& options)](./getprintingpagebreaks/) | Gets automatic page breaks. |
| [GetProtection()](./getprotection/) | Represents the various types of protection options available for a worksheet. Supports advanced protection options in ExcelXP and above version. |
| [GetQueryTables()](./getquerytables/) | Gets [QueryTableCollection](../querytablecollection/) in the worksheet. |
| [GetScenarios()](./getscenarios/) | Gets the collection of [Scenario](../scenario/). |
| [GetSelectedAreas()](./getselectedareas/) | Gets selected ranges of cells in the designer spreadsheet. |
| [GetShapes()](./getshapes/) | Returns all drawing shapes in this worksheet. |
| [GetShowFormulas()](./getshowformulas/) | Indicates whether to show formulas or their results. |
| [GetSlicers()](./getslicers/) | Get the Slicer collection in the worksheet. |
| [GetSmartTagSetting()](./getsmarttagsetting/) | Gets all SmartTagCollection objects of the worksheet. |
| [GetSparklineGroups()](./getsparklinegroups/) | Gets the sparkline groups in the worksheet. |
| [GetTabColor()](./gettabcolor/) | Represents worksheet tab color. |
| [GetTabId()](./gettabid/) | Specifies the internal identifier for the sheet. |
| [GetTextBoxes()](./gettextboxes/) | Gets a TextBox collection. |
| [GetTimelines()](./gettimelines/) | Get the Timeline collection in the worksheet. |
| [GetTransitionEntry()](./gettransitionentry/) | Indicates whether the Transition Formula Entry (Lotus compatibility) option is enabled. |
| [GetTransitionEvaluation()](./gettransitionevaluation/) | Indicates whether the Transition Formula Evaluation (Lotus compatibility) option is enabled. |
| [GetType()](./gettype/) | Represents worksheet type. |
| [GetUniqueId()](./getuniqueid/) | Gets and sets the unique id, it is same as {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. |
| [GetValidations()](./getvalidations/) | Gets the data validation setting collection in the worksheet. |
| [GetVerticalPageBreaks()](./getverticalpagebreaks/) | Gets the [VerticalPageBreakCollection](../verticalpagebreakcollection/) collection. |
| [GetViewType()](./getviewtype/) | Gets and sets the view type. |
| [GetVisibilityType()](./getvisibilitytype/) | Indicates the visible state for this sheet. |
| [GetWorkbook()](./getworkbook/) | Gets the workbook object which contains this sheet. |
| [GetZoom()](./getzoom/) | Represents the scaling factor in percentage. It should be between 10 and 400. |
| [IsGridlinesVisible()](./isgridlinesvisible/) | Gets or sets a value indicating whether the gridlines are visible.Default is true. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsOutlineShown()](./isoutlineshown/) | Indicates whether to show outline. |
| [IsPageBreakPreview()](./ispagebreakpreview/) | Indicates whether the specified worksheet is shown in normal view or page break preview. |
| [IsProtected()](./isprotected/) | Indicates if the worksheet is protected. |
| [IsRowColumnHeadersVisible()](./isrowcolumnheadersvisible/) | Gets or sets a value indicating whether the worksheet will display row and column headers. Default is true. |
| [IsRulerVisible()](./isrulervisible/) | Indicates whether the ruler is visible. This property is only applied for page break preview. |
| [IsSelected()](./isselected/) | Indicates whether this worksheet is selected when the workbook is opened. |
| [IsVisible()](./isvisible/) | Represents if the worksheet is visible. |
| [MoveTo(int32_t index)](./moveto/) | Moves the sheet to another location in the spreadsheet. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const Worksheet\& src)](./operator_asm/) | operator= |
| [Protect(ProtectionType type)](./protect/) | Protects worksheet. |
| [Protect(ProtectionType type, const U16String\& password, const U16String\& oldPassword)](./protect/) | Protects worksheet. |
| [Protect(ProtectionType type, const char16_t* password, const char16_t* oldPassword)](./protect/) | Protects worksheet. |
| [RefreshPivotTables()](./refreshpivottables/) | Refreshes all the PivotTables in this [Worksheet](./). |
| [RefreshPivotTables(const PivotTableRefreshOption\& option)](./refreshpivottables/) | Refreshes all the PivotTables in this [Worksheet](./). |
| [RemoveAllDrawingObjects()](./removealldrawingobjects/) | Removes all drawing objects in this worksheet. |
| [RemoveAutoFilter()](./removeautofilter/) | Removes the auto filter of the worksheet. |
| [RemoveSplit()](./removesplit/) | Removes split window. |
| [Replace(const U16String\& oldString, const U16String\& newString)](./replace/) | Replaces all cells' text with a new string. |
| [Replace(const char16_t* oldString, const char16_t* newString)](./replace/) | Replaces all cells' text with a new string. |
| [SelectRange(int32_t startRow, int32_t startColumn, int32_t totalRows, int32_t totalColumns, bool removeOthers)](./selectrange/) | Selects a range. |
| [SetActiveCell(const U16String\& value)](./setactivecell/) | Gets or sets the active cell in the worksheet. |
| [SetActiveCell(const char16_t* value)](./setactivecell/) | Gets or sets the active cell in the worksheet. |
| [SetBackgroundImage(const Vector \<uint8_t\>\& value)](./setbackgroundimage/) | Gets and sets worksheet background image. |
| [SetCodeName(const U16String\& value)](./setcodename/) | Gets worksheet code name. |
| [SetCodeName(const char16_t* value)](./setcodename/) | Gets worksheet code name. |
| [SetDisplayRightToLeft(bool value)](./setdisplayrighttoleft/) | Indicates if the specified worksheet is displayed from right to left instead of from left to right. Default is false. |
| [SetDisplayZeros(bool value)](./setdisplayzeros/) | True if zero values are displayed. |
| [SetFirstVisibleColumn(int32_t value)](./setfirstvisiblecolumn/) | Represents first visible column index. |
| [SetFirstVisibleRow(int32_t value)](./setfirstvisiblerow/) | Represents first visible row index. |
| [SetGridlineColor(const Aspose::Cells::Color\& value)](./setgridlinecolor/) | Gets and sets the color of gridline. |
| [SetIsGridlinesVisible(bool value)](./setisgridlinesvisible/) | Gets or sets a value indicating whether the gridlines are visible.Default is true. |
| [SetIsOutlineShown(bool value)](./setisoutlineshown/) | Indicates whether to show outline. |
| [SetIsPageBreakPreview(bool value)](./setispagebreakpreview/) | Indicates whether the specified worksheet is shown in normal view or page break preview. |
| [SetIsRowColumnHeadersVisible(bool value)](./setisrowcolumnheadersvisible/) | Gets or sets a value indicating whether the worksheet will display row and column headers. Default is true. |
| [SetIsRulerVisible(bool value)](./setisrulervisible/) | Indicates whether the ruler is visible. This property is only applied for page break preview. |
| [SetIsSelected(bool value)](./setisselected/) | Indicates whether this worksheet is selected when the workbook is opened. |
| [SetIsVisible(bool value)](./setisvisible/) | Represents if the worksheet is visible. |
| [SetName(const U16String\& value)](./setname/) | Gets or sets the name of the worksheet. |
| [SetName(const char16_t* value)](./setname/) | Gets or sets the name of the worksheet. |
| [SetShowFormulas(bool value)](./setshowformulas/) | Indicates whether to show formulas or their results. |
| [SetTabColor(const Aspose::Cells::Color\& value)](./settabcolor/) | Represents worksheet tab color. |
| [SetTabId(int32_t value)](./settabid/) | Specifies the internal identifier for the sheet. |
| [SetTransitionEntry(bool value)](./settransitionentry/) | Indicates whether the Transition Formula Entry (Lotus compatibility) option is enabled. |
| [SetTransitionEvaluation(bool value)](./settransitionevaluation/) | Indicates whether the Transition Formula Evaluation (Lotus compatibility) option is enabled. |
| [SetType(SheetType value)](./settype/) | Represents worksheet type. |
| [SetUniqueId(const U16String\& value)](./setuniqueid/) | Gets and sets the unique id, it is same as {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. |
| [SetUniqueId(const char16_t* value)](./setuniqueid/) | Gets and sets the unique id, it is same as {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. |
| [SetViewType(ViewType value)](./setviewtype/) | Gets and sets the view type. |
| [SetVisibilityType(VisibilityType value)](./setvisibilitytype/) | Indicates the visible state for this sheet. |
| [SetVisible(bool isVisible, bool ignoreError)](./setvisible/) | Sets the visible options. |
| [SetZoom(int32_t value)](./setzoom/) | Represents the scaling factor in percentage. It should be between 10 and 400. |
| [Split()](./split/) | Splits window. |
| [StartAccessCache(AccessCacheOptions opts)](./startaccesscache/) | Starts the session that uses caches to access the data in this worksheet. |
| [ToString()](./tostring/) | Returns a string represents the current [Worksheet](./) object. |
| [UnFreezePanes()](./unfreezepanes/) | Unfreezes panes in the worksheet. |
| [Unprotect()](./unprotect/) | Unprotects worksheet. |
| [Unprotect(const U16String\& password)](./unprotect/) | Unprotects worksheet. |
| [Unprotect(const char16_t* password)](./unprotect/) | Unprotects worksheet. |
| [Worksheet(Worksheet_Impl* impl)](./worksheet/) | Constructs from an implementation object. |
| [Worksheet(const Worksheet\& src)](./worksheet/) | Copy constructor. |
| [~Worksheet()](./~worksheet/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//The following example shows how to freeze panes and insert hyperlink to worksheet with .Net or VB.
Workbook workbook;
Worksheet sheet = workbook.GetWorksheets().Get(0);
//Freeze panes at "AS40" with 10 rows and 10 columns
sheet.FreezePanes(u"AS40", 10, 10);
//Add a hyperlink in Cell A1
sheet.GetHyperlinks().Add(u"A1", 1, 1, u"http://www.aspose.com");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
