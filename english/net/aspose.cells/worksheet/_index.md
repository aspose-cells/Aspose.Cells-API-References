---
title: Worksheet
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 6480
url: /net/aspose.cells/worksheet/
---
## Worksheet class

Encapsulates the object that represents a single worksheet.

```csharp
public class Worksheet : IDisposable
```

## Properties

| Name | Description |
| --- | --- |
| [ActiveCell](activecell) { get; set; } | Gets or sets the active cell in the worksheet. |
| [AllowEditRanges](alloweditranges) { get; } | Gets the allow edit range collection in the worksheet. |
| [AutoFilter](autofilter) { get; } | Represents auto filter for the specified worksheet. |
| [BackgroundImage](backgroundimage) { get; set; } | Gets and sets worksheet background image. |
| [Cells](cells) { get; } | Gets the [`Cells`](./cells) collection. |
| [CellWatches](cellwatches) { get; } | Gets collection of cells on this worksheet being watched in the 'watch window'. |
| [Charts](charts) { get; } | Gets a [`Chart`](../../aspose.cells.charts/chart) collection |
| [CheckBoxes](checkboxes) { get; } | Gets a [`CheckBox`](../../aspose.cells.drawing/checkbox) collection. |
| [CodeName](codename) { get; set; } | Gets worksheet code name. |
| [Comments](comments) { get; } | Gets the [`Comment`](../comment) collection. |
| [ConditionalFormattings](conditionalformattings) { get; } | Gets the ConditionalFormattings in the worksheet. |
| [CustomProperties](customproperties) { get; } | Gets an object representing the identifier information associated with a worksheet. |
| [DisplayRightToLeft](displayrighttoleft) { get; set; } | Indicates if the specified worksheet is displayed from right to left instead of from left to right. Default is false. |
| [DisplayZeros](displayzeros) { get; set; } | True if zero values are displayed. |
| [ErrorCheckOptions](errorcheckoptions) { get; } | Gets error check setting applied on certain ranges. |
| [FirstVisibleColumn](firstvisiblecolumn) { get; set; } | Represents first visible column index. |
| [FirstVisibleRow](firstvisiblerow) { get; set; } | Represents first visible row index. |
| [HasAutofilter](hasautofilter) { get; } | Indicates whether this worksheet has auto filter. |
| [HorizontalPageBreaks](horizontalpagebreaks) { get; } | Gets the [`HorizontalPageBreakCollection`](../horizontalpagebreakcollection) collection. |
| [Hyperlinks](hyperlinks) { get; } | Gets the [`HyperlinkCollection`](../hyperlinkcollection) collection. |
| [Index](index) { get; } | Gets the index of sheet in the worksheet collection. |
| [IsGridlinesVisible](isgridlinesvisible) { get; set; } | Gets or sets a value indicating whether the gridlines are visible.Default is true. |
| [IsOutlineShown](isoutlineshown) { get; set; } | Indicates whether to show outline. |
| [IsPageBreakPreview](ispagebreakpreview) { get; set; } | Indicates whether the specified worksheet is shown in normal view or page break preview. |
| [IsProtected](isprotected) { get; } | Indicates if the worksheet is protected. |
| [IsRowColumnHeadersVisible](isrowcolumnheadersvisible) { get; set; } | Gets or sets a value indicating whether the worksheet will display row and column headers. Default is true. |
| [IsRulerVisible](isrulervisible) { get; set; } | Indicates whether the ruler is visible. This property is only applied for page break preview. |
| [IsSelected](isselected) { get; set; } | Indicates whether this worksheet is selected when the workbook is opened. |
| [IsVisible](isvisible) { get; set; } | Represents if the worksheet is visible. |
| [ListObjects](listobjects) { get; } | Gets all ListObjects in this worksheet. |
| [Name](name) { get; set; } | Gets or sets the name of the worksheet. |
| [OleObjects](oleobjects) { get; } | Represents a collection of [`OleObject`](../../aspose.cells.drawing/oleobject) in a worksheet. |
| [Outline](outline) { get; } | Gets the outline on this worksheet. |
| [PageSetup](pagesetup) { get; } | Represents the page setup description in this sheet. |
| [PaneState](panestate) { get; } | Indicates whether the pane has horizontal or vertical splits, and whether those splits are frozen. |
| [Pictures](pictures) { get; } | Gets a [`Picture`](../../aspose.cells.drawing/picture) collection. |
| [PivotTables](pivottables) { get; } | Gets all pivot tables in this worksheet. |
| [Protection](protection) { get; } | Represents the various types of protection options available for a worksheet. Supports advanced protection options in ExcelXP and above version. |
| [QueryTables](querytables) { get; } | Gets [`QueryTableCollection`](../querytablecollection) in the worksheet. |
| [Scenarios](scenarios) { get; } | Gets the collection of [`Scenario`](../scenario). |
| [Shapes](shapes) { get; } | Returns all drawing shapes in this worksheet. |
| [ShowFormulas](showformulas) { get; set; } | Indicates whether to show formulas or their results. |
| [Slicers](slicers) { get; } | Get the Slicer collection in the worksheet |
| [SmartTagSetting](smarttagsetting) { get; } | Gets all [`SmartTagCollection`](../../aspose.cells.markup/smarttagcollection) objects of the worksheet. |
| [SparklineGroupCollection](sparklinegroupcollection) { get; } | Gets the sparkline group collection in the worksheet. |
| [TabColor](tabcolor) { get; set; } | Represents worksheet tab color. |
| [TabId](tabid) { get; set; } | Specifies the internal identifier for the sheet. |
| [TextBoxes](textboxes) { get; } | Gets a [`TextBox`](../../aspose.cells.drawing/textbox) collection. |
| [Timelines](timelines) { get; } | Get the Timeline collection in the worksheet |
| [TransitionEntry](transitionentry) { get; set; } | Indicates whether the Transition Formula Entry (Lotus compatibility) option is enabled. |
| [TransitionEvaluation](transitionevaluation) { get; set; } | Indicates whether the Transition Formula Evaluation (Lotus compatibility) option is enabled. |
| [Type](type) { get; set; } | Represents worksheet type. |
| [UniqueId](uniqueid) { get; set; } | Gets and sets the unique id, it is same as {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. |
| [Validations](validations) { get; } | Gets the data validation setting collection in the worksheet. |
| [VerticalPageBreaks](verticalpagebreaks) { get; } | Gets the [`VerticalPageBreakCollection`](../verticalpagebreakcollection) collection. |
| [ViewType](viewtype) { get; set; } | Gets and sets the view type. |
| [VisibilityType](visibilitytype) { get; set; } | Indicates the visible state for this sheet. |
| [Workbook](workbook) { get; } | Gets the workbook object which contains this sheet. |
| [Zoom](zoom) { get; set; } | Represents the scaling factor in percentage. It should be between 10 and 400. |

## Methods

| Name | Description |
| --- | --- |
| [AddPageBreaks](addpagebreaks)(string) | Adds page break. |
| [AdvancedFilter](advancedfilter)(bool, string, string, string, bool) | Filters data using complex criteria. |
| [AutoFitColumn](autofitcolumn)(int) | Autofits the column width. |
| [AutoFitColumn](autofitcolumn)(int, int, int) | Autofits the column width. |
| [AutoFitColumns](autofitcolumns)() | Autofits all columns in this worksheet. |
| [AutoFitColumns](autofitcolumns)(AutoFitterOptions) | Autofits all columns in this worksheet. |
| [AutoFitColumns](autofitcolumns)(int, int) | Autofits the columns width. |
| [AutoFitColumns](autofitcolumns)(int, int, AutoFitterOptions) | Autofits the columns width. |
| [AutoFitColumns](autofitcolumns)(int, int, int, int) | Autofits the columns width. |
| [AutoFitColumns](autofitcolumns)(int, int, int, int, AutoFitterOptions) | Autofits the columns width. |
| [AutoFitRow](autofitrow)(int) | Autofits the row height. |
| [AutoFitRow](autofitrow)(int, int, int) | Autofits the row height. |
| [AutoFitRow](autofitrow)(int, int, int, AutoFitterOptions) | Autofits the row height. |
| [AutoFitRow](autofitrow)(int, int, int, int) | Autofits row height in a rectangle range. |
| [AutoFitRows](autofitrows)() | Autofits all rows in this worksheet. |
| [AutoFitRows](autofitrows)(AutoFitterOptions) | Autofits all rows in this worksheet. |
| [AutoFitRows](autofitrows)(bool) | Autofits all rows in this worksheet. |
| [AutoFitRows](autofitrows)(int, int) | Autofits row height in a range. |
| [AutoFitRows](autofitrows)(int, int, AutoFitterOptions) | Autofits row height in a range. |
| [CalculateFormula](calculateformula)(string) | Calculates a formula. |
| [CalculateFormula](calculateformula)(CalculationOptions, bool) | Calculates all formulas in this worksheet. |
| [CalculateFormula](calculateformula)(string, CalculationOptions) | Calculates a formula. |
| [ClearComments](clearcomments)() | Clears all comments in designer spreadsheet. |
| [CloseAccessCache](closeaccesscache)(AccessCacheOptions) | Closes the session that uses caches to access the data in this worksheet. |
| [Copy](copy)(Worksheet) | Copies contents and formats from another worksheet. |
| [Copy](copy)(Worksheet, CopyOptions) | Copies contents and formats from another worksheet. |
| [Dispose](dispose)() | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [FreezePanes](freezepanes)(string, int, int) | Freezes panes at the specified cell in the worksheet. |
| [FreezePanes](freezepanes)(int, int, int, int) | Freezes panes at the specified cell in the worksheet. |
| [GetFreezedPanes](getfreezedpanes)(out int, out int, out int, out int) | Gets the freeze panes. |
| [GetPanes](getpanes)() | Gets the window panes. |
| [GetPrintingPageBreaks](getprintingpagebreaks)(ImageOrPrintOptions) | Gets automatic page breaks. |
| [GetSelectedRanges](getselectedranges)() | Gets selected ranges of cells in the designer spreadsheet. |
| [MoveTo](moveto)(int) | Moves the sheet to another location in the spreadsheet. |
| [Protect](protect)(ProtectionType) | Protects worksheet. |
| [Protect](protect)(ProtectionType, string, string) | Protects worksheet. |
| [RefreshPivotTables](refreshpivottables)() | Refreshes all the PivotTables in this Worksheet. |
| [RemoveAllDrawingObjects](removealldrawingobjects)() | Removes all drawing objects in this worksheet. |
| [RemoveAutoFilter](removeautofilter)() | Removes the auto filter of the worksheet. |
| [RemoveSplit](removesplit)() | Removes split window. |
| [Replace](replace)(string, string) | Replaces all cells' text with a new string. |
| [SelectRange](selectrange)(int, int, int, int, bool) | Selects a range. |
| [SetVisible](setvisible)(bool, bool) | Sets the visible options. |
| [Split](split)() | Splits window. |
| [StartAccessCache](startaccesscache)(AccessCacheOptions) | Starts the session that uses caches to access the data in this worksheet. |
| override [ToString](tostring)() | Returns a string represents the current Worksheet object. |
| [UnFreezePanes](unfreezepanes)() | Unfreezes panes in the worksheet. |
| [Unprotect](unprotect)() | Unprotects worksheet. |
| [Unprotect](unprotect)(string) | Unprotects worksheet. |
| [XmlMapQuery](xmlmapquery)(string, XmlMap) | Query cell areas that mapped/linked to the specific path of xml map. |

### Examples

```csharp
[C#]

Workbook workbook = new Workbook();

Worksheet sheet = workbook.Worksheets[0];

//Freeze panes at "AS40" with 10 rows and 10 columns
sheet.FreezePanes("AS40", 10, 10);

//Add a hyperlink in Cell A1
sheet.Hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");

[Visual Basic]

Dim workbook as Workbook = new Workbook()

Dim sheet as Worksheet = workbook.Worksheets(0)

'Freeze panes at "AS40" with 10 rows and 10 columns
sheet.FreezePanes("AS40", 10, 10)

'Add a hyperlink in Cell A1
sheet.Hyperlinks.Add("A1", 1, 1, "http://www.aspose.com")
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
