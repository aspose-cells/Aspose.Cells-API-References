---
title: Worksheet Class 
linktitle: Worksheet
second_title: Aspose.Cells for Go API Reference
description: 'Worksheet class. Encapsulates the object that represents worksheet in Go.'
type: docs
weight: 200
url: /go/aspose.cells/worksheet/
---

## Worksheet class

Encapsulates the object that represents a single worksheet.

```go

type Worksheet struct 

worksheet, _ := asposecells.NewWorksheet()

```
## Constructors

| Method | Description |
| --- | --- |
|[NewWorksheet](./newworksheet/) | Constructs from an implementation object. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[Dispose](./dispose/) | Performs application-defined tasks associated with freeing, releasing, orresetting unmanaged resources. | 
|[GetProtection](./getprotection/) | Represents the various types of protection options available for a worksheet. Supports advanced protection options in ExcelXP and above version. | 
|[GetUniqueId](./getuniqueid/) | Gets and sets the unique id, it is same as {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. | 
|[SetUniqueId](./setuniqueid/) | Gets and sets the unique id, it is same as {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. | 
|[GetPanes](./getpanes/) | Gets the window panes. | 
|[GetWorkbook](./getworkbook/) | Gets the workbook object which contains this sheet. | 
|[GetCells](./getcells/) | Gets the <see cref="Cells"/> collection. | 
|[GetQueryTables](./getquerytables/) | Gets <see cref="QueryTableCollection"/> in the worksheet. | 
|[GetPivotTables](./getpivottables/) | Gets all pivot tables in this worksheet. | 
|[GetType](./gettype/) | Represents worksheet type. | 
|[SetType](./settype/) | Represents worksheet type. | 
|[GetName](./getname/) | Gets or sets the name of the worksheet. | 
|[SetName](./setname/) | Gets or sets the name of the worksheet. | 
|[GetShowFormulas](./getshowformulas/) | Indicates whether to show formulas or their results. | 
|[SetShowFormulas](./setshowformulas/) | Indicates whether to show formulas or their results. | 
|[IsGridlinesVisible](./isgridlinesvisible/) | Gets or sets a value indicating whether the gridlines are visible.Default is true. | 
|[SetIsGridlinesVisible](./setisgridlinesvisible/) | Gets or sets a value indicating whether the gridlines are visible.Default is true. | 
|[IsRowColumnHeadersVisible](./isrowcolumnheadersvisible/) | Gets or sets a value indicating whether the worksheet will display row and column headers.Default is true. | 
|[SetIsRowColumnHeadersVisible](./setisrowcolumnheadersvisible/) | Gets or sets a value indicating whether the worksheet will display row and column headers.Default is true. | 
|[GetPaneState](./getpanestate/) | Indicates whether the pane has horizontal or vertical splits, and whether those splits are frozen. | 
|[GetDisplayZeros](./getdisplayzeros/) | True if zero values are displayed. | 
|[SetDisplayZeros](./setdisplayzeros/) | True if zero values are displayed. | 
|[GetDisplayRightToLeft](./getdisplayrighttoleft/) | Indicates if the specified worksheet is displayed from right to left instead of from left to right.Default is false. | 
|[SetDisplayRightToLeft](./setdisplayrighttoleft/) | Indicates if the specified worksheet is displayed from right to left instead of from left to right.Default is false. | 
|[IsOutlineShown](./isoutlineshown/) | Indicates whether to show outline. | 
|[SetIsOutlineShown](./setisoutlineshown/) | Indicates whether to show outline. | 
|[IsSelected](./isselected/) | Indicates whether this worksheet is selected when the workbook is opened. | 
|[SetIsSelected](./setisselected/) | Indicates whether this worksheet is selected when the workbook is opened. | 
|[FreezePanes](./freezepanes/) | Freezes panes at the specified cell in the worksheet. | 
|[GetFreezedPanes](./getfreezedpanes/) | Gets the freeze panes. | 
|[Split](./split/) | Splits window. | 
|[FreezePanes](./freezepanes/) | Freezes panes at the specified cell in the worksheet. | 
|[UnFreezePanes](./unfreezepanes/) | Unfreezes panes in the worksheet. | 
|[RemoveSplit](./removesplit/) | Removes split window. | 
|[GetListObjects](./getlistobjects/) | Gets all ListObjects in this worksheet. | 
|[GetTabId](./gettabid/) | Specifies the internal identifier for the sheet. | 
|[SetTabId](./settabid/) | Specifies the internal identifier for the sheet. | 
|[GetHorizontalPageBreaks](./gethorizontalpagebreaks/) | Gets the <see cref="HorizontalPageBreakCollection"/> collection. | 
|[GetVerticalPageBreaks](./getverticalpagebreaks/) | Gets the <see cref="VerticalPageBreakCollection"/> collection. | 
|[AddPageBreaks](./addpagebreaks/) | Adds page break. | 
|[GetHyperlinks](./gethyperlinks/) | Gets the <see cref="HyperlinkCollection"/> collection. | 
|[Copy](./copy/) | Copies contents and formats from another worksheet. | 
|[Copy](./copy/) | Copies contents and formats from another worksheet. | 
|[AutoFitColumn](./autofitcolumn/) | Autofits the column width. | 
|[AutoFitColumns](./autofitcolumns/) | Autofits all columns in this worksheet. | 
|[AutoFitColumns](./autofitcolumns/) | Autofits all columns in this worksheet. | 
|[AutoFitColumn](./autofitcolumn/) | Autofits the column width. | 
|[AutoFitColumns](./autofitcolumns/) | Autofits the columns width. | 
|[AutoFitColumns](./autofitcolumns/) | Autofits the columns width. | 
|[AutoFitColumns](./autofitcolumns/) | Autofits the columns width. | 
|[AutoFitColumns](./autofitcolumns/) | Autofits the columns width. | 
|[AutoFitRow](./autofitrow/) | Autofits the row height. | 
|[AutoFitRow](./autofitrow/) | Autofits the row height. | 
|[AutoFitRows](./autofitrows/) | Autofits all rows in this worksheet. | 
|[AutoFitRows](./autofitrows/) | Autofits all rows in this worksheet. | 
|[AutoFitRows](./autofitrows/) | Autofits all rows in this worksheet. | 
|[AutoFitRows](./autofitrows/) | Autofits row height in a range. | 
|[AutoFitRows](./autofitrows/) | Autofits row height in a range. | 
|[AutoFitRow](./autofitrow/) | Autofits row height in a rectangle range. | 
|[AutoFitRow](./autofitrow/) | Autofits the row height. | 
|[GetPageSetup](./getpagesetup/) | Represents the page setup description in this sheet. | 
|[GetAutoFilter](./getautofilter/) | Represents auto filter for the specified worksheet. | 
|[GetAdvancedFilter](./getadvancedfilter/) | Gets the settings of advanced filter. | 
|[Advanced_Filter](./advanced_filter/) | Filters data using complex criteria. | 
|[RemoveAutoFilter](./removeautofilter/) | Removes the auto filter of the worksheet. | 
|[GetHasAutofilter](./gethasautofilter/) | Indicates whether this worksheet has auto filter. | 
|[GetTransitionEvaluation](./gettransitionevaluation/) | Indicates whether the Transition Formula Evaluation (Lotus compatibility) option is enabled. | 
|[SetTransitionEvaluation](./settransitionevaluation/) | Indicates whether the Transition Formula Evaluation (Lotus compatibility) option is enabled. | 
|[GetTransitionEntry](./gettransitionentry/) | Indicates whether the Transition Formula Entry (Lotus compatibility) option is enabled. | 
|[SetTransitionEntry](./settransitionentry/) | Indicates whether the Transition Formula Entry (Lotus compatibility) option is enabled. | 
|[GetVisibilityType](./getvisibilitytype/) | Indicates the visible state for this sheet. | 
|[SetVisibilityType](./setvisibilitytype/) | Indicates the visible state for this sheet. | 
|[SetVisible](./setvisible/) | Sets the visible options. | 
|[IsVisible](./isvisible/) | Represents if the worksheet is visible. | 
|[SetIsVisible](./setisvisible/) | Represents if the worksheet is visible. | 
|[SelectRange](./selectrange/) | Selects a range. | 
|[RemoveAllDrawingObjects](./removealldrawingobjects/) | Removes all drawing objects in this worksheet. | 
|[ClearComments](./clearcomments/) | Clears all comments in designer spreadsheet. | 
|[GetSparklineGroups](./getsparklinegroups/) | Gets the sparkline groups in the worksheet. | 
|[GetCharts](./getcharts/) | Gets a <see cref="Chart"/> collection | 
|[GetComments](./getcomments/) | Gets the <see cref="Comment"/> collection. | 
|[GetPictures](./getpictures/) | Gets a <see cref="Picture"/> collection. | 
|[GetTextBoxes](./gettextboxes/) | Gets a <see cref="TextBox"/> collection. | 
|[GetCheckBoxes](./getcheckboxes/) | Gets a <see cref="CheckBox"/> collection. | 
|[GetOleObjects](./getoleobjects/) | Represents a collection of <see cref="OleObject"/> in a worksheet. | 
|[GetShapes](./getshapes/) | Returns all drawing shapes in this worksheet. | 
|[GetSlicers](./getslicers/) | Get the Slicer collection in the worksheet | 
|[GetTimelines](./gettimelines/) | Get the Timeline collection in the worksheet | 
|[Protect](./protect/) | Protects worksheet. | 
|[Protect](./protect/) | Protects worksheet. | 
|[Unprotect](./unprotect/) | Unprotects worksheet. | 
|[Unprotect](./unprotect/) | Unprotects worksheet. | 
|[GetIndex](./getindex/) | Gets the index of sheet in the worksheet collection. | 
|[MoveTo](./moveto/) | Moves the sheet to another location in the spreadsheet. | 
|[IsProtected](./isprotected/) | Indicates if the worksheet is protected. | 
|[GetValidations](./getvalidations/) | Gets the data validation setting collection in the worksheet. | 
|[GetAllowEditRanges](./getalloweditranges/) | Gets the allow edit range collection in the worksheet. | 
|[GetErrorCheckOptions](./geterrorcheckoptions/) | Gets error check setting applied on certain ranges. | 
|[GetOutline](./getoutline/) | Gets the outline on this worksheet. | 
|[GetFirstVisibleRow](./getfirstvisiblerow/) | Represents first visible row index. | 
|[SetFirstVisibleRow](./setfirstvisiblerow/) | Represents first visible row index. | 
|[GetFirstVisibleColumn](./getfirstvisiblecolumn/) | Represents first visible column index. | 
|[SetFirstVisibleColumn](./setfirstvisiblecolumn/) | Represents first visible column index. | 
|[Replace](./replace/) | Replaces all cells' text with a new string. | 
|[GetZoom](./getzoom/) | Represents the scaling factor in percentage. It should be between 10 and 400. | 
|[SetZoom](./setzoom/) | Represents the scaling factor in percentage. It should be between 10 and 400. | 
|[GetViewType](./getviewtype/) | Gets and sets the view type. | 
|[SetViewType](./setviewtype/) | Gets and sets the view type. | 
|[IsPageBreakPreview](./ispagebreakpreview/) | Indicates whether the specified worksheet is shown in normal view or page break preview. | 
|[SetIsPageBreakPreview](./setispagebreakpreview/) | Indicates whether the specified worksheet is shown in normal view or page break preview. | 
|[IsRulerVisible](./isrulervisible/) | Indicates whether the ruler is visible. This property is only applied for page break preview. | 
|[SetIsRulerVisible](./setisrulervisible/) | Indicates whether the ruler is visible. This property is only applied for page break preview. | 
|[GetTabColor](./gettabcolor/) | Represents worksheet tab color. | 
|[SetTabColor](./settabcolor/) | Represents worksheet tab color. | 
|[GetCodeName](./getcodename/) | Gets worksheet code name. | 
|[SetCodeName](./setcodename/) | Gets worksheet code name. | 
|[GetConditionalFormattings](./getconditionalformattings/) | Gets the ConditionalFormattings in the worksheet. | 
|[GetActiveCell](./getactivecell/) | Gets or sets the active cell in the worksheet. | 
|[SetActiveCell](./setactivecell/) | Gets or sets the active cell in the worksheet. | 
|[GetCustomProperties](./getcustomproperties/) | Gets an object representingthe identifier information associated with a worksheet. | 
|[GetSmartTagSetting](./getsmarttagsetting/) | Gets all <see cref="SmartTagCollection"/> objects of the worksheet. | 
|[ToString](./tostring/) | Returns a string represents the current Worksheet object. | 
|[GetScenarios](./getscenarios/) | Gets the collection of <see cref="Scenario"/>. | 
|[StartAccessCache](./startaccesscache/) | Starts the session that uses caches to access the data in this worksheet. | 
|[CloseAccessCache](./closeaccesscache/) | Closes the session that uses caches to access the data in this worksheet. | 
|[ConvertFormulaReferenceStyle](./convertformulareferencestyle/) | Converts the formula reference style. | 
|[CalculateFormula](./calculateformula/) | Calculates a formula. | 
|[CalculateFormula](./calculateformula/) | Calculates a formula expression directly. | 
|[CalculateFormula](./calculateformula/) | Calculates a formula expression directly. | 
|[CalculateFormula](./calculateformula/) | Calculates all formulas in this worksheet. | 
|[GetCellWatches](./getcellwatches/) | Gets collection of cells on this worksheet being watched in the 'watch window'. | 
|[RefreshPivotTables](./refreshpivottables/) | Refreshes all the PivotTables in this Worksheet. | 
|[RefreshPivotTables](./refreshpivottables/) | Refreshes all the PivotTables in this Worksheet. | 
