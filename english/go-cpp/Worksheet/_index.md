---
title: Worksheet Class 
linktitle: Worksheet
second_title: Aspose.Cells for Go via C++ API Reference
description: 'Worksheet class. Encapsulates the object that represents worksheet in Go.'
type: docs
weight: 200
url: /go-cpp/worksheet/
---

## Worksheet class

Encapsulates the object that represents a single worksheet.

```go

type Worksheet struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |

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
|[GetCells](./getcells/) | Gets the Cells collection. | 
|[GetQueryTables](./getquerytables/) | Gets QueryTableCollection in the worksheet. | 
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
|[FreezePanes_Int_Int_Int_Int](./freezepanes_int_int_int_int/) | Freezes panes at the specified cell in the worksheet. | 
|[GetFreezedPanes](./getfreezedpanes/) | Gets the freeze panes. | 
|[Split](./split/) | Splits window. | 
|[FreezePanes_String_Int_Int](./freezepanes_string_int_int/) | Freezes panes at the specified cell in the worksheet. | 
|[UnFreezePanes](./unfreezepanes/) | Unfreezes panes in the worksheet. | 
|[RemoveSplit](./removesplit/) | Removes split window. | 
|[GetPivotTables](./getpivottables/) | Gets all pivot tables in this worksheet. | 
|[GetListObjects](./getlistobjects/) | Gets all ListObjects in this worksheet. | 
|[GetTabId](./gettabid/) | Specifies the internal identifier for the sheet. | 
|[SetTabId](./settabid/) | Specifies the internal identifier for the sheet. | 
|[GetHorizontalPageBreaks](./gethorizontalpagebreaks/) | Gets the HorizontalPageBreakCollection collection. | 
|[GetVerticalPageBreaks](./getverticalpagebreaks/) | Gets the VerticalPageBreakCollection collection. | 
|[AddPageBreaks](./addpagebreaks/) | Adds page break. | 
|[GetHyperlinks](./gethyperlinks/) | Gets the HyperlinkCollection collection. | 
|[Copy_Worksheet](./copy_worksheet/) | Copies contents and formats from another worksheet. | 
|[Copy_Worksheet_CopyOptions](./copy_worksheet_copyoptions/) | Copies contents and formats from another worksheet. | 
|[AutoFitColumn_Int_Int_Int](./autofitcolumn_int_int_int/) | Autofits the column width. | 
|[AutoFitColumns](./autofitcolumns/) | Autofits all columns in this worksheet. | 
|[AutoFitColumns_AutoFitterOptions](./autofitcolumns_autofitteroptions/) | Autofits all columns in this worksheet. | 
|[AutoFitColumn_Int](./autofitcolumn_int/) | Autofits the column width. | 
|[AutoFitColumns_Int_Int](./autofitcolumns_int_int/) | Autofits the columns width. | 
|[AutoFitColumns_Int_Int_AutoFitterOptions](./autofitcolumns_int_int_autofitteroptions/) | Autofits the columns width. | 
|[AutoFitColumns_Int_Int_Int_Int](./autofitcolumns_int_int_int_int/) | Autofits the columns width. | 
|[AutoFitColumns_Int_Int_Int_Int_AutoFitterOptions](./autofitcolumns_int_int_int_int_autofitteroptions/) | Autofits the columns width. | 
|[AutoFitRow_Int_Int_Int](./autofitrow_int_int_int/) | Autofits the row height. | 
|[AutoFitRow_Int_Int_Int_AutoFitterOptions](./autofitrow_int_int_int_autofitteroptions/) | Autofits the row height. | 
|[AutoFitRows](./autofitrows/) | Autofits all rows in this worksheet. | 
|[AutoFitRows_Bool](./autofitrows_bool/) | Autofits all rows in this worksheet. | 
|[AutoFitRows_AutoFitterOptions](./autofitrows_autofitteroptions/) | Autofits all rows in this worksheet. | 
|[AutoFitRows_Int_Int](./autofitrows_int_int/) | Autofits row height in a range. | 
|[AutoFitRows_Int_Int_AutoFitterOptions](./autofitrows_int_int_autofitteroptions/) | Autofits row height in a range. | 
|[AutoFitRow_Int_Int_Int_Int](./autofitrow_int_int_int_int/) | Autofits row height in a rectangle range. | 
|[AutoFitRow_Int](./autofitrow_int/) | Autofits the row height. | 
|[GetPageSetup](./getpagesetup/) | Represents the page setup description in this sheet. | 
|[GetAutoFilter](./getautofilter/) | Represents auto filter for the specified worksheet. | 
|[Filter](./filter/) | Filters the range. | 
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
|[GetCharts](./getcharts/) | Gets a Chart collection | 
|[GetComments](./getcomments/) | Gets the Comment collection. | 
|[GetPictures](./getpictures/) | Gets a Picture collection. | 
|[GetTextBoxes](./gettextboxes/) | Gets a TextBox collection. | 
|[GetCheckBoxes](./getcheckboxes/) | Gets a CheckBox collection. | 
|[GetOleObjects](./getoleobjects/) | Represents a collection of OleObject in a worksheet. | 
|[GetShapes](./getshapes/) | Returns all drawing shapes in this worksheet. | 
|[GetSlicers](./getslicers/) | Get the Slicer collection in the worksheet | 
|[GetTimelines](./gettimelines/) | Get the Timeline collection in the worksheet | 
|[Protect_ProtectionType](./protect_protectiontype/) | Protects worksheet. | 
|[Protect_ProtectionType_String_String](./protect_protectiontype_string_string/) | Protects worksheet. | 
|[Unprotect](./unprotect/) | Unprotects worksheet. | 
|[Unprotect_String](./unprotect_string/) | Unprotects worksheet. | 
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
|[GetSelectedAreas](./getselectedareas/) | Gets selected ranges of cells in the designer spreadsheet. | 
|[GetTabColor](./gettabcolor/) | Represents worksheet tab color. | 
|[SetTabColor](./settabcolor/) | Represents worksheet tab color. | 
|[GetGridlineColor](./getgridlinecolor/) | Gets and sets the color of gridline | 
|[SetGridlineColor](./setgridlinecolor/) | Gets and sets the color of gridline | 
|[GetCodeName](./getcodename/) | Gets worksheet code name. | 
|[SetCodeName](./setcodename/) | Gets worksheet code name. | 
|[GetBackgroundImage](./getbackgroundimage/) | Gets and sets worksheet background image. | 
|[SetBackgroundImage](./setbackgroundimage/) | Gets and sets worksheet background image. | 
|[GetConditionalFormattings](./getconditionalformattings/) | Gets the ConditionalFormattings in the worksheet. | 
|[GetActiveCell](./getactivecell/) | Gets or sets the active cell in the worksheet. | 
|[SetActiveCell](./setactivecell/) | Gets or sets the active cell in the worksheet. | 
|[GetCustomProperties](./getcustomproperties/) | Gets an object representingthe identifier information associated with a worksheet. | 
|[GetPrintingPageBreaks](./getprintingpagebreaks/) | Gets automatic page breaks. | 
|[GetSmartTagSetting](./getsmarttagsetting/) | Gets all SmartTagCollection objects of the worksheet. | 
|[ToString](./tostring/) | Returns a string represents the current Worksheet object. | 
|[GetScenarios](./getscenarios/) | Gets the collection of Scenario. | 
|[StartAccessCache](./startaccesscache/) | Starts the session that uses caches to access the data in this worksheet. | 
|[CloseAccessCache](./closeaccesscache/) | Closes the session that uses caches to access the data in this worksheet. | 
|[ConvertFormulaReferenceStyle](./convertformulareferencestyle/) | Converts the formula reference style. | 
|[CalculateFormula_String](./calculateformula_string/) | Calculates a formula. | 
|[CalculateFormula_String_CalculationOptions](./calculateformula_string_calculationoptions/) | Calculates a formula expression directly. | 
|[CalculateFormula_String_FormulaParseOptions_CalculationOptions_Int_Int_CalculationData](./calculateformula_string_formulaparseoptions_calculationoptions_int_int_calculationdata/) | Calculates a formula expression directly. | 
|[CalculateArrayFormula_String_CalculationOptions](./calculatearrayformula_string_calculationoptions/) | Calculates a formula as array formula. | 
|[CalculateArrayFormula_String_CalculationOptions_Int_Int](./calculatearrayformula_string_calculationoptions_int_int/) | Calculates a formula as array formula. | 
|[CalculateArrayFormula_String_FormulaParseOptions_CalculationOptions_Int_Int_Int_Int_CalculationData](./calculatearrayformula_string_formulaparseoptions_calculationoptions_int_int_int_int_calculationdata/) | Calculates a formula as array formula. | 
|[CalculateFormula_CalculationOptions_Bool](./calculateformula_calculationoptions_bool/) | Calculates all formulas in this worksheet. | 
|[GetCellWatches](./getcellwatches/) | Gets collection of cells on this worksheet being watched in the 'watch window'. | 
|[RefreshPivotTables](./refreshpivottables/) | Refreshes all the PivotTables in this Worksheet. | 
|[RefreshPivotTables_PivotTableRefreshOption](./refreshpivottables_pivottablerefreshoption/) | Refreshes all the PivotTables in this Worksheet. | 
