---
title: Aspose::Cells::Pivot::PivotTable class
linktitle: PivotTable
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Pivot::PivotTable class. Summary description for PivotTable in C++.'
type: docs
weight: 1800
url: /cpp/aspose.cells.pivot/pivottable/
---
## PivotTable class


Summary description for [PivotTable](./).

```cpp
class PivotTable
```

## Methods

| Method | Description |
| --- | --- |
| [AddCalculatedField(const U16String\& name, const U16String\& formula, bool dragToDataArea)](./addcalculatedfield/) | Adds a calculated field to pivot field. |
| [AddCalculatedField(const char16_t* name, const char16_t* formula, bool dragToDataArea)](./addcalculatedfield/) | Adds a calculated field to pivot field. |
| [AddCalculatedField(const U16String\& name, const U16String\& formula)](./addcalculatedfield/) | Adds a calculated field to pivot field and drag it to data area. |
| [AddCalculatedField(const char16_t* name, const char16_t* formula)](./addcalculatedfield/) | Adds a calculated field to pivot field and drag it to data area. |
| [AddFieldToArea(PivotFieldType fieldType, const U16String\& fieldName)](./addfieldtoarea/) | Adds the field to the specific area. |
| [AddFieldToArea(PivotFieldType fieldType, const char16_t* fieldName)](./addfieldtoarea/) | Adds the field to the specific area. |
| [AddFieldToArea(PivotFieldType fieldType, int32_t baseFieldIndex)](./addfieldtoarea/) | Adds the field to the specific area. |
| [AddFieldToArea(PivotFieldType fieldType, const PivotField\& pivotField)](./addfieldtoarea/) | Adds the field to the specific area. |
| [CalculateData()](./calculatedata/) | Calculates pivottable's data to cells. |
| [CalculateRange()](./calculaterange/) | Calculates pivottable's range. |
| [ChangeDataSource(const Vector \<U16String\>\& source)](./changedatasource/) | Set pivottable's source data. Sheet1!$A$1:$C$3. |
| [ClearData()](./cleardata/) | Clear [PivotTable](./)'s data and formatting. |
| [CopyStyle(const PivotTable\& pivotTable)](./copystyle/) | Copies named style from another pivot table. |
| [Dispose()](./dispose/) | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [Fields(PivotFieldType fieldType)](./fields/) | Gets the specific fields by the field type. |
| [Format(const PivotArea\& pivotArea, const Style\& style)](./format/) | Formats selected area of the [PivotTable](./). |
| [Format(int32_t row, int32_t column, const Style\& style)](./format/) | Format the cell in the pivottable area. |
| [FormatAll(const Style\& style)](./formatall/) | Format all the cell in the pivottable area. |
| [FormatRow(int32_t row, const Style\& style)](./formatrow/) | Format the row data in the pivottable area. |
| [GetAltTextDescription()](./getalttextdescription/) | Gets the description of the alt text. |
| [GetAltTextTitle()](./getalttexttitle/) | Gets the title of the altertext. |
| [GetAutofitColumnWidthOnUpdate()](./getautofitcolumnwidthonupdate/) | Indicates whether autofitting column width on update. |
| [GetAutoFormatType()](./getautoformattype/) | Gets the [PivotTable](./) auto format type. |
| [GetBaseFields()](./getbasefields/) | Returns a PivotFields object that includes all fields in the [PivotTable](./) report. |
| [GetCellByDisplayName(const U16String\& displayName)](./getcellbydisplayname/) | Gets the [Cell](../../aspose.cells/cell/) object by the display name of [PivotField](../pivotfield/). |
| [GetCellByDisplayName(const char16_t* displayName)](./getcellbydisplayname/) | Gets the [Cell](../../aspose.cells/cell/) object by the display name of [PivotField](../pivotfield/). |
| [GetChildren()](./getchildren/) | Gets the Children [Pivot](../)[Tables](../../aspose.cells.tables/) which use this [PivotTable](./) data as data source. |
| [GetColumnFields()](./getcolumnfields/) | Returns a PivotFields object that are currently shown as column fields. |
| [GetColumnGrand()](./getcolumngrand/) | Indicates whether the [PivotTable](./) report shows grand totals for columns. |
| [GetColumnHeaderCaption()](./getcolumnheadercaption/) | Gets the [Column](../../aspose.cells/column/) Header Caption of the [PivotTable](./). |
| [GetColumnRange()](./getcolumnrange/) | Returns a [CellArea](../../aspose.cells/cellarea/) object that represents the range that contains the column area in the [PivotTable](./) report. Read-only. |
| [GetCustomListSort()](./getcustomlistsort/) | Indicates whether consider built-in custom list when sort data. |
| [GetDataBodyRange()](./getdatabodyrange/) | Returns a [CellArea](../../aspose.cells/cellarea/) object that represents the range that contains the data area in the list between the header row and the insert row. Read-only. |
| [GetDataField()](./getdatafield/) | Gets a [PivotField](../pivotfield/) object that represents all the data fields in a [PivotTable](./). Read-only.It would be init only when there are two or more data fields in the DataPiovtFiels. It only use to add DataPivotField to the [PivotTable](./) row/column area . Default is in row area. |
| [GetDataFieldHeaderName()](./getdatafieldheadername/) | Gets and sets the name of the value area field header in the [PivotTable](./). |
| [GetDataFields()](./getdatafields/) | Gets a [PivotField](../pivotfield/) object that represents all the data fields in a [PivotTable](./). Read-only.It would be init only when there are two or more data fields in the DataPiovtFiels. It only use to add DataPivotField to the [PivotTable](./) row/column area . Default is in row area. |
| [GetDataSource()](./getdatasource/) | Gets and sets the data source of the pivot table. |
| [GetDisplayErrorString()](./getdisplayerrorstring/) | Indicates whether the [PivotTable](./) report displays a custom string in cells that contain errors. |
| [GetDisplayImmediateItems()](./getdisplayimmediateitems/) | Indicates whether items in the row and column areas are visible when the data area of the [PivotTable](./) is empty. The default value is true. |
| [GetDisplayNullString()](./getdisplaynullstring/) | Indicates whether the [PivotTable](./) report displays a custom string in cells that contain null values. |
| [GetEnableDataValueEditing()](./getenabledatavalueediting/) | Specifies a boolean value that indicates whether the user is allowed to edit the cells in the data area of the pivottable. Enable cell editing in the values area. |
| [GetEnableDrilldown()](./getenabledrilldown/) | Gets whether drilldown is enabled. |
| [GetEnableFieldDialog()](./getenablefielddialog/) | Indicates whether the [PivotTable](./) Field dialog box is available when the user double-clicks the [PivotTable](./) field. |
| [GetEnableFieldList()](./getenablefieldlist/) | Gets whether enable the field list for the [PivotTable](./). |
| [GetEnableWizard()](./getenablewizard/) | Indicates whether the [PivotTable](./) Wizard is available. |
| [GetErrorString()](./geterrorstring/) | Gets the string displayed in cells that contain errors when the DisplayErrorString property is true.The default value is an empty string. |
| [GetExternalConnectionDataSource()](./getexternalconnectiondatasource/) | Gets the external connection data source. |
| [GetFieldListSortAscending()](./getfieldlistsortascending/) | Specifies a boolean value that indicates whether fields in the [PivotTable](./) are sorted in non-default order in the field list. |
| [GetGrandTotalName()](./getgrandtotalname/) | Returns the text string label that is displayed in the grand total column or row heading. The default value is the string "Grand Total". |
| [GetHasBlankRows()](./gethasblankrows/) | Indicates whether to add blank rows. This property only applies for the [PivotTable](./) auto format types which needs to add blank rows. |
| [GetIndent()](./getindent/) | Specifies the indentation increment for compact axis and can be used to set the Report Layout to Compact Form. |
| [GetItemPrintTitles()](./getitemprinttitles/) | A bit that specifies whether pivot item captions on the row axis are repeated on each printed page for pivot fields in tabular form. |
| [GetManualUpdate()](./getmanualupdate/) | Indicates whether the [PivotTable](./) report is recalculated only at the user's request. |
| [GetMergeLabels()](./getmergelabels/) | Indicates whether the specified [PivotTable](./) report's outer-row item, column item, subtotal, and grand total labels use merged cells. |
| [GetMissingItemsLimit()](./getmissingitemslimit/) | Specifies a boolean value that indicates whether the fields of a [PivotTable](./) can have multiple filters set on them. |
| [GetName()](./getname/) | Gets the name of the [PivotTable](./). |
| [GetNullString()](./getnullstring/) | Gets the string displayed in cells that contain null values when the DisplayNullString property is true.The default value is an empty string. |
| [GetPageFieldOrder()](./getpagefieldorder/) | Gets the order in which page fields are added to the [PivotTable](./) report's layout. |
| [GetPageFields()](./getpagefields/) | Returns a PivotFields object that are currently shown as page fields. |
| [GetPageFieldWrapCount()](./getpagefieldwrapcount/) | Gets the number of page fields in each column or row in the [PivotTable](./) report. |
| [GetPivotFilters()](./getpivotfilters/) | Returns a [PivotFilterCollection](../pivotfiltercollection/) object. |
| [GetPivotFormatConditions()](./getpivotformatconditions/) | Gets the Format Conditions of the pivot table. |
| [GetPivotFormats()](./getpivotformats/) | Gets the collection of formats applied to [PivotTable](./). |
| [GetPivotTableStyleName()](./getpivottablestylename/) | Gets and sets the pivottable style name. |
| [GetPivotTableStyleType()](./getpivottablestyletype/) | Gets and sets the built-in pivot table style. |
| [GetPreserveFormatting()](./getpreserveformatting/) | Indicates whether formatting is preserved when the [PivotTable](./) is refreshed or recalculated. |
| [GetPrintDrill()](./getprintdrill/) | Specifies a boolean value that indicates whether drill indicators should be printed. print expand/collapse buttons when displayed on pivottable. |
| [GetPrintTitles()](./getprinttitles/) | Indicates whether the print titles for the worksheet are set based on the [PivotTable](./) report. The default value is false. |
| [GetRefreshDataFlag()](./getrefreshdataflag/) | Indicates whether Refreshing Data or not. |
| [GetRefreshDataOnOpeningFile()](./getrefreshdataonopeningfile/) | Indicates whether Refresh Data when Opening File. |
| [GetRefreshDate()](./getrefreshdate/) | Gets the date when the [PivotTable](./) was last refreshed. |
| [GetRefreshedByWho()](./getrefreshedbywho/) | Gets the name of the user who last refreshed the [PivotTable](./). |
| [GetRowFields()](./getrowfields/) | Returns a PivotFields object that are currently shown as row fields. |
| [GetRowGrand()](./getrowgrand/) | Indicates whether the [PivotTable](./) report shows grand totals for rows. |
| [GetRowHeaderCaption()](./getrowheadercaption/) | Gets the [Row](../../aspose.cells/row/) Header Caption of the [PivotTable](./). |
| [GetRowRange()](./getrowrange/) | Returns a [CellArea](../../aspose.cells/cellarea/) object that represents the range that contains the row area in the [PivotTable](./) report. Read-only. |
| [GetSaveData()](./getsavedata/) | Indicates whether data for the [PivotTable](./) report is saved with the workbook. |
| [GetShowDataTips()](./getshowdatatips/) | Specifies a boolean value that indicates whether tooltips should be displayed for [PivotTable](./) data cells. |
| [GetShowDrill()](./getshowdrill/) | Gets whether expand/collapse buttons is shown. |
| [GetShowEmptyCol()](./getshowemptycol/) | Specifies a boolean value that indicates whether to include empty columns in the table. |
| [GetShowEmptyRow()](./getshowemptyrow/) | Specifies a boolean value that indicates whether to include empty rows in the table. |
| [GetShowMemberPropertyTips()](./getshowmemberpropertytips/) | Specifies a boolean value that indicates whether member property information should be omitted from [PivotTable](./) tooltips. |
| [GetShowPivotStyleColumnHeader()](./getshowpivotstylecolumnheader/) | Indicates whether the column header in the pivot table should have the style applied. |
| [GetShowPivotStyleColumnStripes()](./getshowpivotstylecolumnstripes/) | Indicates whether column stripe formatting is applied. |
| [GetShowPivotStyleLastColumn()](./getshowpivotstylelastcolumn/) | Indicates whether column stripe formatting is applied. |
| [GetShowPivotStyleRowHeader()](./getshowpivotstylerowheader/) | Indicates whether the row header in the pivot table should have the style applied. |
| [GetShowPivotStyleRowStripes()](./getshowpivotstylerowstripes/) | Indicates whether row stripe formatting is applied. |
| [GetShowRowHeaderCaption()](./getshowrowheadercaption/) | Indicates whether row header caption is shown in the [PivotTable](./) report Indicates whether Display field captions and filter drop downs. |
| [GetShowValuesRow()](./getshowvaluesrow/) | Specifies a boolean value that indicates whether show values row. show the values row. |
| [GetSource()](./getsource/) | Get pivottable's source data. |
| [GetSubtotalHiddenPageItems()](./getsubtotalhiddenpageitems/) | Indicates whether hidden page field items in the [PivotTable](./) report are included in row and column subtotals, block totals, and grand totals. The default value is False. |
| [GetTableRange1()](./gettablerange1/) | Returns a [CellArea](../../aspose.cells/cellarea/) object that represents the range containing the entire [PivotTable](./) report, but doesn't include page fields. Read-only. |
| [GetTableRange2()](./gettablerange2/) | Returns a [CellArea](../../aspose.cells/cellarea/) object that represents the range containing the entire [PivotTable](./) report, includes page fields. Read-only. |
| [GetTag()](./gettag/) | Gets a string saved with the [PivotTable](./) report. |
| [IsAutoFormat()](./isautoformat/) | Indicates whether the [PivotTable](./) report is automatically formatted. Checkbox "autoformat table " which is in pivottable option for Excel 2003. |
| [IsExcel2003Compatible()](./isexcel2003compatible/) | Specifies whether the [PivotTable](./) is compatible for Excel2003 when refreshing [PivotTable](./), if true, a string must be less than or equal to 255 characters, so if the string is greater than 255 characters, it will be truncated. if false, a string will not have the aforementioned restriction. The default value is true. |
| [IsGridDropZones()](./isgriddropzones/) | Indicates whether the [PivotTable](./) report displays classic pivottable layout. (enables dragging fields in the grid) |
| [IsMultipleFieldFilters()](./ismultiplefieldfilters/) | Specifies a boolean value that indicates whether the fields of a [PivotTable](./) can have multiple filters set on them. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsSelected()](./isselected/) | Indicates whether the [PivotTable](./) is selected. |
| [Move(int32_t row, int32_t column)](./move/) | Moves the [PivotTable](./) to a different location in the worksheet. |
| [Move(const U16String\& destCellName)](./move/) | Moves the [PivotTable](./) to a different location in the worksheet. |
| [Move(const char16_t* destCellName)](./move/) | Moves the [PivotTable](./) to a different location in the worksheet. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const PivotTable\& src)](./operator_asm/) | operator= |
| [PivotTable(PivotTable_Impl* impl)](./pivottable/) | Constructs from an implementation object. |
| [PivotTable(const PivotTable\& src)](./pivottable/) | Copy constructor. |
| [RefreshData()](./refreshdata/) | Refreshes pivottable's data and setting from it's data source. |
| [RemoveField(PivotFieldType fieldType, const U16String\& fieldName)](./removefield/) | Removes a field from specific field area. |
| [RemoveField(PivotFieldType fieldType, const char16_t* fieldName)](./removefield/) | Removes a field from specific field area. |
| [RemoveField(PivotFieldType fieldType, int32_t baseFieldIndex)](./removefield/) | Removes a field from specific field area. |
| [RemoveField(PivotFieldType fieldType, const PivotField\& pivotField)](./removefield/) | Remove field from specific field area. |
| [SetAltTextDescription(const U16String\& value)](./setalttextdescription/) | Gets the description of the alt text. |
| [SetAltTextDescription(const char16_t* value)](./setalttextdescription/) | Gets the description of the alt text. |
| [SetAltTextTitle(const U16String\& value)](./setalttexttitle/) | Gets the title of the altertext. |
| [SetAltTextTitle(const char16_t* value)](./setalttexttitle/) | Gets the title of the altertext. |
| [SetAutofitColumnWidthOnUpdate(bool value)](./setautofitcolumnwidthonupdate/) | Indicates whether autofitting column width on update. |
| [SetAutoFormatType(PivotTableAutoFormatType value)](./setautoformattype/) | Gets the [PivotTable](./) auto format type. |
| [SetColumnGrand(bool value)](./setcolumngrand/) | Indicates whether the [PivotTable](./) report shows grand totals for columns. |
| [SetColumnHeaderCaption(const U16String\& value)](./setcolumnheadercaption/) | Gets the [Column](../../aspose.cells/column/) Header Caption of the [PivotTable](./). |
| [SetColumnHeaderCaption(const char16_t* value)](./setcolumnheadercaption/) | Gets the [Column](../../aspose.cells/column/) Header Caption of the [PivotTable](./). |
| [SetCustomListSort(bool value)](./setcustomlistsort/) | Indicates whether consider built-in custom list when sort data. |
| [SetDataFieldHeaderName(const U16String\& value)](./setdatafieldheadername/) | Gets and sets the name of the value area field header in the [PivotTable](./). |
| [SetDataFieldHeaderName(const char16_t* value)](./setdatafieldheadername/) | Gets and sets the name of the value area field header in the [PivotTable](./). |
| [SetDataSource(const Vector \<U16String\>\& value)](./setdatasource/) | Gets and sets the data source of the pivot table. |
| [SetDisplayErrorString(bool value)](./setdisplayerrorstring/) | Indicates whether the [PivotTable](./) report displays a custom string in cells that contain errors. |
| [SetDisplayImmediateItems(bool value)](./setdisplayimmediateitems/) | Indicates whether items in the row and column areas are visible when the data area of the [PivotTable](./) is empty. The default value is true. |
| [SetDisplayNullString(bool value)](./setdisplaynullstring/) | Indicates whether the [PivotTable](./) report displays a custom string in cells that contain null values. |
| [SetEnableDataValueEditing(bool value)](./setenabledatavalueediting/) | Specifies a boolean value that indicates whether the user is allowed to edit the cells in the data area of the pivottable. Enable cell editing in the values area. |
| [SetEnableDrilldown(bool value)](./setenabledrilldown/) | Gets whether drilldown is enabled. |
| [SetEnableFieldDialog(bool value)](./setenablefielddialog/) | Indicates whether the [PivotTable](./) Field dialog box is available when the user double-clicks the [PivotTable](./) field. |
| [SetEnableFieldList(bool value)](./setenablefieldlist/) | Gets whether enable the field list for the [PivotTable](./). |
| [SetEnableWizard(bool value)](./setenablewizard/) | Indicates whether the [PivotTable](./) Wizard is available. |
| [SetErrorString(const U16String\& value)](./seterrorstring/) | Gets the string displayed in cells that contain errors when the DisplayErrorString property is true.The default value is an empty string. |
| [SetErrorString(const char16_t* value)](./seterrorstring/) | Gets the string displayed in cells that contain errors when the DisplayErrorString property is true.The default value is an empty string. |
| [SetFieldListSortAscending(bool value)](./setfieldlistsortascending/) | Specifies a boolean value that indicates whether fields in the [PivotTable](./) are sorted in non-default order in the field list. |
| [SetGrandTotalName(const U16String\& value)](./setgrandtotalname/) | Returns the text string label that is displayed in the grand total column or row heading. The default value is the string "Grand Total". |
| [SetGrandTotalName(const char16_t* value)](./setgrandtotalname/) | Returns the text string label that is displayed in the grand total column or row heading. The default value is the string "Grand Total". |
| [SetHasBlankRows(bool value)](./sethasblankrows/) | Indicates whether to add blank rows. This property only applies for the [PivotTable](./) auto format types which needs to add blank rows. |
| [SetIndent(int32_t value)](./setindent/) | Specifies the indentation increment for compact axis and can be used to set the Report Layout to Compact Form. |
| [SetIsAutoFormat(bool value)](./setisautoformat/) | Indicates whether the [PivotTable](./) report is automatically formatted. Checkbox "autoformat table " which is in pivottable option for Excel 2003. |
| [SetIsExcel2003Compatible(bool value)](./setisexcel2003compatible/) | Specifies whether the [PivotTable](./) is compatible for Excel2003 when refreshing [PivotTable](./), if true, a string must be less than or equal to 255 characters, so if the string is greater than 255 characters, it will be truncated. if false, a string will not have the aforementioned restriction. The default value is true. |
| [SetIsGridDropZones(bool value)](./setisgriddropzones/) | Indicates whether the [PivotTable](./) report displays classic pivottable layout. (enables dragging fields in the grid) |
| [SetIsMultipleFieldFilters(bool value)](./setismultiplefieldfilters/) | Specifies a boolean value that indicates whether the fields of a [PivotTable](./) can have multiple filters set on them. |
| [SetIsSelected(bool value)](./setisselected/) | Indicates whether the [PivotTable](./) is selected. |
| [SetItemPrintTitles(bool value)](./setitemprinttitles/) | A bit that specifies whether pivot item captions on the row axis are repeated on each printed page for pivot fields in tabular form. |
| [SetManualUpdate(bool value)](./setmanualupdate/) | Indicates whether the [PivotTable](./) report is recalculated only at the user's request. |
| [SetMergeLabels(bool value)](./setmergelabels/) | Indicates whether the specified [PivotTable](./) report's outer-row item, column item, subtotal, and grand total labels use merged cells. |
| [SetMissingItemsLimit(PivotMissingItemLimitType value)](./setmissingitemslimit/) | Specifies a boolean value that indicates whether the fields of a [PivotTable](./) can have multiple filters set on them. |
| [SetName(const U16String\& value)](./setname/) | Gets the name of the [PivotTable](./). |
| [SetName(const char16_t* value)](./setname/) | Gets the name of the [PivotTable](./). |
| [SetNullString(const U16String\& value)](./setnullstring/) | Gets the string displayed in cells that contain null values when the DisplayNullString property is true.The default value is an empty string. |
| [SetNullString(const char16_t* value)](./setnullstring/) | Gets the string displayed in cells that contain null values when the DisplayNullString property is true.The default value is an empty string. |
| [SetPageFieldOrder(PrintOrderType value)](./setpagefieldorder/) | Gets the order in which page fields are added to the [PivotTable](./) report's layout. |
| [SetPageFieldWrapCount(int32_t value)](./setpagefieldwrapcount/) | Gets the number of page fields in each column or row in the [PivotTable](./) report. |
| [SetPivotTableStyleName(const U16String\& value)](./setpivottablestylename/) | Gets and sets the pivottable style name. |
| [SetPivotTableStyleName(const char16_t* value)](./setpivottablestylename/) | Gets and sets the pivottable style name. |
| [SetPivotTableStyleType(PivotTableStyleType value)](./setpivottablestyletype/) | Gets and sets the built-in pivot table style. |
| [SetPreserveFormatting(bool value)](./setpreserveformatting/) | Indicates whether formatting is preserved when the [PivotTable](./) is refreshed or recalculated. |
| [SetPrintDrill(bool value)](./setprintdrill/) | Specifies a boolean value that indicates whether drill indicators should be printed. print expand/collapse buttons when displayed on pivottable. |
| [SetPrintTitles(bool value)](./setprinttitles/) | Indicates whether the print titles for the worksheet are set based on the [PivotTable](./) report. The default value is false. |
| [SetRefreshDataFlag(bool value)](./setrefreshdataflag/) | Indicates whether Refreshing Data or not. |
| [SetRefreshDataOnOpeningFile(bool value)](./setrefreshdataonopeningfile/) | Indicates whether Refresh Data when Opening File. |
| [SetRowGrand(bool value)](./setrowgrand/) | Indicates whether the [PivotTable](./) report shows grand totals for rows. |
| [SetRowHeaderCaption(const U16String\& value)](./setrowheadercaption/) | Gets the [Row](../../aspose.cells/row/) Header Caption of the [PivotTable](./). |
| [SetRowHeaderCaption(const char16_t* value)](./setrowheadercaption/) | Gets the [Row](../../aspose.cells/row/) Header Caption of the [PivotTable](./). |
| [SetSaveData(bool value)](./setsavedata/) | Indicates whether data for the [PivotTable](./) report is saved with the workbook. |
| [SetShowDataTips(bool value)](./setshowdatatips/) | Specifies a boolean value that indicates whether tooltips should be displayed for [PivotTable](./) data cells. |
| [SetShowDrill(bool value)](./setshowdrill/) | Gets whether expand/collapse buttons is shown. |
| [SetShowEmptyCol(bool value)](./setshowemptycol/) | Specifies a boolean value that indicates whether to include empty columns in the table. |
| [SetShowEmptyRow(bool value)](./setshowemptyrow/) | Specifies a boolean value that indicates whether to include empty rows in the table. |
| [SetShowMemberPropertyTips(bool value)](./setshowmemberpropertytips/) | Specifies a boolean value that indicates whether member property information should be omitted from [PivotTable](./) tooltips. |
| [SetShowPivotStyleColumnHeader(bool value)](./setshowpivotstylecolumnheader/) | Indicates whether the column header in the pivot table should have the style applied. |
| [SetShowPivotStyleColumnStripes(bool value)](./setshowpivotstylecolumnstripes/) | Indicates whether column stripe formatting is applied. |
| [SetShowPivotStyleLastColumn(bool value)](./setshowpivotstylelastcolumn/) | Indicates whether column stripe formatting is applied. |
| [SetShowPivotStyleRowHeader(bool value)](./setshowpivotstylerowheader/) | Indicates whether the row header in the pivot table should have the style applied. |
| [SetShowPivotStyleRowStripes(bool value)](./setshowpivotstylerowstripes/) | Indicates whether row stripe formatting is applied. |
| [SetShowRowHeaderCaption(bool value)](./setshowrowheadercaption/) | Indicates whether row header caption is shown in the [PivotTable](./) report Indicates whether Display field captions and filter drop downs. |
| [SetShowValuesRow(bool value)](./setshowvaluesrow/) | Specifies a boolean value that indicates whether show values row. show the values row. |
| [SetSubtotalHiddenPageItems(bool value)](./setsubtotalhiddenpageitems/) | Indicates whether hidden page field items in the [PivotTable](./) report are included in row and column subtotals, block totals, and grand totals. The default value is False. |
| [SetTag(const U16String\& value)](./settag/) | Gets a string saved with the [PivotTable](./) report. |
| [SetTag(const char16_t* value)](./settag/) | Gets a string saved with the [PivotTable](./) report. |
| [ShowInCompactForm()](./showincompactform/) | Layouts the [PivotTable](./) in compact form. |
| [ShowInOutlineForm()](./showinoutlineform/) | Layouts the [PivotTable](./) in outline form. |
| [ShowInTabularForm()](./showintabularform/) | Layouts the [PivotTable](./) in tabular form. |
| [ShowReportFilterPage(const PivotField\& pageField)](./showreportfilterpage/) | Show all the report filter pages according to [PivotField](../pivotfield/), the [PivotField](../pivotfield/) must be located in the PageFields. |
| [ShowReportFilterPageByIndex(int32_t posIndex)](./showreportfilterpagebyindex/) | Show all the report filter pages according to the position index in the PageFields. |
| [ShowReportFilterPageByName(const U16String\& fieldName)](./showreportfilterpagebyname/) | Show all the report filter pages according to [PivotField](../pivotfield/)'s name, the [PivotField](../pivotfield/) must be located in the PageFields. |
| [ShowReportFilterPageByName(const char16_t* fieldName)](./showreportfilterpagebyname/) | Show all the report filter pages according to [PivotField](../pivotfield/)'s name, the [PivotField](../pivotfield/) must be located in the PageFields. |
| [~PivotTable()](./~pivottable/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
Workbook book;
Worksheet sheet = book.GetWorksheets().Get(0);
Cells cells = sheet.GetCells();
cells.Get(0, 0).PutValue(u"fruit");
cells.Get(1, 0).PutValue(u"grape");
cells.Get(2, 0).PutValue(u"blueberry");
cells.Get(3, 0).PutValue(u"kiwi");
cells.Get(4, 0).PutValue(u"cherry");
cells.Get(5, 0).PutValue(u"grape");
cells.Get(6, 0).PutValue(u"blueberry");
cells.Get(7, 0).PutValue(u"kiwi");
cells.Get(8, 0).PutValue(u"cherry");

cells.Get(0, 1).PutValue(u"year");
cells.Get(1, 1).PutValue(2020);
cells.Get(2, 1).PutValue(2020);
cells.Get(3, 1).PutValue(2020);
cells.Get(4, 1).PutValue(2020);
cells.Get(5, 1).PutValue(2021);
cells.Get(6, 1).PutValue(2021);
cells.Get(7, 1).PutValue(2021);
cells.Get(8, 1).PutValue(2021);

cells.Get(0, 2).PutValue(u"amount");
cells.Get(1, 2).PutValue(50);
cells.Get(2, 2).PutValue(60);
cells.Get(3, 2).PutValue(70);
cells.Get(4, 2).PutValue(80);
cells.Get(5, 2).PutValue(90);
cells.Get(6, 2).PutValue(100);
cells.Get(7, 2).PutValue(110);
cells.Get(8, 2).PutValue(120);

PivotTableCollection pivots = sheet.GetPivotTables();

int pivotIndex = pivots.Add(u"=Sheet1!A1:C9", u"A12", u"TestPivotTable");
PivotTable pivot = pivots.Get(pivotIndex);
pivot.AddFieldToArea(PivotFieldType::Row, u"fruit");
pivot.AddFieldToArea(PivotFieldType::Column, u"year");
pivot.AddFieldToArea(PivotFieldType::Data, u"amount");

pivot.SetPivotTableStyleType(PivotTableStyleType::PivotTableStyleMedium10);

//Change PivotField's attributes
PivotField rowField = pivot.GetRowFields().Get(0);
rowField.SetDisplayName(u"custom display name");

//Add PivotFilter
int index = pivot.GetPivotFilters().Add(0, PivotFilterType::Count);
PivotFilter filter = pivot.GetPivotFilters().Get(index);
filter.GetAutoFilter().FilterTop10(0, false, false, 2);

//Add PivotFormatCondition
int formatIndex = pivot.GetPivotFormatConditions().Add();
PivotFormatCondition pfc = pivot.GetPivotFormatConditions().Get(formatIndex);
FormatConditionCollection fcc = pfc.GetFormatConditions();
fcc.AddArea(pivot.GetDataBodyRange());
int idx = fcc.AddCondition(FormatConditionType::CellValue);
FormatCondition fc = fcc.Get(idx);
fc.SetFormula1(u"100");
fc.SetOperator(OperatorType::GreaterOrEqual);
fc.GetStyle().SetBackgroundColor(Color{ 0xff, 0xff, 0, 0 });//Red

pivot.RefreshData();
pivot.CalculateData();


book.Save("out.xlsx");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Pivot](../)
* Library [Aspose.Cells for C++](../../)
