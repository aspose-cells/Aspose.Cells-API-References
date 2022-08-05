---
title: PivotTable
second_title: Aspose.Cells for .NET API Reference
description: Summary description for PivotTable.
type: docs
weight: 4730
url: /net/aspose.cells.pivot/pivottable/
---
## PivotTable class

Summary description for PivotTable.

```csharp
public class PivotTable : IDisposable
```

## Properties

| Name | Description |
| --- | --- |
| [AltTextDescription](../../aspose.cells.pivot/pivottable/alttextdescription) { get; set; } | Gets the description of the alt text |
| [AltTextTitle](../../aspose.cells.pivot/pivottable/alttexttitle) { get; set; } | Gets the title of the altertext |
| [AutoFormatType](../../aspose.cells.pivot/pivottable/autoformattype) { get; set; } | Gets the PivotTable auto format type. |
| [BaseFields](../../aspose.cells.pivot/pivottable/basefields) { get; } | Returns a PivotFields object that includes all fields in the PivotTable report |
| [ColumnFields](../../aspose.cells.pivot/pivottable/columnfields) { get; } | Returns a PivotFields object that are currently shown as column fields. |
| [ColumnGrand](../../aspose.cells.pivot/pivottable/columngrand) { get; set; } | Indicates whether the PivotTable report shows grand totals for columns. |
| [ColumnHeaderCaption](../../aspose.cells.pivot/pivottable/columnheadercaption) { get; set; } | Gets the Column Header Caption of the PivotTable. |
| [ColumnRange](../../aspose.cells.pivot/pivottable/columnrange) { get; } | Returns a CellArea object that represents the range that contains the column area in the PivotTable report. Read-only. |
| [CustomListSort](../../aspose.cells.pivot/pivottable/customlistsort) { get; set; } | Indicates whether consider built-in custom list when sort data |
| [DataBodyRange](../../aspose.cells.pivot/pivottable/databodyrange) { get; } | Returns a CellArea object that represents the range that contains the data area in the list between the header row and the insert row. Read-only. |
| [DataField](../../aspose.cells.pivot/pivottable/datafield) { get; } | Gets a PivotField object that represents all the data fields in a PivotTable. Read-only.It would be init only when there are two or more data fields in the DataPiovtFiels. It only use to add DataPivotField to the PivotTable row/column area . Default is in row area. |
| [DataFields](../../aspose.cells.pivot/pivottable/datafields) { get; } | Gets a PivotField object that represents all the data fields in a PivotTable. Read-only.It would be init only when there are two or more data fields in the DataPiovtFiels. It only use to add DataPivotField to the PivotTable row/column area . Default is in row area. |
| [DataSource](../../aspose.cells.pivot/pivottable/datasource) { get; set; } | Gets and sets the data source of the pivot table. |
| [DisplayErrorString](../../aspose.cells.pivot/pivottable/displayerrorstring) { get; set; } | Indicates whether the PivotTable report displays a custom string in cells that contain errors. |
| [DisplayImmediateItems](../../aspose.cells.pivot/pivottable/displayimmediateitems) { get; set; } | Indicates whether items in the row and column areas are visible when the data area of the PivotTable is empty. The default value is true. |
| [DisplayNullString](../../aspose.cells.pivot/pivottable/displaynullstring) { get; set; } | Indicates whether the PivotTable report displays a custom string in cells that contain null values. |
| [EnableDataValueEditing](../../aspose.cells.pivot/pivottable/enabledatavalueediting) { get; set; } | Specifies a boolean value that indicates whether the user is allowed to edit the cells in the data area of the pivottable. Enable cell editing in the values area |
| [EnableDrilldown](../../aspose.cells.pivot/pivottable/enabledrilldown) { get; set; } | Gets whether drilldown is enabled. |
| [EnableFieldDialog](../../aspose.cells.pivot/pivottable/enablefielddialog) { get; set; } | Indicates whether the PivotTable Field dialog box is available when the user double-clicks the PivotTable field. |
| [EnableFieldList](../../aspose.cells.pivot/pivottable/enablefieldlist) { get; set; } | Gets whether enable the field list for the PivotTable. |
| [EnableWizard](../../aspose.cells.pivot/pivottable/enablewizard) { get; set; } | Indicates whether the PivotTable Wizard is available. |
| [ErrorString](../../aspose.cells.pivot/pivottable/errorstring) { get; set; } | Gets the string displayed in cells that contain errors when the DisplayErrorString property is true.The default value is an empty string. |
| [ExternalConnectionDataSource](../../aspose.cells.pivot/pivottable/externalconnectiondatasource) { get; } | Gets the external connection data source. |
| [FieldListSortAscending](../../aspose.cells.pivot/pivottable/fieldlistsortascending) { get; set; } | Specifies a boolean value that indicates whether fields in the PivotTable are sorted in non-default order in the field list. |
| [GrandTotalName](../../aspose.cells.pivot/pivottable/grandtotalname) { get; set; } | Returns the text string label that is displayed in the grand total column or row heading. The default value is the string "Grand Total". |
| [HasBlankRows](../../aspose.cells.pivot/pivottable/hasblankrows) { get; set; } | Indicates whether to add blank rows. This property only applies for the PivotTable auto format types which needs to add blank rows. |
| [Indent](../../aspose.cells.pivot/pivottable/indent) { get; set; } | Specifies the indentation increment for compact axis and can be used to set the Report Layout to Compact Form. |
| [IsAutoFormat](../../aspose.cells.pivot/pivottable/isautoformat) { get; set; } | Indicates whether the PivotTable report is automatically formatted. Checkbox "autoformat table " which is in pivottable option for Excel 2003 Checkbox "autofit column width on update" which is in pivot table Options :Layout Format for Excel 2007 |
| [IsExcel2003Compatible](../../aspose.cells.pivot/pivottable/isexcel2003compatible) { get; set; } | Specifies whether the PivotTable is compatible for Excel2003 when refreshing PivotTable, if true, a string must be less than or equal to 255 characters, so if the string is greater than 255 characters, it will be truncated. if false, a string will not have the aforementioned restriction. The default value is true. |
| [IsGridDropZones](../../aspose.cells.pivot/pivottable/isgriddropzones) { get; set; } | Indicates whether the PivotTable report displays classic pivottable layout. (enables dragging fields in the grid) |
| [IsMultipleFieldFilters](../../aspose.cells.pivot/pivottable/ismultiplefieldfilters) { get; set; } | Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. |
| [IsSelected](../../aspose.cells.pivot/pivottable/isselected) { get; set; } | Indicates whether the PivotTable is selected. |
| [ItemPrintTitles](../../aspose.cells.pivot/pivottable/itemprinttitles) { get; set; } | A bit that specifies whether pivot item captions on the row axis are repeated on each printed page for pivot fields in tabular form. |
| [ManualUpdate](../../aspose.cells.pivot/pivottable/manualupdate) { get; set; } | Indicates whether the PivotTable report is recalculated only at the user's request. |
| [MergeLabels](../../aspose.cells.pivot/pivottable/mergelabels) { get; set; } | Indicates whether the specified PivotTable report's outer-row item, column item, subtotal, and grand total labels use merged cells. |
| [MissingItemsLimit](../../aspose.cells.pivot/pivottable/missingitemslimit) { get; set; } | Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. |
| [Name](../../aspose.cells.pivot/pivottable/name) { get; set; } | Gets the name of the PivotTable |
| [NullString](../../aspose.cells.pivot/pivottable/nullstring) { get; set; } | Gets the string displayed in cells that contain null values when the DisplayNullString property is true.The default value is an empty string. |
| [PageFieldOrder](../../aspose.cells.pivot/pivottable/pagefieldorder) { get; set; } | Gets the order in which page fields are added to the PivotTable report's layout. |
| [PageFields](../../aspose.cells.pivot/pivottable/pagefields) { get; } | Returns a PivotFields object that are currently shown as page fields. |
| [PageFieldWrapCount](../../aspose.cells.pivot/pivottable/pagefieldwrapcount) { get; set; } | Gets the number of page fields in each column or row in the PivotTable report. |
| [PivotFilters](../../aspose.cells.pivot/pivottable/pivotfilters) { get; } | Returns a PivotFilterCollection object. |
| [PivotFormatConditions](../../aspose.cells.pivot/pivottable/pivotformatconditions) { get; } | Gets the Format Conditions of the pivot table. |
| [PivotTableStyleName](../../aspose.cells.pivot/pivottable/pivottablestylename) { get; set; } | Gets and sets the pivottable style name. |
| [PivotTableStyleType](../../aspose.cells.pivot/pivottable/pivottablestyletype) { get; set; } | Gets and sets the built-in pivot table style. |
| [PreserveFormatting](../../aspose.cells.pivot/pivottable/preserveformatting) { get; set; } | Indicates whether formatting is preserved when the PivotTable is refreshed or recalculated. |
| [PrintDrill](../../aspose.cells.pivot/pivottable/printdrill) { get; set; } | Specifies a boolean value that indicates whether drill indicators should be printed. print expand/collapse buttons when displayed on pivottable. |
| [PrintTitles](../../aspose.cells.pivot/pivottable/printtitles) { get; set; } | Indicates whether the print titles for the worksheet are set based on the PivotTable report. The default value is false. |
| [RefreshDataFlag](../../aspose.cells.pivot/pivottable/refreshdataflag) { get; set; } | Indicates whether Refresh Data or not. |
| [RefreshDataOnOpeningFile](../../aspose.cells.pivot/pivottable/refreshdataonopeningfile) { get; set; } | Indicates whether Refresh Data when Opening File. |
| [RefreshDate](../../aspose.cells.pivot/pivottable/refreshdate) { get; } | Gets the date when the PivotTable was last refreshed. |
| [RefreshedByWho](../../aspose.cells.pivot/pivottable/refreshedbywho) { get; } | Gets the name of the user who last refreshed the PivotTable |
| [RowFields](../../aspose.cells.pivot/pivottable/rowfields) { get; } | Returns a PivotFields object that are currently shown as row fields. |
| [RowGrand](../../aspose.cells.pivot/pivottable/rowgrand) { get; set; } | Indicates whether the PivotTable report shows grand totals for rows. |
| [RowHeaderCaption](../../aspose.cells.pivot/pivottable/rowheadercaption) { get; set; } | Gets the Row Header Caption of the PivotTable. |
| [RowRange](../../aspose.cells.pivot/pivottable/rowrange) { get; } | Returns a CellArea object that represents the range that contains the row area in the PivotTable report. Read-only. |
| [SaveData](../../aspose.cells.pivot/pivottable/savedata) { get; set; } | Indicates whether data for the PivotTable report is saved with the workbook. |
| [ShowDataTips](../../aspose.cells.pivot/pivottable/showdatatips) { get; set; } | Specifies a boolean value that indicates whether tooltips should be displayed for PivotTable data cells. |
| [ShowDrill](../../aspose.cells.pivot/pivottable/showdrill) { get; set; } | Gets whether expand/collapse buttons is shown. |
| [ShowEmptyCol](../../aspose.cells.pivot/pivottable/showemptycol) { get; set; } | Specifies a boolean value that indicates whether to include empty columns in the table |
| [ShowEmptyRow](../../aspose.cells.pivot/pivottable/showemptyrow) { get; set; } | Specifies a boolean value that indicates whether to include empty rows in the table. |
| [ShowMemberPropertyTips](../../aspose.cells.pivot/pivottable/showmemberpropertytips) { get; set; } | Specifies a boolean value that indicates whether member property information should be omitted from PivotTable tooltips. |
| [ShowPivotStyleColumnHeader](../../aspose.cells.pivot/pivottable/showpivotstylecolumnheader) { get; set; } | Indicates whether the column header in the pivot table should have the style applied. |
| [ShowPivotStyleColumnStripes](../../aspose.cells.pivot/pivottable/showpivotstylecolumnstripes) { get; set; } | Indicates whether column stripe formatting is applied. |
| [ShowPivotStyleLastColumn](../../aspose.cells.pivot/pivottable/showpivotstylelastcolumn) { get; set; } | Indicates whether column stripe formatting is applied. |
| [ShowPivotStyleRowHeader](../../aspose.cells.pivot/pivottable/showpivotstylerowheader) { get; set; } | Indicates whether the row header in the pivot table should have the style applied. |
| [ShowPivotStyleRowStripes](../../aspose.cells.pivot/pivottable/showpivotstylerowstripes) { get; set; } | Indicates whether row stripe formatting is applied. |
| [ShowRowHeaderCaption](../../aspose.cells.pivot/pivottable/showrowheadercaption) { get; set; } | Indicates whether row header caption is shown in the PivotTable report Indicates whether Display field captions and filter drop downs |
| [ShowValuesRow](../../aspose.cells.pivot/pivottable/showvaluesrow) { get; set; } | Specifies a boolean value that indicates whether show values row. show the values row |
| [SubtotalHiddenPageItems](../../aspose.cells.pivot/pivottable/subtotalhiddenpageitems) { get; set; } | Indicates whether hidden page field items in the PivotTable report are included in row and column subtotals, block totals, and grand totals. The default value is False. |
| [TableRange1](../../aspose.cells.pivot/pivottable/tablerange1) { get; } | Returns a CellArea object that represents the range containing the entire PivotTable report, but doesn't include page fields. Read-only. |
| [TableRange2](../../aspose.cells.pivot/pivottable/tablerange2) { get; } | Returns a CellArea object that represents the range containing the entire PivotTable report, includes page fields. Read-only. |
| [Tag](../../aspose.cells.pivot/pivottable/tag) { get; set; } | Gets a string saved with the PivotTable report. |

## Methods

| Name | Description |
| --- | --- |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield#addcalculatedfield)(string, string) | Adds a calculated field to pivot field and drag it to data area. |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield#addcalculatedfield_1)(string, string, bool) | Adds a calculated field to pivot field. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea#addfieldtoarea_1)(PivotFieldType, int) | Adds the field to the specific area. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea#addfieldtoarea)(PivotFieldType, PivotField) | Adds the field to the specific area. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea#addfieldtoarea_2)(PivotFieldType, string) | Adds the field to the specific area. |
| [CalculateData](../../aspose.cells.pivot/pivottable/calculatedata)() | Calculates pivottable's data to cells. |
| [CalculateRange](../../aspose.cells.pivot/pivottable/calculaterange)() | Calculates pivottable's range. |
| [ChangeDataSource](../../aspose.cells.pivot/pivottable/changedatasource)(string[]) | Set pivottable's source data. Sheet1!$A$1:$C$3 |
| [ClearData](../../aspose.cells.pivot/pivottable/cleardata)() | Clear PivotTable's data and formatting |
| [CopyStyle](../../aspose.cells.pivot/pivottable/copystyle)(PivotTable) | Copies named style from another pivot table. |
| [Dispose](../../aspose.cells.pivot/pivottable/dispose)() | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [Fields](../../aspose.cells.pivot/pivottable/fields)(PivotFieldType) | Gets the specific fields by the field type. |
| [Format](../../aspose.cells.pivot/pivottable/format)(int, int, Style) | Format the cell in the pivottable area |
| [FormatAll](../../aspose.cells.pivot/pivottable/formatall)(Style) | Format all the cell in the pivottable area |
| [FormatRow](../../aspose.cells.pivot/pivottable/formatrow)(int, Style) | Format the row data in the pivottable area |
| [GetCellByDisplayName](../../aspose.cells.pivot/pivottable/getcellbydisplayname)(string) | Gets the Cell object by the DisplayName of PivotField |
| [GetChildren](../../aspose.cells.pivot/pivottable/getchildren)() | Gets the Children Pivot Tables which use this PivotTable data as data source. |
| [GetHorizontalBreaks](../../aspose.cells.pivot/pivottable/gethorizontalbreaks)() | get pivot table row index list of horizontal pagebreaks |
| [GetSource](../../aspose.cells.pivot/pivottable/getsource)() | Get pivottable's source data. |
| [Move](../../aspose.cells.pivot/pivottable/move#move_1)(string) | Moves the PivotTable to a different location in the worksheet. |
| [Move](../../aspose.cells.pivot/pivottable/move#move)(int, int) | Moves the PivotTable to a different location in the worksheet. |
| [RefreshData](../../aspose.cells.pivot/pivottable/refreshdata)() | Refreshes pivottable's data and setting from it's data source. |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield#removefield_1)(PivotFieldType, int) | Removes a field from specific field area |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield#removefield)(PivotFieldType, PivotField) | Remove field from specific field area |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield#removefield_2)(PivotFieldType, string) | Removes a field from specific field area |
| [SetAutoGroupField](../../aspose.cells.pivot/pivottable/setautogroupfield#setautogroupfield_1)(int) | Sets auto field group by the PivotTable. |
| [SetAutoGroupField](../../aspose.cells.pivot/pivottable/setautogroupfield#setautogroupfield)(PivotField) | Sets auto field group by the PivotTable. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield_3)(int, DateTime, DateTime, ArrayList, int) | Sets manual field group by the PivotTable. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield_2)(int, double, double, ArrayList, double) | Sets manual field group by the PivotTable. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield_1)(PivotField, DateTime, DateTime, ArrayList, int) | Sets manual field group by the PivotTable. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield)(PivotField, double, double, ArrayList, double) | Sets manual field group by the PivotTable. |
| [SetUngroup](../../aspose.cells.pivot/pivottable/setungroup#setungroup_1)(int) | Sets ungroup by the PivotTable |
| [SetUngroup](../../aspose.cells.pivot/pivottable/setungroup#setungroup)(PivotField) | Sets ungroup by the PivotTable |
| [ShowInCompactForm](../../aspose.cells.pivot/pivottable/showincompactform)() | Layouts the PivotTable in compact form. |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivottable/showinoutlineform)() | Layouts the PivotTable in outline form. |
| [ShowInTabularForm](../../aspose.cells.pivot/pivottable/showintabularform)() | Layouts the PivotTable in tabular form. |
| [ShowReportFilterPage](../../aspose.cells.pivot/pivottable/showreportfilterpage)(PivotField) | Show all the report filter pages according to PivotField, the PivotField must be located in the PageFields. |
| [ShowReportFilterPageByIndex](../../aspose.cells.pivot/pivottable/showreportfilterpagebyindex)(int) | Show all the report filter pages according to the position index in the PageFields |
| [ShowReportFilterPageByName](../../aspose.cells.pivot/pivottable/showreportfilterpagebyname)(string) | Show all the report filter pages according to PivotField's name, the PivotField must be located in the PageFields. |

### Examples

```csharp

[C#]

Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
cells[0, 0].Value = "fruit";
cells[1, 0].Value = "grape";
cells[2, 0].Value = "blueberry";
cells[3, 0].Value = "kiwi";
cells[4, 0].Value = "cherry";
cells[5, 0].Value = "grape";
cells[6, 0].Value = "blueberry";
cells[7, 0].Value = "kiwi";
cells[8, 0].Value = "cherry";

cells[0, 1].Value = "year";
cells[1, 1].Value = 2020;
cells[2, 1].Value = 2020;
cells[3, 1].Value = 2020;
cells[4, 1].Value = 2020;
cells[5, 1].Value = 2021;
cells[6, 1].Value = 2021;
cells[7, 1].Value = 2021;
cells[8, 1].Value = 2021;

cells[0, 2].Value = "amount";
cells[1, 2].Value = 50;
cells[2, 2].Value = 60;
cells[3, 2].Value = 70;
cells[4, 2].Value = 80;
cells[5, 2].Value = 90;
cells[6, 2].Value = 100;
cells[7, 2].Value = 110;
cells[8, 2].Value = 120;

PivotTableCollection pivots = sheet.PivotTables;

int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

//Change PivotField's attributes
PivotField rowField = pivot.RowFields[0];
rowField.DisplayName = "custom display name";

//Add PivotFilter
int index = pivot.PivotFilters.Add(0, PivotFilterType.Count);
PivotFilter filter = pivot.PivotFilters[index];
filter.AutoFilter.FilterTop10(0, false, false, 2);

//Add PivotFormatCondition
int formatIndex = pivot.PivotFormatConditions.Add();
PivotFormatCondition pfc = pivot.PivotFormatConditions[formatIndex];
FormatConditionCollection fcc = pfc.FormatConditions;
fcc.AddArea(pivot.DataBodyRange);
int idx = fcc.AddCondition(FormatConditionType.CellValue);
FormatCondition fc = fcc[idx];
fc.Formula1 = "100";
fc.Operator = OperatorType.GreaterOrEqual;
fc.Style.BackgroundColor = Color.Red;

pivot.RefreshData();
pivot.CalculateData();

//do your business

book.Save("out.xlsx");

[Visual Basic]

Dim book As Workbook = New Workbook()
Dim sheet As Worksheet = book.Worksheets(0)
Dim cells As Cells = sheet.Cells

cells(0, 0).Value = "fruit"
cells(1, 0).Value = "grape"
cells(2, 0).Value = "blueberry"
cells(3, 0).Value = "kiwi"
cells(4, 0).Value = "cherry"
cells(5, 0).Value = "grape"
cells(6, 0).Value = "blueberry"
cells(7, 0).Value = "kiwi"
cells(8, 0).Value = "cherry"

cells(0, 1).Value = "year"
cells(1, 1).Value = 2020
cells(2, 1).Value = 2020
cells(3, 1).Value = 2020
cells(4, 1).Value = 2020
cells(5, 1).Value = 2021
cells(6, 1).Value = 2021
cells(7, 1).Value = 2021
cells(8, 1).Value = 2021

cells(0, 2).Value = "amount"
cells(1, 2).Value = 50
cells(2, 2).Value = 60
cells(3, 2).Value = 70
cells(4, 2).Value = 80
cells(5, 2).Value = 90
cells(6, 2).Value = 100
cells(7, 2).Value = 110
cells(8, 2).Value = 120

Dim pivots As PivotTableCollection = sheet.PivotTables
Dim pivotIndex As Int32 = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable")
Dim pivot As PivotTable = pivots(pivotIndex)
pivot.AddFieldToArea(PivotFieldType.Row, "fruit")
Pivot.AddFieldToArea(PivotFieldType.Column, "year")
Pivot.AddFieldToArea(PivotFieldType.Data, "amount")

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10

'Change PivotField's attributes
Dim rowField As PivotField = pivot.RowFields(0)
rowField.DisplayName = "custom display name"

'Add PivotFilter
Dim filterIndex As Int32 = pivot.PivotFilters.Add(0, PivotFilterType.Count)
Dim filter As PivotFilter = pivot.PivotFilters(filterIndex)
filter.AutoFilter.FilterTop10(0, False, False, 2)

'Add PivotFormatCondition
Dim formatIndex As Int32 = pivot.PivotFormatConditions.Add()
Dim pfc As PivotFormatCondition = pivot.PivotFormatConditions(formatIndex)
Dim fcc As FormatConditionCollection = pfc.FormatConditions
fcc.AddArea(pivot.DataBodyRange)
Dim idx As Int32 = fcc.AddCondition(FormatConditionType.CellValue)
Dim fc As FormatCondition = fcc(idx)
fc.Formula1 = "100"
fc.Operator = OperatorType.GreaterOrEqual
fc.Style.BackgroundColor = Color.Red

pivot.RefreshData()
pivot.CalculateData()

book.Save("out_vb.xlsx")
```

### See Also

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
