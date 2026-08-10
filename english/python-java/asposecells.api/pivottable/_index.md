---
title: "PivotTable Class"
linktitle: "PivotTable"
articleTitle: "PivotTable"
second_title: "Aspose.Cells for Python via Java"
description: "Summary description for PivotTable."
type: docs
weight: 4820
url: /python-java/asposecells.api/pivottable/
---

## PivotTable class

Summary description for PivotTable.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [PivotCache](#pivotcache) | PivotCache |  |
| [IsExcel2003Compatible](#isexcel2003compatible) | boolean | Specifies whether the PivotTable is compatible for Excel2003 when refreshing PivotTable, if true, a string must be less  |
| [RefreshedByWho](#refreshedbywho) | String | Gets the name of the last user who refreshed this PivotTable |
| [RefreshDate](#refreshdate) | DateTime | Gets the last date time when the PivotTable was refreshed. |
| [PivotTableStyle](#pivottablestyle) | TableStyle |  |
| [PivotTableStyleName](#pivottablestylename) | String | Gets and sets the pivottable style name. |
| [PivotTableStyleType](#pivottablestyletype) | int | Gets and sets the built-in pivot table style. The value of the property is PivotTableStyleType integer constant. |
| [ColumnFields](#columnfields) | PivotFieldCollection | Returns a PivotFields object that are currently shown as column fields. |
| [RowFields](#rowfields) | PivotFieldCollection | Returns a PivotFields object that are currently shown as row fields. |
| [PageFields](#pagefields) | PivotFieldCollection | Returns a PivotFields object that are currently shown as page fields. |
| [DataFields](#datafields) | PivotFieldCollection | Gets a PivotField object that represents all the data fields in a PivotTable. Read-only.It would be init only when there |
| [DataField](#datafield) | PivotField | Gets a PivotField object that represents all the data fields in a PivotTable. Read-only. It would only be created when t |
| [ValuesField](#valuesfield) | PivotField |  |
| [BaseFields](#basefields) | PivotFieldCollection | Returns all base pivot fields in the PivotTable. |
| [PivotFilters](#pivotfilters) | PivotFilterCollection | Returns a list of pivot filters. |
| [TopRightArea](#toprightarea) | CellArea |  |
| [FilterArea](#filterarea) | CellArea |  |
| [ColumnRange](#columnrange) | CellArea | Returns a CellArea object that represents the range that contains the column area in the PivotTable report. Read-only. |
| [RowRange](#rowrange) | CellArea | Returns a CellArea object that represents the range that contains the row area in the PivotTable report. Read-only. |
| [DataBodyRange](#databodyrange) | CellArea | Returns a CellArea object that represents the range that contains the data area in the list between the header row and t |
| [TableRange1](#tablerange1) | CellArea | Returns a CellArea object that represents the range containing the entire PivotTable report, but doesn't include page fi |
| [TableRange2](#tablerange2) | CellArea | Returns a CellArea object that represents the range containing the entire PivotTable report, includes page fields. Read- |
| [IsGridDropZones](#isgriddropzones) | boolean | Indicates whether the PivotTable report displays classic pivottable layout. (enables dragging fields in the grid) |
| [ShowColumnGrandTotals](#showcolumngrandtotals) | boolean |  |
| [ShowRowGrandTotals](#showrowgrandtotals) | boolean |  |
| [ColumnGrand](#columngrand) | boolean | Indicates whether the PivotTable report shows grand totals for columns. |
| [RowGrand](#rowgrand) | boolean | Indicates whether the PivotTable report shows grand totals for rows. |
| [DisplayNullString](#displaynullstring) | boolean | Indicates whether the PivotTable report displays a custom string if the value is null. |
| [NullString](#nullstring) | String | Gets the string displayed in cells that contain null values when the DisplayNullString property is true.The default valu |
| [DisplayErrorString](#displayerrorstring) | boolean | Indicates whether the PivotTable report displays a custom string in cells that contain errors. |
| [DataFieldHeaderName](#datafieldheadername) | String | Gets and sets the name of the value area field header in the PivotTable. |
| [ErrorString](#errorstring) | String | Gets the string displayed in cells that contain errors when the DisplayErrorString property is true.The default value is |
| [IsAutoFormat](#isautoformat) | boolean | Indicates whether the PivotTable report is automatically formatted. Checkbox "autoformat table " which is in pivottable  |
| [AutofitColumnWidthOnUpdate](#autofitcolumnwidthonupdate) | boolean | Indicates whether autofitting column width on update |
| [AutoFormatType](#autoformattype) | int | Gets and sets the auto format type of PivotTable. The value of the property is PivotTableAutoFormatType integer constant |
| [HasBlankRows](#hasblankrows) | boolean | Indicates whether to add blank rows. This property only applies for the PivotTable auto format types which needs to add  |
| [MergeLabels](#mergelabels) | boolean | True if the specified PivotTable report's outer-row item, column item, subtotal, and grand total labels use merged cells |
| [PreserveFormatting](#preserveformatting) | boolean | Indicates whether formatting is preserved when the PivotTable is refreshed or recalculated. |
| [ShowDrill](#showdrill) | boolean | Gets and sets whether showing expand/collapse buttons. |
| [EnableDrilldown](#enabledrilldown) | boolean | Gets whether drilldown is enabled. |
| [EnableFieldDialog](#enablefielddialog) | boolean | Indicates whether the PivotTable Field dialog box is available when the user double-clicks the PivotTable field. |
| [EnableFieldList](#enablefieldlist) | boolean | Gets whether enable the field list for the PivotTable. |
| [EnableWizard](#enablewizard) | boolean | Indicates whether the PivotTable Wizard is available. |
| [SubtotalHiddenPageItems](#subtotalhiddenpageitems) | boolean | Indicates whether hidden page field items in the PivotTable report are included in row and column subtotals, block total |
| [GrandTotalName](#grandtotalname) | String | Returns the text string label that is displayed in the grand total column or row heading. The default value is the strin |
| [ManualUpdate](#manualupdate) | boolean | Indicates whether the PivotTable report is recalculated only at the user's request. |
| [IsMultipleFieldFilters](#ismultiplefieldfilters) | boolean | Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. |
| [AllowMultipleFiltersPerField](#allowmultiplefiltersperfield) | boolean |  |
| [MissingItemsLimit](#missingitemslimit) | int | Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. The v |
| [EnableDataValueEditing](#enabledatavalueediting) | boolean | Specifies a boolean value that indicates whether the user is allowed to edit the cells in the data area of the pivottabl |
| [ShowDataTips](#showdatatips) | boolean | Specifies a boolean value that indicates whether tooltips should be displayed for PivotTable data cells. |
| [ShowMemberPropertyTips](#showmemberpropertytips) | boolean | Specifies a boolean value that indicates whether member property information should be omitted from PivotTable tooltips. |
| [ShowValuesRow](#showvaluesrow) | boolean | Specifies a boolean value that indicates whether show values row. show the values row |
| [ShowEmptyCol](#showemptycol) | boolean | Specifies a boolean value that indicates whether to include empty columns in the table |
| [ShowEmptyRow](#showemptyrow) | boolean | Specifies a boolean value that indicates whether to include empty rows in the table. |
| [FieldListSortAscending](#fieldlistsortascending) | boolean | Indicates whether fields in the PivotTable are sorted in non-default order in the field list. |
| [PrintDrill](#printdrill) | boolean | Specifies a boolean value that indicates whether drill indicators should be printed. print expand/collapse buttons when  |
| [AltTextTitle](#alttexttitle) | String | Gets the title of the altertext |
| [AltTextDescription](#alttextdescription) | String | Gets the description of the alt text |
| [Name](#name) | String | Gets the name of the PivotTable |
| [ColumnHeaderCaption](#columnheadercaption) | String | Gets the Column Header Caption of the PivotTable. |
| [Indent](#indent) | int | Specifies the indentation increment for compact axis and can be used to set the Report Layout to Compact Form. |
| [RowHeaderCaption](#rowheadercaption) | String | Gets the Row Header Caption of the PivotTable. |
| [ShowRowHeaderCaption](#showrowheadercaption) | boolean | Indicates whether row header caption is shown in the PivotTable report Indicates whether Display field captions and filt |
| [CustomListSort](#customlistsort) | boolean | Indicates whether consider built-in custom list when sort data |
| [PivotFormatConditions](#pivotformatconditions) | PivotFormatConditionCollection | Gets the Format Conditions of the pivot table. |
| [ConditionalFormats](#conditionalformats) | PivotConditionalFormatCollection |  |
| [PageFieldOrder](#pagefieldorder) | int | Gets the order in which page fields are added to the PivotTable report's layout. The value of the property is PrintOrder |
| [PageFieldWrapCount](#pagefieldwrapcount) | int | Gets the number of page fields in each column or row in the PivotTable report. |
| [Tag](#tag) | String | Gets a string saved with the PivotTable report. |
| [SaveData](#savedata) | boolean | Indicates whether data for the PivotTable report is saved with the workbook. |
| [RefreshDataOnOpeningFile](#refreshdataonopeningfile) | boolean | Indicates whether Refresh Data when Opening File. |
| [RefreshDataFlag](#refreshdataflag) | boolean | Indicates whether Refreshing Data or not. |
| [SourceType](#sourcetype) | byte | The value of the property is PivotTableSourceType integer constant. |
| [ExternalConnectionDataSource](#externalconnectiondatasource) | ExternalConnection | Gets the external connection data source. |
| [DataSource](#datasource) | String[] | Gets and sets the data source of the pivot table. |
| [PivotFormats](#pivotformats) | PivotTableFormatCollection | Gets the collection of formats applied to PivotTable. |
| [ItemPrintTitles](#itemprinttitles) | boolean | Indicates whether PivotItem names should be repeated at the top of each printed page. |
| [RepeatItemsOnEachPrintedPage](#repeatitemsoneachprintedpage) | boolean |  |
| [PrintTitles](#printtitles) | boolean | Indicates whether the print titles for the worksheet are set based on the PivotTable report. The default value is false. |
| [DisplayImmediateItems](#displayimmediateitems) | boolean | Indicates whether items in the row and column areas are visible when the data area of the PivotTable is empty. The defau |
| [IsSelected](#isselected) | boolean | Indicates whether this PivotTable is selected. |
| [ShowPivotStyleRowHeader](#showpivotstylerowheader) | boolean | Indicates whether the row header in the pivot table should have the style applied. |
| [ShowPivotStyleColumnHeader](#showpivotstylecolumnheader) | boolean | Indicates whether the column header in the pivot table should have the style applied. |
| [ShowPivotStyleRowStripes](#showpivotstylerowstripes) | boolean | Indicates whether row stripe formatting is applied. |
| [ShowPivotStyleColumnStripes](#showpivotstylecolumnstripes) | boolean | Indicates whether stripe formatting is applied for column. |
| [ShowPivotStyleLastColumn](#showpivotstylelastcolumn) | boolean | Indicates whether the column formatting is applied. |

## Methods

| Name | Description |
| --- | --- |
| [getHorizontalPageBreaks](#gethorizontalpagebreaks) |  |
| [getHorizontalBreaks](#gethorizontalbreaks) | get pivot table row index list of horizontal pagebreaks |
| [showInCompactForm](#showincompactform) | Layouts the PivotTable in compact form. |
| [showInOutlineForm](#showinoutlineform) | Layouts the PivotTable in outline form. |
| [showInTabularForm](#showintabularform) | Layouts the PivotTable in tabular form. |
| [getCellByDisplayName](#getcellbydisplayname) | Gets the Cell object by the display name of PivotField. |
| [getDependentPivotTables](#getdependentpivottables) |  |
| [getChildren](#getchildren) | Gets the Children Pivot Tables which use this PivotTable data as data source. |
| [getSourceDataConnections](#getsourcedataconnections) |  |
| [getNamesOfSourceDataConnections](#getnamesofsourcedataconnections) |  |
| [changeDataSource](#changedatasource) | Set pivottable's source data. Sheet1!$A$1:$C$3 |
| [getSource](#getsource) | Get pivottable's source data. |
| [refreshData](#refreshdata) | Refreshes pivottable's data and setting from it's data source.

We will gather data from data source to a pivot cache ,t |
| [calculateData](#calculatedata) | Calculates pivottable's data to cells.

Cell.Value in the pivot range could not return the correct result if the method  |
| [getPivotTablesWithSamePivotCache](#getpivottableswithsamepivotcache) |  |
| [clearData](#cleardata) | Clear PivotTable's data and formatting

If this method is not called before you add or delete PivotField, Maybe the Pivo |
| [clearFilters](#clearfilters) |  |
| [clearAll](#clearall) |  |
| [calculateRange](#calculaterange) | Calculates pivottable's range.

If this method is not been called,maybe the pivottable range is not corrected. |
| [formatAll](#formatall) | Format all the cell in the pivottable area |
| [formatRow](#formatrow) | Format the row data in the pivottable area |
| [format](#format) | Formats selected area of the PivotTable. |
| [selectArea](#selectarea) |  |
| [showDetail](#showdetail) |  |
| [setAutoGroupField](#setautogroupfield) | Sets auto field group by the PivotTable.

baseFieldIndex - The row or column field index in the base fields NOTE: This m |
| [setManualGroupField](#setmanualgroupfield) | Sets manual field group by the PivotTable.

NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy()  |
| [setUngroup](#setungroup) | Sets ungroup by the PivotTable

NOTE: This method is now obsolete. Instead, please use PivotField.Ungroup() method. This |
| [dispose](#dispose) | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [copyStyle](#copystyle) | Copies named style from another pivot table. |
| [showReportFilterPage](#showreportfilterpage) | Show all the report filter pages according to PivotField, the PivotField must be located in the PageFields. |
| [showReportFilterPageByName](#showreportfilterpagebyname) | Show all the report filter pages according to PivotField's name, the PivotField must be located in the PageFields. |
| [showReportFilterPageByIndex](#showreportfilterpagebyindex) | Show all the report filter pages according to the position index in the PageFields |
| [removeField](#removefield) | Removes a field from specific field area |
| [addFieldToArea](#addfieldtoarea) | Adds the field to the specific area. |
| [addCalculatedField](#addcalculatedfield) | Adds a calculated field to pivot field. |
| [getFields](#getfields) | Gets the specific pivot field list by the region. |
| [fields](#fields) | Gets the specific fields by the field type.

NOTE: This method is now obsolete. Instead, please use PivotField.GetFields |
| [getButtonArea](#getbuttonarea) |  |
| [move](#move) | Moves the PivotTable to a different location in the worksheet. |
| [moveTo](#moveto) |  |

### PivotTable.PivotCache property {#pivotcache}

**Type:** PivotCache

### PivotTable.IsExcel2003Compatible property {#isexcel2003compatible}

Specifies whether the PivotTable is compatible for Excel2003 when refreshing PivotTable, if true, a string must be less than or equal to 255 characters, so if the string is greater than 255 characters, it will be truncated. if false, a string will not have the aforementioned restriction. The default value is true.

**Type:** boolean

### PivotTable.RefreshedByWho property {#refreshedbywho}

Gets the name of the last user who refreshed this PivotTable

**Type:** String

### PivotTable.RefreshDate property {#refreshdate}

Gets the last date time when the PivotTable was refreshed.

**Type:** DateTime

### PivotTable.PivotTableStyle property {#pivottablestyle}

**Type:** TableStyle

### PivotTable.PivotTableStyleName property {#pivottablestylename}

Gets and sets the pivottable style name.

**Type:** String

### PivotTable.PivotTableStyleType property {#pivottablestyletype}

Gets and sets the built-in pivot table style. The value of the property is PivotTableStyleType integer constant.

**Type:** int

### PivotTable.ColumnFields property {#columnfields}

Returns a PivotFields object that are currently shown as column fields.

**Type:** PivotFieldCollection

### PivotTable.RowFields property {#rowfields}

Returns a PivotFields object that are currently shown as row fields.

**Type:** PivotFieldCollection

### PivotTable.PageFields property {#pagefields}

Returns a PivotFields object that are currently shown as page fields.

**Type:** PivotFieldCollection

### PivotTable.DataFields property {#datafields}

Gets a PivotField object that represents all the data fields in a PivotTable. Read-only.It would be init only when there are two or more data fields in the DataPiovtFiels. It only use to add DataPivotField to the PivotTable row/column area . Default is in row area.

**Type:** PivotFieldCollection

### PivotTable.DataField property {#datafield}

Gets a PivotField object that represents all the data fields in a PivotTable. Read-only. It would only be created when there are two or more data fields in the Data region. Defaultly it is in row region. You can drag it to the row/column region with PivotTable.AddFieldToArea() method .

**Type:** PivotField

### PivotTable.ValuesField property {#valuesfield}

**Type:** PivotField

### PivotTable.BaseFields property {#basefields}

Returns all base pivot fields in the PivotTable.

**Type:** PivotFieldCollection

### PivotTable.PivotFilters property {#pivotfilters}

Returns a list of pivot filters.

**Type:** PivotFilterCollection

### PivotTable.TopRightArea property {#toprightarea}

**Type:** CellArea

### PivotTable.FilterArea property {#filterarea}

**Type:** CellArea

### PivotTable.ColumnRange property {#columnrange}

Returns a CellArea object that represents the range that contains the column area in the PivotTable report. Read-only.

**Type:** CellArea

### PivotTable.RowRange property {#rowrange}

Returns a CellArea object that represents the range that contains the row area in the PivotTable report. Read-only.

**Type:** CellArea

### PivotTable.DataBodyRange property {#databodyrange}

Returns a CellArea object that represents the range that contains the data area in the list between the header row and the insert row. Read-only.

**Type:** CellArea

### PivotTable.TableRange1 property {#tablerange1}

Returns a CellArea object that represents the range containing the entire PivotTable report, but doesn't include page fields. Read-only.

**Type:** CellArea

### PivotTable.TableRange2 property {#tablerange2}

Returns a CellArea object that represents the range containing the entire PivotTable report, includes page fields. Read-only.

**Type:** CellArea

### PivotTable.IsGridDropZones property {#isgriddropzones}

Indicates whether the PivotTable report displays classic pivottable layout. (enables dragging fields in the grid)

**Type:** boolean

### PivotTable.ShowColumnGrandTotals property {#showcolumngrandtotals}

**Type:** boolean

### PivotTable.ShowRowGrandTotals property {#showrowgrandtotals}

**Type:** boolean

### PivotTable.ColumnGrand property {#columngrand}

Indicates whether the PivotTable report shows grand totals for columns.

**Type:** boolean

### PivotTable.RowGrand property {#rowgrand}

Indicates whether the PivotTable report shows grand totals for rows.

**Type:** boolean

### PivotTable.DisplayNullString property {#displaynullstring}

Indicates whether the PivotTable report displays a custom string if the value is null.

**Type:** boolean

### PivotTable.NullString property {#nullstring}

Gets the string displayed in cells that contain null values when the DisplayNullString property is true.The default value is an empty string.

**Type:** String

### PivotTable.DisplayErrorString property {#displayerrorstring}

Indicates whether the PivotTable report displays a custom string in cells that contain errors.

**Type:** boolean

### PivotTable.DataFieldHeaderName property {#datafieldheadername}

Gets and sets the name of the value area field header in the PivotTable.

**Type:** String

### PivotTable.ErrorString property {#errorstring}

Gets the string displayed in cells that contain errors when the DisplayErrorString property is true.The default value is an empty string.

**Type:** String

### PivotTable.IsAutoFormat property {#isautoformat}

Indicates whether the PivotTable report is automatically formatted. Checkbox "autoformat table " which is in pivottable option for Excel 2003

**Type:** boolean

### PivotTable.AutofitColumnWidthOnUpdate property {#autofitcolumnwidthonupdate}

Indicates whether autofitting column width on update

**Type:** boolean

### PivotTable.AutoFormatType property {#autoformattype}

Gets and sets the auto format type of PivotTable. The value of the property is PivotTableAutoFormatType integer constant.

**Type:** int

### PivotTable.HasBlankRows property {#hasblankrows}

Indicates whether to add blank rows. This property only applies for the PivotTable auto format types which needs to add blank rows.

**Type:** boolean

### PivotTable.MergeLabels property {#mergelabels}

True if the specified PivotTable report's outer-row item, column item, subtotal, and grand total labels use merged cells.

**Type:** boolean

### PivotTable.PreserveFormatting property {#preserveformatting}

Indicates whether formatting is preserved when the PivotTable is refreshed or recalculated.

**Type:** boolean

### PivotTable.ShowDrill property {#showdrill}

Gets and sets whether showing expand/collapse buttons.

**Type:** boolean

### PivotTable.EnableDrilldown property {#enabledrilldown}

Gets whether drilldown is enabled.

**Type:** boolean

### PivotTable.EnableFieldDialog property {#enablefielddialog}

Indicates whether the PivotTable Field dialog box is available when the user double-clicks the PivotTable field.

**Type:** boolean

### PivotTable.EnableFieldList property {#enablefieldlist}

Gets whether enable the field list for the PivotTable.

**Type:** boolean

### PivotTable.EnableWizard property {#enablewizard}

Indicates whether the PivotTable Wizard is available.

**Type:** boolean

### PivotTable.SubtotalHiddenPageItems property {#subtotalhiddenpageitems}

Indicates whether hidden page field items in the PivotTable report are included in row and column subtotals, block totals, and grand totals. The default value is False.

**Type:** boolean

### PivotTable.GrandTotalName property {#grandtotalname}

Returns the text string label that is displayed in the grand total column or row heading. The default value is the string "Grand Total".

**Type:** String

### PivotTable.ManualUpdate property {#manualupdate}

Indicates whether the PivotTable report is recalculated only at the user's request.

**Type:** boolean

### PivotTable.IsMultipleFieldFilters property {#ismultiplefieldfilters}

Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them.

**Type:** boolean

### PivotTable.AllowMultipleFiltersPerField property {#allowmultiplefiltersperfield}

**Type:** boolean

### PivotTable.MissingItemsLimit property {#missingitemslimit}

Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. The value of the property is PivotMissingItemLimitType integer constant.

**Type:** int

### PivotTable.EnableDataValueEditing property {#enabledatavalueediting}

Specifies a boolean value that indicates whether the user is allowed to edit the cells in the data area of the pivottable. Enable cell editing in the values area

**Type:** boolean

### PivotTable.ShowDataTips property {#showdatatips}

Specifies a boolean value that indicates whether tooltips should be displayed for PivotTable data cells.

**Type:** boolean

### PivotTable.ShowMemberPropertyTips property {#showmemberpropertytips}

Specifies a boolean value that indicates whether member property information should be omitted from PivotTable tooltips.

**Type:** boolean

### PivotTable.ShowValuesRow property {#showvaluesrow}

Specifies a boolean value that indicates whether show values row. show the values row

**Type:** boolean

### PivotTable.ShowEmptyCol property {#showemptycol}

Specifies a boolean value that indicates whether to include empty columns in the table

**Type:** boolean

### PivotTable.ShowEmptyRow property {#showemptyrow}

Specifies a boolean value that indicates whether to include empty rows in the table.

**Type:** boolean

### PivotTable.FieldListSortAscending property {#fieldlistsortascending}

Indicates whether fields in the PivotTable are sorted in non-default order in the field list.

**Type:** boolean

### PivotTable.PrintDrill property {#printdrill}

Specifies a boolean value that indicates whether drill indicators should be printed. print expand/collapse buttons when displayed on pivottable.

**Type:** boolean

### PivotTable.AltTextTitle property {#alttexttitle}

Gets the title of the altertext

**Type:** String

### PivotTable.AltTextDescription property {#alttextdescription}

Gets the description of the alt text

**Type:** String

### PivotTable.Name property {#name}

Gets the name of the PivotTable

**Type:** String

### PivotTable.ColumnHeaderCaption property {#columnheadercaption}

Gets the Column Header Caption of the PivotTable.

**Type:** String

### PivotTable.Indent property {#indent}

Specifies the indentation increment for compact axis and can be used to set the Report Layout to Compact Form.

**Type:** int

### PivotTable.RowHeaderCaption property {#rowheadercaption}

Gets the Row Header Caption of the PivotTable.

**Type:** String

### PivotTable.ShowRowHeaderCaption property {#showrowheadercaption}

Indicates whether row header caption is shown in the PivotTable report Indicates whether Display field captions and filter drop downs

**Type:** boolean

### PivotTable.CustomListSort property {#customlistsort}

Indicates whether consider built-in custom list when sort data

**Type:** boolean

### PivotTable.PivotFormatConditions property {#pivotformatconditions}

Gets the Format Conditions of the pivot table.

**Type:** PivotFormatConditionCollection

### PivotTable.ConditionalFormats property {#conditionalformats}

**Type:** PivotConditionalFormatCollection

### PivotTable.PageFieldOrder property {#pagefieldorder}

Gets the order in which page fields are added to the PivotTable report's layout. The value of the property is PrintOrderType integer constant.

**Type:** int

### PivotTable.PageFieldWrapCount property {#pagefieldwrapcount}

Gets the number of page fields in each column or row in the PivotTable report.

**Type:** int

### PivotTable.Tag property {#tag}

Gets a string saved with the PivotTable report.

**Type:** String

### PivotTable.SaveData property {#savedata}

Indicates whether data for the PivotTable report is saved with the workbook.

**Type:** boolean

### PivotTable.RefreshDataOnOpeningFile property {#refreshdataonopeningfile}

Indicates whether Refresh Data when Opening File.

**Type:** boolean

### PivotTable.RefreshDataFlag property {#refreshdataflag}

Indicates whether Refreshing Data or not.

**Type:** boolean

### PivotTable.SourceType property {#sourcetype}

The value of the property is PivotTableSourceType integer constant.

**Type:** byte

### PivotTable.ExternalConnectionDataSource property {#externalconnectiondatasource}

Gets the external connection data source.

**Type:** ExternalConnection

### PivotTable.DataSource property {#datasource}

Gets and sets the data source of the pivot table.

**Type:** String[]

### PivotTable.PivotFormats property {#pivotformats}

Gets the collection of formats applied to PivotTable.

**Type:** PivotTableFormatCollection

### PivotTable.ItemPrintTitles property {#itemprinttitles}

Indicates whether PivotItem names should be repeated at the top of each printed page.

**Type:** boolean

### PivotTable.RepeatItemsOnEachPrintedPage property {#repeatitemsoneachprintedpage}

**Type:** boolean

### PivotTable.PrintTitles property {#printtitles}

Indicates whether the print titles for the worksheet are set based on the PivotTable report. The default value is false.

**Type:** boolean

### PivotTable.DisplayImmediateItems property {#displayimmediateitems}

Indicates whether items in the row and column areas are visible when the data area of the PivotTable is empty. The default value is true.

**Type:** boolean

### PivotTable.IsSelected property {#isselected}

Indicates whether this PivotTable is selected.

**Type:** boolean

### PivotTable.ShowPivotStyleRowHeader property {#showpivotstylerowheader}

Indicates whether the row header in the pivot table should have the style applied.

**Type:** boolean

### PivotTable.ShowPivotStyleColumnHeader property {#showpivotstylecolumnheader}

Indicates whether the column header in the pivot table should have the style applied.

**Type:** boolean

### PivotTable.ShowPivotStyleRowStripes property {#showpivotstylerowstripes}

Indicates whether row stripe formatting is applied.

**Type:** boolean

### PivotTable.ShowPivotStyleColumnStripes property {#showpivotstylecolumnstripes}

Indicates whether stripe formatting is applied for column.

**Type:** boolean

### PivotTable.ShowPivotStyleLastColumn property {#showpivotstylelastcolumn}

Indicates whether the column formatting is applied.

**Type:** boolean

### getHorizontalPageBreaks() {#gethorizontalpagebreaks}

### getHorizontalBreaks() {#gethorizontalbreaks}

get pivot table row index list of horizontal pagebreaks

### showInCompactForm() {#showincompactform}

Layouts the PivotTable in compact form.

### showInOutlineForm() {#showinoutlineform}

Layouts the PivotTable in outline form.

### showInTabularForm() {#showintabularform}

Layouts the PivotTable in tabular form.

### getCellByDisplayName(displayName) {#getcellbydisplayname}

Gets the Cell object by the display name of PivotField.

| Parameter | Type | Description |
| --- | --- | --- |
| displayName | String | the DisplayName of PivotField |

**Returns:** the Cell object

### getDependentPivotTables() {#getdependentpivottables}

### getChildren() {#getchildren}

Gets the Children Pivot Tables which use this PivotTable data as data source.

**Returns:** the PivotTable array object

### getSourceDataConnections() {#getsourcedataconnections}

### getNamesOfSourceDataConnections() {#getnamesofsourcedataconnections}

### changeDataSource(source) {#changedatasource}

Set pivottable's source data. Sheet1!$A$1:$C$3

### getSource() (1 of 2) {#getsource}

Get pivottable's source data.

---

### getSource(isOriginal) (2 of 2) {#getsource-1}

### refreshData() (1 of 2) {#refreshdata}

Refreshes pivottable's data and setting from it's data source.

We will gather data from data source to a pivot cache ,then calculate the data in the cache to the cells. This method is only used to gather all data to a pivot cache.

---

### refreshData(option) (2 of 2) {#refreshdata-1}

Refreshes pivottable's data and setting from it's data source with options.

| Parameter | Type | Description |
| --- | --- | --- |
| option | PivotTableRefreshOption | The options for refreshing data source of pivot table. |

### calculateData() (1 of 2) {#calculatedata}

Calculates pivottable's data to cells.

Cell.Value in the pivot range could not return the correct result if the method is not been called. This method calculates data with an inner pivot cache,not original data source. So if the data source is changed, please call RefreshData() method first.

---

### calculateData(option) (2 of 2) {#calculatedata-1}

Calculating pivot tables with options

| Parameter | Type | Description |
| --- | --- | --- |
| option | PivotTableCalculateOption |  |

### getPivotTablesWithSamePivotCache() {#getpivottableswithsamepivotcache}

### clearData() {#cleardata}

Clear PivotTable's data and formatting

If this method is not called before you add or delete PivotField, Maybe the PivotTable data is not corrected

### clearFilters() {#clearfilters}

### clearAll() {#clearall}

### calculateRange() {#calculaterange}

Calculates pivottable's range.

If this method is not been called,maybe the pivottable range is not corrected.

### formatAll(style) {#formatall}

Format all the cell in the pivottable area

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | Style which is to format |

### formatRow(row, style) {#formatrow}

Format the row data in the pivottable area

| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row Index of the Row object |
| style | Style | Style which is to format |

### format(pivotArea, style) (1 of 3) {#format}

Formats selected area of the PivotTable.

| Parameter | Type | Description |
| --- | --- | --- |
| pivotArea | PivotArea |  |
| style | Style |  |

---

### format(ca, style) (2 of 3) {#format-1}

---

### format(row, column, style) (3 of 3) {#format-2}

Format the cell in the pivottable area

| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row Index of the cell |
| column | int | Column index of the cell |
| style | Style | Style which is to format the cell |

### selectArea(ca) {#selectarea}

### showDetail(rowOffset, columnOffset, newSheet, destRow, destColumn) {#showdetail}

### setAutoGroupField(baseFieldIndex) (1 of 2) {#setautogroupfield}

Sets auto field group by the PivotTable.

baseFieldIndex - The row or column field index in the base fields NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

---

### setAutoGroupField(pivotField) (2 of 2) {#setautogroupfield-1}

Sets auto field group by the PivotTable.

NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| pivotField | PivotField | The row or column field in the specific fields |

### setManualGroupField(baseFieldIndex, startVal, endVal, groupByList, intervalNum) (1 of 4) {#setmanualgroupfield}

Sets manual field group by the PivotTable.

NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | int | The row or column field index in the base fields |
| startVal | float | Specifies the starting value for numeric grouping. |
| endVal | float | Specifies the ending value for numeric grouping. |
| groupByList | ArrayList | Specifies the grouping type list. Specified by PivotTableGroupType |
| intervalNum | float | Specifies the interval number group by numeric grouping. |

---

### setManualGroupField(pivotField, startVal, endVal, groupByList, intervalNum) (2 of 4) {#setmanualgroupfield-1}

Sets manual field group by the PivotTable.

NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| pivotField | PivotField | The row or column field in the base fields |
| startVal | float | Specifies the starting value for numeric grouping. |
| endVal | float | Specifies the ending value for numeric grouping. |
| groupByList | ArrayList | Specifies the grouping type list. Specified by PivotTableGroupType |
| intervalNum | float | Specifies the interval number group by numeric grouping. |

---

### setManualGroupField(baseFieldIndex, startVal, endVal, groupByList, intervalNum) (3 of 4) {#setmanualgroupfield-2}

Sets manual field group by the PivotTable.

NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | int | The row or column field index in the base fields |
| startVal | DateTime | Specifies the starting value for date grouping. |
| endVal | DateTime | Specifies the ending value for date grouping. |
| groupByList | ArrayList | Specifies the grouping type list. Specified by PivotTableGroupType |
| intervalNum | int | Specifies the interval number group by in days grouping.The number of days must be positive integer of nonzero |

---

### setManualGroupField(pivotField, startVal, endVal, groupByList, intervalNum) (4 of 4) {#setmanualgroupfield-3}

Sets manual field group by the PivotTable.

NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| pivotField | PivotField | The row or column field in the base fields |
| startVal | DateTime | Specifies the starting value for date grouping. |
| endVal | DateTime | Specifies the ending value for date grouping. |
| groupByList | ArrayList | Specifies the grouping type list. Specified by PivotTableGroupType |
| intervalNum | int | Specifies the interval number group by in days grouping.The number of days must be positive integer of nonzero |

### setUngroup(baseFieldIndex) (1 of 2) {#setungroup}

Sets ungroup by the PivotTable

NOTE: This method is now obsolete. Instead, please use PivotField.Ungroup() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | int | The row or column field index in the base fields |

---

### setUngroup(pivotField) (2 of 2) {#setungroup-1}

Sets ungroup by the PivotTable

NOTE: This method is now obsolete. Instead, please use PivotField.Ungroup() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| pivotField | PivotField | The row or column field in the base fields |

### dispose() {#dispose}

Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources.

### copyStyle(pivotTable) {#copystyle}

Copies named style from another pivot table.

| Parameter | Type | Description |
| --- | --- | --- |
| pivotTable | PivotTable | Source pivot table. |

### showReportFilterPage(pageField) {#showreportfilterpage}

Show all the report filter pages according to PivotField, the PivotField must be located in the PageFields.

| Parameter | Type | Description |
| --- | --- | --- |
| pageField | PivotField | The PivotField object |

### showReportFilterPageByName(fieldName) {#showreportfilterpagebyname}

Show all the report filter pages according to PivotField's name, the PivotField must be located in the PageFields.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldName | String | The name of PivotField |

### showReportFilterPageByIndex(posIndex) {#showreportfilterpagebyindex}

Show all the report filter pages according to the position index in the PageFields

| Parameter | Type | Description |
| --- | --- | --- |
| posIndex | int | The position index in the PageFields |

### removeField(fieldType, fieldName) (1 of 3) {#removefield}

Removes a field from specific field area

| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | int | A PivotFieldType value. The fields area type. |
| fieldName | String | The name in the base fields. |

---

### removeField(fieldType, baseFieldIndex) (2 of 3) {#removefield-1}

Removes a field from specific field area

| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | int | A PivotFieldType value. The fields area type. |
| baseFieldIndex | int | The field index in the base fields. |

---

### removeField(fieldType, pivotField) (3 of 3) {#removefield-2}

Remove field from specific field area

| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | int | A PivotFieldType value. the fields area type. |
| pivotField | PivotField | the field in the base fields. |

### addFieldToArea(fieldType, fieldName) (1 of 3) {#addfieldtoarea}

Adds the field to the specific area.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | int | A PivotFieldType value. The fields area type. |
| fieldName | String | The name in the base fields. |

**Returns:** The field position in the specific fields.If there is no field named as it, return -1.

---

### addFieldToArea(fieldType, baseFieldIndex) (2 of 3) {#addfieldtoarea-1}

Adds the field to the specific area.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | int | A PivotFieldType value. The fields area type. |
| baseFieldIndex | int | The field index in the base fields. |

**Returns:** The field position in the specific fields.

---

### addFieldToArea(fieldType, pivotField) (3 of 3) {#addfieldtoarea-2}

Adds the field to the specific area.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | int | A PivotFieldType value. the fields area type. |
| pivotField | PivotField | the field in the base fields. |

**Returns:** the field position in the specific fields.

### addCalculatedField(name, formula, dragToDataArea) (1 of 2) {#addcalculatedfield}

Adds a calculated field to pivot field.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the calculated field |
| formula | String | The formula of the calculated field. |
| dragToDataArea | boolean | True,drag this field to data area immediately |

---

### addCalculatedField(name, formula) (2 of 2) {#addcalculatedfield-1}

Adds a calculated field to pivot field and drag it to data area.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the calculated field |
| formula | String | The formula of the calculated field. |

### getFields(fieldType) {#getfields}

Gets the specific pivot field list by the region.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | int | A PivotFieldType value. the region type. |

**Returns:** the specific pivot field collection

### fields(fieldType) {#fields}

Gets the specific fields by the field type.

NOTE: This method is now obsolete. Instead, please use PivotField.GetFields() method. This method will be removed 12 months later since May 2024. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | int | A PivotFieldType value. the field type. |

**Returns:** the specific field collection

### getButtonArea(axisType) {#getbuttonarea}

### move(row, column) (1 of 2) {#move}

Moves the PivotTable to a different location in the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| row | int | row index. |
| column | int | column index. |

---

### move(destCellName) (2 of 2) {#move-1}

Moves the PivotTable to a different location in the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| destCellName | String | the dest cell name. |

### moveTo(row, column) (1 of 2) {#moveto}

---

### moveTo(destCellName) (2 of 2) {#moveto-1}
