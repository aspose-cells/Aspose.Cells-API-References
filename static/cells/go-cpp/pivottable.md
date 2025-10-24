##PivotTable Class
'PivotTable class. Encapsulates the object that represents pivottable in Go.'
## PivotTable class
Summary description for PivotTable.
```go
type PivotTable struct  {
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
|[IsExcel2003Compatible](./isexcel2003compatible/) | Specifies whether the PivotTable is compatible for Excel2003 when refreshing PivotTable,if true, a string must be less than or equal to 255 characters, so if the string is greater than 255 characters,it will be truncated. if false, a string will not have the aforementioned restriction.The default value is true. |
|[SetIsExcel2003Compatible](./setisexcel2003compatible/) | Specifies whether the PivotTable is compatible for Excel2003 when refreshing PivotTable,if true, a string must be less than or equal to 255 characters, so if the string is greater than 255 characters,it will be truncated. if false, a string will not have the aforementioned restriction.The default value is true. |
|[GetRefreshedByWho](./getrefreshedbywho/) | Gets the name of the last user who refreshed this PivotTable |
|[GetRefreshDate](./getrefreshdate/) | Gets the last date time when the PivotTable was refreshed. |
|[GetPivotTableStyleName](./getpivottablestylename/) | Gets and sets the pivottable style name. |
|[SetPivotTableStyleName](./setpivottablestylename/) | Gets and sets the pivottable style name. |
|[GetPivotTableStyleType](./getpivottablestyletype/) | Gets and sets the built-in pivot table style. |
|[SetPivotTableStyleType](./setpivottablestyletype/) | Gets and sets the built-in pivot table style. |
|[CopyStyle](./copystyle/) | Copies named style from another pivot table. |
|[ShowReportFilterPage](./showreportfilterpage/) | Show all the report filter pages according to PivotField, the PivotField must be located in the PageFields. |
|[ShowReportFilterPageByName](./showreportfilterpagebyname/) | Show all the report filter pages according to PivotField's name, the PivotField must be located in the PageFields. |
|[ShowReportFilterPageByIndex](./showreportfilterpagebyindex/) | Show all the report filter pages according to the position index in the PageFields |
|[RemoveField_PivotFieldType_String](./removefield_pivotfieldtype_string/) | Removes a field from specific field area |
|[RemoveField_PivotFieldType_Int](./removefield_pivotfieldtype_int/) | Removes a field from specific field area |
|[RemoveField_PivotFieldType_PivotField](./removefield_pivotfieldtype_pivotfield/) | Remove field from specific field area |
|[AddFieldToArea_PivotFieldType_String](./addfieldtoarea_pivotfieldtype_string/) | Adds the field to the specific area. |
|[AddFieldToArea_PivotFieldType_Int](./addfieldtoarea_pivotfieldtype_int/) | Adds the field to the specific area. |
|[AddFieldToArea_PivotFieldType_PivotField](./addfieldtoarea_pivotfieldtype_pivotfield/) | Adds the field to the specific area. |
|[AddCalculatedField_String_String_Bool](./addcalculatedfield_string_string_bool/) | Adds a calculated field to pivot field. |
|[AddCalculatedField_String_String](./addcalculatedfield_string_string/) | Adds a calculated field to pivot field and drag it to data area. |
|[GetFields](./getfields/) | Gets the specific pivot field list by the region. |
|[GetColumnFields](./getcolumnfields/) | Returns a PivotFields object that are currently shown as column fields. |
|[GetRowFields](./getrowfields/) | Returns a PivotFields object that are currently shown as row fields. |
|[GetPageFields](./getpagefields/) | Returns a PivotFields object that are currently shown as page fields. |
|[GetDataFields](./getdatafields/) | Gets a PivotField object that represents all the data fields in a PivotTable.Read-only.It would be init only when there are two or more data fields in the DataPiovtFiels.It only use to add DataPivotField to the PivotTable row/column area . Default is in row area. |
|[GetDataField](./getdatafield/) | Gets a PivotField object that represents all the data fields in a PivotTable.Read-only.It would only be created when there are two or more data fields in the Data region.Defaultly it is in row region. You can drag it to the row/column region with PivotTable.AddFieldToArea() method . |
|[GetBaseFields](./getbasefields/) | Returns all base pivot fields in the PivotTable. |
|[GetPivotFilters](./getpivotfilters/) | Returns all filters of pivot fields in the pivot table. |
|[GetColumnRange](./getcolumnrange/) | Returns a CellArea object that represents the rangethat contains the column area in the PivotTable report. Read-only. |
|[GetRowRange](./getrowrange/) | Returns a CellArea object that represents the rangethat contains the row area in the PivotTable report. Read-only. |
|[GetDataBodyRange](./getdatabodyrange/) | Returns a CellArea object that represents the range that contains the data areain the list between the header row and the insert row. Read-only. |
|[GetTableRange1](./gettablerange1/) | Returns a CellArea object that represents the range containing the entire PivotTable report,but doesn't include page fields. Read-only. |
|[GetTableRange2](./gettablerange2/) | Returns a CellArea object that represents the range containing the entire PivotTable report,includes page fields. Read-only. |
|[MoveTo_Int_Int](./moveto_int_int/) | Moves the PivotTable to a different location in the worksheet. |
|[MoveTo_String](./moveto_string/) | Moves the PivotTable to a different location in the worksheet. |
|[IsGridDropZones](./isgriddropzones/) | Indicates whether the PivotTable report displays classic pivottable layout.(enables dragging fields in the grid) |
|[SetIsGridDropZones](./setisgriddropzones/) | Indicates whether the PivotTable report displays classic pivottable layout.(enables dragging fields in the grid) |
|[GetShowColumnGrandTotals](./getshowcolumngrandtotals/) | Indicates whether to show grand totals for columns of this pivot table. |
|[SetShowColumnGrandTotals](./setshowcolumngrandtotals/) | Indicates whether to show grand totals for columns of this pivot table. |
|[GetShowRowGrandTotals](./getshowrowgrandtotals/) | Indicates whether to show grand totals for rows of the pivot table. |
|[SetShowRowGrandTotals](./setshowrowgrandtotals/) | Indicates whether to show grand totals for rows of the pivot table. |
|[GetDisplayNullString](./getdisplaynullstring/) | Indicates whether the PivotTable report displays a custom string if the value is null. |
|[SetDisplayNullString](./setdisplaynullstring/) | Indicates whether the PivotTable report displays a custom string if the value is null. |
|[GetNullString](./getnullstring/) | Gets the string displayed in cells that contain null valueswhen the DisplayNullString property is true.The default value is an empty string. |
|[SetNullString](./setnullstring/) | Gets the string displayed in cells that contain null valueswhen the DisplayNullString property is true.The default value is an empty string. |
|[GetDisplayErrorString](./getdisplayerrorstring/) | Indicates whether the PivotTable report displays a custom string in cells that contain errors. |
|[SetDisplayErrorString](./setdisplayerrorstring/) | Indicates whether the PivotTable report displays a custom string in cells that contain errors. |
|[GetDataFieldHeaderName](./getdatafieldheadername/) | Gets and sets the name of the value area field header in the PivotTable. |
|[SetDataFieldHeaderName](./setdatafieldheadername/) | Gets and sets the name of the value area field header in the PivotTable. |
|[GetErrorString](./geterrorstring/) | Gets the string displayed in cells that contain errorswhen the DisplayErrorString property is true.The default value is an empty string. |
|[SetErrorString](./seterrorstring/) | Gets the string displayed in cells that contain errorswhen the DisplayErrorString property is true.The default value is an empty string. |
|[IsAutoFormat](./isautoformat/) | Indicates whether the PivotTable report is automatically formatted.Checkbox "autoformat table " which is in pivottable option for Excel 2003 |
|[SetIsAutoFormat](./setisautoformat/) | Indicates whether the PivotTable report is automatically formatted.Checkbox "autoformat table " which is in pivottable option for Excel 2003 |
|[GetAutofitColumnWidthOnUpdate](./getautofitcolumnwidthonupdate/) | Indicates whether autofitting column width on update |
|[SetAutofitColumnWidthOnUpdate](./setautofitcolumnwidthonupdate/) | Indicates whether autofitting column width on update |
|[GetAutoFormatType](./getautoformattype/) | Gets and sets the auto format type of PivotTable. |
|[SetAutoFormatType](./setautoformattype/) | Gets and sets the auto format type of PivotTable. |
|[GetHasBlankRows](./gethasblankrows/) | Indicates whether to add blank rows.This property only applies for the PivotTable auto format types which needs to add blank rows. |
|[SetHasBlankRows](./sethasblankrows/) | Indicates whether to add blank rows.This property only applies for the PivotTable auto format types which needs to add blank rows. |
|[GetMergeLabels](./getmergelabels/) | True if the specified PivotTable report's outer-row item, column item, subtotal, and grand total labels use merged cells. |
|[SetMergeLabels](./setmergelabels/) | True if the specified PivotTable report's outer-row item, column item, subtotal, and grand total labels use merged cells. |
|[GetPreserveFormatting](./getpreserveformatting/) | Indicates whether formatting is preserved when the PivotTable is refreshed or recalculated. |
|[SetPreserveFormatting](./setpreserveformatting/) | Indicates whether formatting is preserved when the PivotTable is refreshed or recalculated. |
|[GetShowDrill](./getshowdrill/) | Gets and sets whether showing expand/collapse buttons. |
|[SetShowDrill](./setshowdrill/) | Gets and sets whether showing expand/collapse buttons. |
|[GetEnableDrilldown](./getenabledrilldown/) | Gets whether drilldown is enabled. |
|[SetEnableDrilldown](./setenabledrilldown/) | Gets whether drilldown is enabled. |
|[GetEnableFieldDialog](./getenablefielddialog/) | Indicates whether the PivotTable Field dialog box is availablewhen the user double-clicks the PivotTable field. |
|[SetEnableFieldDialog](./setenablefielddialog/) | Indicates whether the PivotTable Field dialog box is availablewhen the user double-clicks the PivotTable field. |
|[GetEnableFieldList](./getenablefieldlist/) | Indicates whether the field list for the PivotTable is available on the view of Excel. |
|[SetEnableFieldList](./setenablefieldlist/) | Indicates whether the field list for the PivotTable is available on the view of Excel. |
|[GetEnableWizard](./getenablewizard/) | Indicates whether the PivotTable Wizard is available. |
|[SetEnableWizard](./setenablewizard/) | Indicates whether the PivotTable Wizard is available. |
|[GetSubtotalHiddenPageItems](./getsubtotalhiddenpageitems/) | Indicates whether hidden page field items in the PivotTable reportare included in row and column subtotals, block totals, and grand totals.The default value is False. |
|[SetSubtotalHiddenPageItems](./setsubtotalhiddenpageitems/) | Indicates whether hidden page field items in the PivotTable reportare included in row and column subtotals, block totals, and grand totals.The default value is False. |
|[GetGrandTotalName](./getgrandtotalname/) | Returns the label that is displayed in the grand total column or row heading.The default value is the string "Grand Total". |
|[SetGrandTotalName](./setgrandtotalname/) | Returns the label that is displayed in the grand total column or row heading.The default value is the string "Grand Total". |
|[GetManualUpdate](./getmanualupdate/) | Indicates whether the PivotTable report is recalculated only at the user's request. |
|[SetManualUpdate](./setmanualupdate/) | Indicates whether the PivotTable report is recalculated only at the user's request. |
|[GetAllowMultipleFiltersPerField](./getallowmultiplefiltersperfield/) | Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. |
|[SetAllowMultipleFiltersPerField](./setallowmultiplefiltersperfield/) | Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. |
|[GetMissingItemsLimit](./getmissingitemslimit/) | Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. |
|[SetMissingItemsLimit](./setmissingitemslimit/) | Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. |
|[GetEnableDataValueEditing](./getenabledatavalueediting/) | Specifies a boolean value that indicates whether the user is allowed to edit the cells in the data area of the pivottable.Enable cell editing in the values area |
|[SetEnableDataValueEditing](./setenabledatavalueediting/) | Specifies a boolean value that indicates whether the user is allowed to edit the cells in the data area of the pivottable.Enable cell editing in the values area |
|[GetShowDataTips](./getshowdatatips/) | Specifies a boolean value that indicates whether tooltips should be displayed for PivotTable data cells. |
|[SetShowDataTips](./setshowdatatips/) | Specifies a boolean value that indicates whether tooltips should be displayed for PivotTable data cells. |
|[GetShowMemberPropertyTips](./getshowmemberpropertytips/) | Specifies a boolean value that indicates whether member property information should be omitted from PivotTable tooltips. |
|[SetShowMemberPropertyTips](./setshowmemberpropertytips/) | Specifies a boolean value that indicates whether member property information should be omitted from PivotTable tooltips. |
|[GetShowValuesRow](./getshowvaluesrow/) | Indicates whether showing values row. |
|[SetShowValuesRow](./setshowvaluesrow/) | Indicates whether showing values row. |
|[GetShowEmptyCol](./getshowemptycol/) | Indicates whether to include empty columns in the table |
|[SetShowEmptyCol](./setshowemptycol/) | Indicates whether to include empty columns in the table |
|[GetShowEmptyRow](./getshowemptyrow/) | Indicates whether to include empty rows in the table. |
|[SetShowEmptyRow](./setshowemptyrow/) | Indicates whether to include empty rows in the table. |
|[GetFieldListSortAscending](./getfieldlistsortascending/) | Indicates whether fields in the PivotTable are sorted in non-default order in the field list. |
|[SetFieldListSortAscending](./setfieldlistsortascending/) | Indicates whether fields in the PivotTable are sorted in non-default order in the field list. |
|[GetPrintDrill](./getprintdrill/) | Specifies a boolean value that indicates whether drill indicators should be printed.print expand/collapse buttons when displayed on pivottable. |
|[SetPrintDrill](./setprintdrill/) | Specifies a boolean value that indicates whether drill indicators should be printed.print expand/collapse buttons when displayed on pivottable. |
|[GetAltTextTitle](./getalttexttitle/) | Gets and sets the title of the alter text. |
|[SetAltTextTitle](./setalttexttitle/) | Gets and sets the title of the alter text. |
|[GetAltTextDescription](./getalttextdescription/) | Gets the description of the alt text. |
|[SetAltTextDescription](./setalttextdescription/) | Gets the description of the alt text. |
|[GetName](./getname/) | Gets the name of the PivotTable |
|[SetName](./setname/) | Gets the name of the PivotTable |
|[GetColumnHeaderCaption](./getcolumnheadercaption/) | Gets the Column Header Caption of the PivotTable. |
|[SetColumnHeaderCaption](./setcolumnheadercaption/) | Gets the Column Header Caption of the PivotTable. |
|[GetIndent](./getindent/) | Specifies the indentation increment for compact axis and can be used to set the Report Layout to Compact Form. |
|[SetIndent](./setindent/) | Specifies the indentation increment for compact axis and can be used to set the Report Layout to Compact Form. |
|[GetRowHeaderCaption](./getrowheadercaption/) | Gets the Row Header Caption of the PivotTable. |
|[SetRowHeaderCaption](./setrowheadercaption/) | Gets the Row Header Caption of the PivotTable. |
|[GetShowRowHeaderCaption](./getshowrowheadercaption/) | Indicates whether row header caption is shown in the PivotTable reportIndicates whether Display field captions and filter drop downs |
|[SetShowRowHeaderCaption](./setshowrowheadercaption/) | Indicates whether row header caption is shown in the PivotTable reportIndicates whether Display field captions and filter drop downs |
|[GetCustomListSort](./getcustomlistsort/) | Indicates whether consider built-in custom list when sort data |
|[SetCustomListSort](./setcustomlistsort/) | Indicates whether consider built-in custom list when sort data |
|[GetConditionalFormats](./getconditionalformats/) | Gets the conditional formats of the pivot table. |
|[GetPageFieldOrder](./getpagefieldorder/) | Gets and sets the order in which page fields are added to the PivotTable report's layout. |
|[SetPageFieldOrder](./setpagefieldorder/) | Gets and sets the order in which page fields are added to the PivotTable report's layout. |
|[GetPageFieldWrapCount](./getpagefieldwrapcount/) | Gets the number of page fields in each column or row in the PivotTable report. |
|[SetPageFieldWrapCount](./setpagefieldwrapcount/) | Gets the number of page fields in each column or row in the PivotTable report. |
|[GetTag](./gettag/) | Gets a string saved with the PivotTable report. |
|[SetTag](./settag/) | Gets a string saved with the PivotTable report. |
|[GetSaveData](./getsavedata/) | Indicates whether data for the PivotTable report is saved with the workbook. |
|[SetSaveData](./setsavedata/) | Indicates whether data for the PivotTable report is saved with the workbook. |
|[GetRefreshDataOnOpeningFile](./getrefreshdataonopeningfile/) | Indicates whether Refresh Data when Opening File. |
|[SetRefreshDataOnOpeningFile](./setrefreshdataonopeningfile/) | Indicates whether Refresh Data when Opening File. |
|[GetSourceType](./getsourcetype/) | Gets the data source type of the pivot table. |
|[GetSourceDataConnections](./getsourcedataconnections/) | Gets the external connection data sources. |
|[GetNamesOfSourceDataConnections](./getnamesofsourcedataconnections/) | Gets the name of external source data connections. |
|[GetDataSource](./getdatasource/) | Gets and sets the data source of the pivot table. |
|[SetDataSource](./setdatasource/) | Gets and sets the data source of the pivot table. |
|[ChangeDataSource](./changedatasource/) | Set pivottable's source data. |
|[GetSource](./getsource/) | Get pivottable's source data. |
|[GetSource_Bool](./getsource_bool/) | Get pivottable's source data. |
|[RefreshData](./refreshdata/) | Refreshes pivottable's data and setting from it's data source. |
|[RefreshData_PivotTableRefreshOption](./refreshdata_pivottablerefreshoption/) | Refreshes pivottable's data and setting from it's data source with options. |
|[CalculateData](./calculatedata/) | Calculates pivottable's data to cells. |
|[CalculateData_PivotTableCalculateOption](./calculatedata_pivottablecalculateoption/) | Calculating pivot tables with options |
|[ClearData](./cleardata/) | Clear PivotTable's data and formatting |
|[CalculateRange](./calculaterange/) | Calculates pivottable's range. |
|[FormatAll](./formatall/) | Format all the cell in the pivottable area |
|[FormatRow](./formatrow/) | Format the row data in the pivottable area |
|[Format_PivotArea_Style](./format_pivotarea_style/) | Formats selected area of the PivotTable. |
|[Format_CellArea_Style](./format_cellarea_style/) | Formats selected area of the PivotTable. |
|[Format_Int_Int_Style](./format_int_int_style/) | Format the cell in the pivottable area |
|[SelectArea](./selectarea/) | Select an area of pivot table view. |
|[ShowDetail](./showdetail/) | Show the detail of one item in the data region to a new Table. |
|[GetPivotFormats](./getpivotformats/) | Gets the collection of formats applied to PivotTable. |
|[GetRepeatItemsOnEachPrintedPage](./getrepeatitemsoneachprintedpage/) | Indicates whether pivot item captions on the row area are repeated on each printed page for pivot fields in tabular form. |
|[SetRepeatItemsOnEachPrintedPage](./setrepeatitemsoneachprintedpage/) | Indicates whether pivot item captions on the row area are repeated on each printed page for pivot fields in tabular form. |
|[GetPrintTitles](./getprinttitles/) | Indicates whether the print titles for the worksheet are set basedon the PivotTable report. The default value is false. |
|[SetPrintTitles](./setprinttitles/) | Indicates whether the print titles for the worksheet are set basedon the PivotTable report. The default value is false. |
|[GetDisplayImmediateItems](./getdisplayimmediateitems/) | Indicates whether items in the row and column areas are visiblewhen the data area of the PivotTable is empty. The default value is true. |
|[SetDisplayImmediateItems](./setdisplayimmediateitems/) | Indicates whether items in the row and column areas are visiblewhen the data area of the PivotTable is empty. The default value is true. |
|[IsSelected](./isselected/) | Indicates whether this PivotTable is selected. |
|[SetIsSelected](./setisselected/) | Indicates whether this PivotTable is selected. |
|[GetShowPivotStyleRowHeader](./getshowpivotstylerowheader/) | Indicates whether the row header in the pivot table should have the style applied. |
|[SetShowPivotStyleRowHeader](./setshowpivotstylerowheader/) | Indicates whether the row header in the pivot table should have the style applied. |
|[GetShowPivotStyleColumnHeader](./getshowpivotstylecolumnheader/) | Indicates whether the column header in the pivot table should have the style applied. |
|[SetShowPivotStyleColumnHeader](./setshowpivotstylecolumnheader/) | Indicates whether the column header in the pivot table should have the style applied. |
|[GetShowPivotStyleRowStripes](./getshowpivotstylerowstripes/) | Indicates whether row stripe formatting is applied. |
|[SetShowPivotStyleRowStripes](./setshowpivotstylerowstripes/) | Indicates whether row stripe formatting is applied. |
|[GetShowPivotStyleColumnStripes](./getshowpivotstylecolumnstripes/) | Indicates whether stripe formatting is applied for column. |
|[SetShowPivotStyleColumnStripes](./setshowpivotstylecolumnstripes/) | Indicates whether stripe formatting is applied for column. |
|[GetShowPivotStyleLastColumn](./getshowpivotstylelastcolumn/) | Indicates whether the column formatting is applied. |
|[SetShowPivotStyleLastColumn](./setshowpivotstylelastcolumn/) | Indicates whether the column formatting is applied. |
|[GetHorizontalPageBreaks](./gethorizontalpagebreaks/) | Gets horizontal page breaks of this pivot table. |
|[ShowInCompactForm](./showincompactform/) | Layouts the PivotTable in compact form. |
|[ShowInOutlineForm](./showinoutlineform/) | Layouts the PivotTable in outline form. |
|[ShowInTabularForm](./showintabularform/) | Layouts the PivotTable in tabular form. |
|[GetCellByDisplayName](./getcellbydisplayname/) | Gets the Cell object by the display name of PivotField. |
|[GetChildren](./getchildren/) | Gets the Children Pivot Tables which use this PivotTable data as data source. |
