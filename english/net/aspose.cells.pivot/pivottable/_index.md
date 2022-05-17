---
title: PivotTable
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 4680
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
| [AltTextDescription](alttextdescription) { get; set; } | Gets the description of the alt text |
| [AltTextTitle](alttexttitle) { get; set; } | Gets the title of the altertext |
| [AutoFormatType](autoformattype) { get; set; } | Gets the PivotTable auto format type. |
| [BaseFields](basefields) { get; } | Returns a PivotFields object that includes all fields in the PivotTable report |
| [ColumnFields](columnfields) { get; } | Returns a PivotFields object that are currently shown as column fields. |
| [ColumnGrand](columngrand) { get; set; } | Indicates whether the PivotTable report shows grand totals for columns. |
| [ColumnHeaderCaption](columnheadercaption) { get; set; } | Gets the Column Header Caption of the PivotTable. |
| [ColumnRange](columnrange) { get; } | Returns a CellArea object that represents the range that contains the column area in the PivotTable report. Read-only. |
| [CustomListSort](customlistsort) { get; set; } | Indicates whether consider built-in custom list when sort data |
| [DataBodyRange](databodyrange) { get; } | Returns a CellArea object that represents the range that contains the data area in the list between the header row and the insert row. Read-only. |
| [DataField](datafield) { get; } | Gets a PivotField object that represents all the data fields in a PivotTable. Read-only.It would be init only when there are two or more data fields in the DataPiovtFiels. It only use to add DataPivotField to the PivotTable row/column area . Default is in row area. |
| [DataFields](datafields) { get; } | Gets a PivotField object that represents all the data fields in a PivotTable. Read-only.It would be init only when there are two or more data fields in the DataPiovtFiels. It only use to add DataPivotField to the PivotTable row/column area . Default is in row area. |
| [DataSource](datasource) { get; set; } | Gets and sets the data source of the pivot table. |
| [DisplayErrorString](displayerrorstring) { get; set; } | Indicates whether the PivotTable report displays a custom string in cells that contain errors. |
| [DisplayImmediateItems](displayimmediateitems) { get; set; } | Indicates whether items in the row and column areas are visible when the data area of the PivotTable is empty. The default value is true. |
| [DisplayNullString](displaynullstring) { get; set; } | Indicates whether the PivotTable report displays a custom string in cells that contain null values. |
| [EnableDataValueEditing](enabledatavalueediting) { get; set; } | Specifies a boolean value that indicates whether the user is allowed to edit the cells in the data area of the pivottable. Enable cell editing in the values area |
| [EnableDrilldown](enabledrilldown) { get; set; } | Gets whether drilldown is enabled. |
| [EnableFieldDialog](enablefielddialog) { get; set; } | Indicates whether the PivotTable Field dialog box is available when the user double-clicks the PivotTable field. |
| [EnableFieldList](enablefieldlist) { get; set; } | Gets whether enable the field list for the PivotTable. |
| [EnableWizard](enablewizard) { get; set; } | Indicates whether the PivotTable Wizard is available. |
| [ErrorString](errorstring) { get; set; } | Gets the string displayed in cells that contain errors when the DisplayErrorString property is true.The default value is an empty string. |
| [ExternalConnectionDataSource](externalconnectiondatasource) { get; } | Gets the external connection data source. |
| [FieldListSortAscending](fieldlistsortascending) { get; set; } | Specifies a boolean value that indicates whether fields in the PivotTable are sorted in non-default order in the field list. |
| [GrandTotalName](grandtotalname) { get; set; } | Returns the text string label that is displayed in the grand total column or row heading. The default value is the string "Grand Total". |
| [HasBlankRows](hasblankrows) { get; set; } | Indicates whether to add blank rows. This property only applies for the PivotTable auto format types which needs to add blank rows. |
| [Indent](indent) { get; set; } | Specifies the indentation increment for compact axis and can be used to set the Report Layout to Compact Form. |
| [IsAutoFormat](isautoformat) { get; set; } | Indicates whether the PivotTable report is automatically formatted. Checkbox "autoformat table " which is in pivottable option for Excel 2003 Checkbox "autofit column width on update" which is in pivot table Options :Layout Format for Excel 2007 |
| [IsExcel2003Compatible](isexcel2003compatible) { get; set; } | Specifies whether the PivotTable is compatible for Excel2003 when refreshing PivotTable, if true, a string must be less than or equal to 255 characters, so if the string is greater than 255 characters, it will be truncated. if false, a string will not have the aforementioned restriction. The default value is true. |
| [IsGridDropZones](isgriddropzones) { get; set; } | Indicates whether the PivotTable report displays classic pivottable layout. (enables dragging fields in the grid) |
| [IsMultipleFieldFilters](ismultiplefieldfilters) { get; set; } | Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. |
| [IsSelected](isselected) { get; set; } | Indicates whether the PivotTable is selected. |
| [ItemPrintTitles](itemprinttitles) { get; set; } | A bit that specifies whether pivot item captions on the row axis are repeated on each printed page for pivot fields in tabular form. |
| [ManualUpdate](manualupdate) { get; set; } | Indicates whether the PivotTable report is recalculated only at the user's request. |
| [MergeLabels](mergelabels) { get; set; } | Indicates whether the specified PivotTable report's outer-row item, column item, subtotal, and grand total labels use merged cells. |
| [MissingItemsLimit](missingitemslimit) { get; set; } | Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. |
| [Name](name) { get; set; } | Gets the name of the PivotTable |
| [NullString](nullstring) { get; set; } | Gets the string displayed in cells that contain null values when the DisplayNullString property is true.The default value is an empty string. |
| [PageFieldOrder](pagefieldorder) { get; set; } | Gets the order in which page fields are added to the PivotTable report's layout. |
| [PageFields](pagefields) { get; } | Returns a PivotFields object that are currently shown as page fields. |
| [PageFieldWrapCount](pagefieldwrapcount) { get; set; } | Gets the number of page fields in each column or row in the PivotTable report. |
| [PivotFilters](pivotfilters) { get; } | Returns a PivotFilterCollection object. |
| [PivotFormatConditions](pivotformatconditions) { get; } | Gets the Format Conditions of the pivot table. |
| [PivotTableStyleName](pivottablestylename) { get; set; } | Gets and sets the pivottable style name. |
| [PivotTableStyleType](pivottablestyletype) { get; set; } | Gets and sets the built-in pivot table style. |
| [PreserveFormatting](preserveformatting) { get; set; } | Indicates whether formatting is preserved when the PivotTable is refreshed or recalculated. |
| [PrintDrill](printdrill) { get; set; } | Specifies a boolean value that indicates whether drill indicators should be printed. print expand/collapse buttons when displayed on pivottable. |
| [PrintTitles](printtitles) { get; set; } | Indicates whether the print titles for the worksheet are set based on the PivotTable report. The default value is false. |
| [RefreshDataFlag](refreshdataflag) { get; set; } | Indicates whether Refresh Data or not. |
| [RefreshDataOnOpeningFile](refreshdataonopeningfile) { get; set; } | Indicates whether Refresh Data when Opening File. |
| [RefreshDate](refreshdate) { get; } | Gets the date when the PivotTable was last refreshed. |
| [RefreshedByWho](refreshedbywho) { get; } | Gets the name of the user who last refreshed the PivotTable |
| [RowFields](rowfields) { get; } | Returns a PivotFields object that are currently shown as row fields. |
| [RowGrand](rowgrand) { get; set; } | Indicates whether the PivotTable report shows grand totals for rows. |
| [RowHeaderCaption](rowheadercaption) { get; set; } | Gets the Row Header Caption of the PivotTable. |
| [RowRange](rowrange) { get; } | Returns a CellArea object that represents the range that contains the row area in the PivotTable report. Read-only. |
| [SaveData](savedata) { get; set; } | Indicates whether data for the PivotTable report is saved with the workbook. |
| [ShowDataTips](showdatatips) { get; set; } | Specifies a boolean value that indicates whether tooltips should be displayed for PivotTable data cells. |
| [ShowDrill](showdrill) { get; set; } | Gets whether expand/collapse buttons is shown. |
| [ShowEmptyCol](showemptycol) { get; set; } | Specifies a boolean value that indicates whether to include empty columns in the table |
| [ShowEmptyRow](showemptyrow) { get; set; } | Specifies a boolean value that indicates whether to include empty rows in the table. |
| [ShowMemberPropertyTips](showmemberpropertytips) { get; set; } | Specifies a boolean value that indicates whether member property information should be omitted from PivotTable tooltips. |
| [ShowPivotStyleColumnHeader](showpivotstylecolumnheader) { get; set; } | Indicates whether the column header in the pivot table should have the style applied. |
| [ShowPivotStyleColumnStripes](showpivotstylecolumnstripes) { get; set; } | Indicates whether column stripe formatting is applied. |
| [ShowPivotStyleLastColumn](showpivotstylelastcolumn) { get; set; } | Indicates whether column stripe formatting is applied. |
| [ShowPivotStyleRowHeader](showpivotstylerowheader) { get; set; } | Indicates whether the row header in the pivot table should have the style applied. |
| [ShowPivotStyleRowStripes](showpivotstylerowstripes) { get; set; } | Indicates whether row stripe formatting is applied. |
| [ShowRowHeaderCaption](showrowheadercaption) { get; set; } | Indicates whether row header caption is shown in the PivotTable report Indicates whether Display field captions and filter drop downs |
| [ShowValuesRow](showvaluesrow) { get; set; } | Specifies a boolean value that indicates whether show values row. show the values row |
| [SubtotalHiddenPageItems](subtotalhiddenpageitems) { get; set; } | Indicates whether hidden page field items in the PivotTable report are included in row and column subtotals, block totals, and grand totals. The default value is False. |
| [TableRange1](tablerange1) { get; } | Returns a CellArea object that represents the range containing the entire PivotTable report, but doesn't include page fields. Read-only. |
| [TableRange2](tablerange2) { get; } | Returns a CellArea object that represents the range containing the entire PivotTable report, includes page fields. Read-only. |
| [Tag](tag) { get; set; } | Gets a string saved with the PivotTable report. |

## Methods

| Name | Description |
| --- | --- |
| [AddCalculatedField](addcalculatedfield)(string, string) | Adds a calculated field to pivot field and drag it to data area. |
| [AddCalculatedField](addcalculatedfield)(string, string, bool) | Adds a calculated field to pivot field. |
| [AddFieldToArea](addfieldtoarea)(PivotFieldType, int) | Adds the field to the specific area. |
| [AddFieldToArea](addfieldtoarea)(PivotFieldType, PivotField) | Adds the field to the specific area. |
| [AddFieldToArea](addfieldtoarea)(PivotFieldType, string) | Adds the field to the specific area. |
| [CalculateData](calculatedata)() | Calculates pivottable's data to cells. |
| [CalculateRange](calculaterange)() | Calculates pivottable's range. |
| [ChangeDataSource](changedatasource)(string[]) | Set pivottable's source data. Sheet1!$A$1:$C$3 |
| [ClearData](cleardata)() | Clear PivotTable's data and formatting |
| [CopyStyle](copystyle)(PivotTable) | Copies named style from another pivot table. |
| [Dispose](dispose)() | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [Fields](fields)(PivotFieldType) | Gets the specific fields by the field type. |
| [Format](format)(int, int, Style) | Format the cell in the pivottable area |
| [FormatAll](formatall)(Style) | Format all the cell in the pivottable area |
| [GetCellByDisplayName](getcellbydisplayname)(string) | Gets the Cell object by the DisplayName of PivotField |
| [GetChildren](getchildren)() | Gets the Children Pivot Tables which use this PivotTable data as data source. |
| [GetHorizontalBreaks](gethorizontalbreaks)() | get pivot table row index list of horizontal pagebreaks |
| [GetSource](getsource)() | Get pivottable's source data. |
| [Move](move)(string) | Moves the PivotTable to a different location in the worksheet. |
| [Move](move)(int, int) | Moves the PivotTable to a different location in the worksheet. |
| [RefreshData](refreshdata)() | Refreshes pivottable's data and setting from it's data source. |
| [RemoveField](removefield)(PivotFieldType, int) | Removes a field from specific field area |
| [RemoveField](removefield)(PivotFieldType, PivotField) | Remove field from specific field area |
| [RemoveField](removefield)(PivotFieldType, string) | Removes a field from specific field area |
| [SetAutoGroupField](setautogroupfield)(int) | Sets auto field group by the PivotTable. |
| [SetAutoGroupField](setautogroupfield)(PivotField) | Sets auto field group by the PivotTable. |
| [SetManualGroupField](setmanualgroupfield)(int, DateTime, DateTime, ArrayList, int) | Sets manual field group by the PivotTable. |
| [SetManualGroupField](setmanualgroupfield)(int, double, double, ArrayList, double) | Sets manual field group by the PivotTable. |
| [SetManualGroupField](setmanualgroupfield)(PivotField, DateTime, DateTime, ArrayList, int) | Sets manual field group by the PivotTable. |
| [SetManualGroupField](setmanualgroupfield)(PivotField, double, double, ArrayList, double) | Sets manual field group by the PivotTable. |
| [SetUngroup](setungroup)(int) | Sets ungroup by the PivotTable |
| [SetUngroup](setungroup)(PivotField) | Sets ungroup by the PivotTable |
| [ShowInCompactForm](showincompactform)() | Layouts the PivotTable in compact form. |
| [ShowInOutlineForm](showinoutlineform)() | Layouts the PivotTable in outline form. |
| [ShowInTabularForm](showintabularform)() | Layouts the PivotTable in tabular form. |
| [ShowReportFilterPage](showreportfilterpage)(PivotField) | Show all the report filter pages according to PivotField, the PivotField must be located in the PageFields. |
| [ShowReportFilterPageByIndex](showreportfilterpagebyindex)(int) | Show all the report filter pages according to the position index in the PageFields |
| [ShowReportFilterPageByName](showreportfilterpagebyname)(string) | Show all the report filter pages according to PivotField's name, the PivotField must be located in the PageFields. |

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
