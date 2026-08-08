---
title: "PivotTable"
linktitle: "PivotTable"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Summary description for PivotTable."
type: docs
weight: 2900
url: /nodejs/aspose.cells/pivottable/
---

## PivotTable class

Summary description for PivotTable.

## Methods

| Name | Description |
| --- | --- |
| [addCalculatedField(name, formula, dragToDataArea)](#addcalculatedfield) | Adds a calculated field to pivot field. |
| [addCalculatedField(name, formula)](#addcalculatedfield-1) | Adds a calculated field to pivot field and drag it to data area. |
| [addFieldToArea(fieldType, fieldName)](#addfieldtoarea) | Adds the field to the specific area. addFieldToArea(int, com.aspose.cells.PivotField) |
| [addFieldToArea(fieldType, baseFieldIndex)](#addfieldtoarea-1) | Adds the field to the specific area. addFieldToArea(int, com.aspose.cells.PivotField) |
| [addFieldToArea(fieldType, pivotField)](#addfieldtoarea-2) | Adds the field to the specific area. |
| [calculateData()](#calculatedata) | Calculates pivottable's data to cells. Cell.Value in the pivot range could not return the correct result if the method i |
| [calculateData()](#calculatedata-1) |  |
| [calculateRange()](#calculaterange) | Calculates pivottable's range. If this method is not been called,maybe the pivottable range is not corrected. |
| [changeDataSource()](#changedatasource) | Set pivottable's source data. Sheet1!$A$1:$C$3 |
| [clearAll()](#clearall) |  |
| [clearData()](#cleardata) | Clear PivotTable's data and formatting If this method is not called before you add or delete PivotField, Maybe the Pivot |
| [clearFilters()](#clearfilters) |  |
| [copyStyle(pivotTable)](#copystyle) | Copies named style from another pivot table. |
| [dispose()](#dispose) | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [fields(fieldType)](#fields) | Gets the specific fields by the field type. NOTE: This method is now obsolete. Instead, please use PivotField.GetFields( |
| [format(pivotArea, style)](#format) | Formats selected area of the PivotTable. |
| [format()](#format-1) |  |
| [format(row, column, style)](#format-2) | Format the cell in the pivottable area |
| [formatAll(style)](#formatall) | Format all the cell in the pivottable area |
| [formatRow(row, style)](#formatrow) | Format the row data in the pivottable area |
| [getAllowMultipleFiltersPerField()](#getallowmultiplefiltersperfield) |  |
| [getAltTextDescription()](#getalttextdescription) | Gets the description of the alt text |
| [getAltTextTitle()](#getalttexttitle) | Gets the title of the altertext |
| [getAutoFormatType()](#getautoformattype) | Gets and sets the auto format type of PivotTable. The value of the property is PivotTableAutoFormatType integer constant |
| [getAutofitColumnWidthOnUpdate()](#getautofitcolumnwidthonupdate) | Indicates whether autofitting column width on update |
| [getBaseFields()](#getbasefields) | Returns all base pivot fields in the PivotTable. |
| [getButtonArea()](#getbuttonarea) |  |
| [getCellByDisplayName(displayName)](#getcellbydisplayname) | Gets the Cell object by the display name of PivotField. |
| [getChildren()](#getchildren) | Gets the Children Pivot Tables which use this PivotTable data as data source. |
| [getColumnFields()](#getcolumnfields) | Returns a PivotFields object that are currently shown as column fields. |
| [getColumnGrand()](#getcolumngrand) | Indicates whether the PivotTable report shows grand totals for columns. |
| [getColumnHeaderCaption()](#getcolumnheadercaption) | Gets the Column Header Caption of the PivotTable. |
| [getColumnRange()](#getcolumnrange) | Returns a CellArea object that represents the range that contains the column area in the PivotTable report. Read-only. |
| [getConditionalFormats()](#getconditionalformats) |  |
| [getCustomListSort()](#getcustomlistsort) | Indicates whether consider built-in custom list when sort data |
| [getDataBodyRange()](#getdatabodyrange) | Returns a CellArea object that represents the range that contains the data area in the list between the header row and t |
| [getDataField()](#getdatafield) | Gets a PivotField object that represents all the data fields in a PivotTable. Read-only. It would only be created when t |
| [getDataFieldHeaderName()](#getdatafieldheadername) | Gets and sets the name of the value area field header in the PivotTable. |
| [getDataFields()](#getdatafields) | Gets a PivotField object that represents all the data fields in a PivotTable. Read-only.It would be init only when there |
| [getDataSource()](#getdatasource) | Gets and sets the data source of the pivot table. |
| [getDependentPivotTables()](#getdependentpivottables) |  |
| [getDisplayErrorString()](#getdisplayerrorstring) | Indicates whether the PivotTable report displays a custom string in cells that contain errors. |
| [getDisplayImmediateItems()](#getdisplayimmediateitems) | Indicates whether items in the row and column areas are visible when the data area of the PivotTable is empty. The defau |
| [getDisplayNullString()](#getdisplaynullstring) | Indicates whether the PivotTable report displays a custom string if the value is null. |
| [getEnableDataValueEditing()](#getenabledatavalueediting) | Specifies a boolean value that indicates whether the user is allowed to edit the cells in the data area of the pivottabl |
| [getEnableDrilldown()](#getenabledrilldown) | Gets whether drilldown is enabled. |
| [getEnableFieldDialog()](#getenablefielddialog) | Indicates whether the PivotTable Field dialog box is available when the user double-clicks the PivotTable field. |
| [getEnableFieldList()](#getenablefieldlist) | Gets whether enable the field list for the PivotTable. |
| [getEnableWizard()](#getenablewizard) | Indicates whether the PivotTable Wizard is available. |
| [getErrorString()](#geterrorstring) | Gets the string displayed in cells that contain errors when the DisplayErrorString property is true.The default value is |
| [getExternalConnectionDataSource()](#getexternalconnectiondatasource) | Gets the external connection data source. |
| [getFieldListSortAscending()](#getfieldlistsortascending) | Indicates whether fields in the PivotTable are sorted in non-default order in the field list. |
| [getFields(fieldType)](#getfields) | Gets the specific pivot field list by the region. |
| [getFilterArea()](#getfilterarea) |  |
| [getGrandTotalName()](#getgrandtotalname) | Returns the text string label that is displayed in the grand total column or row heading. The default value is the strin |
| [getHorizontalBreaks()](#gethorizontalbreaks) | get pivot table row index list of horizontal pagebreaks |
| [getHorizontalPageBreaks()](#gethorizontalpagebreaks) |  |
| [getIndent()](#getindent) | Specifies the indentation increment for compact axis and can be used to set the Report Layout to Compact Form. |
| [getItemPrintTitles()](#getitemprinttitles) | Indicates whether PivotItem names should be repeated at the top of each printed page. |
| [getManualUpdate()](#getmanualupdate) | Indicates whether the PivotTable report is recalculated only at the user's request. |
| [getMergeLabels()](#getmergelabels) | True if the specified PivotTable report's outer-row item, column item, subtotal, and grand total labels use merged cells |
| [getMissingItemsLimit()](#getmissingitemslimit) | Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. The v |
| [getName()](#getname) | Gets the name of the PivotTable |
| [getNamesOfSourceDataConnections()](#getnamesofsourcedataconnections) |  |
| [getNullString()](#getnullstring) | Gets the string displayed in cells that contain null values when the DisplayNullString property is true.The default valu |
| [getPageFieldOrder()](#getpagefieldorder) | Gets the order in which page fields are added to the PivotTable report's layout. The value of the property is PrintOrder |
| [getPageFieldWrapCount()](#getpagefieldwrapcount) | Gets the number of page fields in each column or row in the PivotTable report. |
| [getPageFields()](#getpagefields) | Returns a PivotFields object that are currently shown as page fields. |
| [getPivotCache()](#getpivotcache) |  |
| [getPivotFilters()](#getpivotfilters) | Returns a list of pivot filters. |
| [getPivotFormatConditions()](#getpivotformatconditions) | Gets the Format Conditions of the pivot table. |
| [getPivotFormats()](#getpivotformats) | Gets the collection of formats applied to PivotTable. |
| [getPivotTableStyle()](#getpivottablestyle) |  |
| [getPivotTableStyleName()](#getpivottablestylename) | Gets and sets the pivottable style name. |
| [getPivotTableStyleType()](#getpivottablestyletype) | Gets and sets the built-in pivot table style. The value of the property is PivotTableStyleType integer constant. |
| [getPivotTablesWithSamePivotCache()](#getpivottableswithsamepivotcache) |  |
| [getPreserveFormatting()](#getpreserveformatting) | Indicates whether formatting is preserved when the PivotTable is refreshed or recalculated. |
| [getPrintDrill()](#getprintdrill) | Specifies a boolean value that indicates whether drill indicators should be printed. print expand/collapse buttons when  |
| [getPrintTitles()](#getprinttitles) | Indicates whether the print titles for the worksheet are set based on the PivotTable report. The default value is false. |
| [getRefreshDataFlag()](#getrefreshdataflag) | Indicates whether Refreshing Data or not. |
| [getRefreshDataOnOpeningFile()](#getrefreshdataonopeningfile) | Indicates whether Refresh Data when Opening File. |
| [getRefreshDate()](#getrefreshdate) | Gets the last date time when the PivotTable was refreshed. |
| [getRefreshedByWho()](#getrefreshedbywho) | Gets the name of the last user who refreshed this PivotTable |
| [getRepeatItemsOnEachPrintedPage()](#getrepeatitemsoneachprintedpage) |  |
| [getRowFields()](#getrowfields) | Returns a PivotFields object that are currently shown as row fields. |
| [getRowGrand()](#getrowgrand) | Indicates whether the PivotTable report shows grand totals for rows. |
| [getRowHeaderCaption()](#getrowheadercaption) | Gets the Row Header Caption of the PivotTable. |
| [getRowRange()](#getrowrange) | Returns a CellArea object that represents the range that contains the row area in the PivotTable report. Read-only. |
| [getSaveData()](#getsavedata) | Indicates whether data for the PivotTable report is saved with the workbook. |
| [getShowColumnGrandTotals()](#getshowcolumngrandtotals) |  |
| [getShowDataTips()](#getshowdatatips) | Specifies a boolean value that indicates whether tooltips should be displayed for PivotTable data cells. |
| [getShowDrill()](#getshowdrill) | Gets and sets whether showing expand/collapse buttons. |
| [getShowEmptyCol()](#getshowemptycol) | Specifies a boolean value that indicates whether to include empty columns in the table |
| [getShowEmptyRow()](#getshowemptyrow) | Specifies a boolean value that indicates whether to include empty rows in the table. |
| [getShowMemberPropertyTips()](#getshowmemberpropertytips) | Specifies a boolean value that indicates whether member property information should be omitted from PivotTable tooltips. |
| [getShowPivotStyleColumnHeader()](#getshowpivotstylecolumnheader) | Indicates whether the column header in the pivot table should have the style applied. |
| [getShowPivotStyleColumnStripes()](#getshowpivotstylecolumnstripes) | Indicates whether stripe formatting is applied for column. |
| [getShowPivotStyleLastColumn()](#getshowpivotstylelastcolumn) | Indicates whether the column formatting is applied. |
| [getShowPivotStyleRowHeader()](#getshowpivotstylerowheader) | Indicates whether the row header in the pivot table should have the style applied. |
| [getShowPivotStyleRowStripes()](#getshowpivotstylerowstripes) | Indicates whether row stripe formatting is applied. |
| [getShowRowGrandTotals()](#getshowrowgrandtotals) |  |
| [getShowRowHeaderCaption()](#getshowrowheadercaption) | Indicates whether row header caption is shown in the PivotTable report Indicates whether Display field captions and filt |
| [getShowValuesRow()](#getshowvaluesrow) | Specifies a boolean value that indicates whether show values row. show the values row |
| [getSource()](#getsource) | Get pivottable's source data. |
| [getSource()](#getsource-1) |  |
| [getSourceDataConnections()](#getsourcedataconnections) |  |
| [getSourceType()](#getsourcetype) | The value of the property is PivotTableSourceType integer constant. |
| [getSubtotalHiddenPageItems()](#getsubtotalhiddenpageitems) | Indicates whether hidden page field items in the PivotTable report are included in row and column subtotals, block total |
| [getTableRange1()](#gettablerange1) | Returns a CellArea object that represents the range containing the entire PivotTable report, but doesn't include page fi |
| [getTableRange2()](#gettablerange2) | Returns a CellArea object that represents the range containing the entire PivotTable report, includes page fields. Read- |
| [getTag()](#gettag) | Gets a string saved with the PivotTable report. |
| [getTopRightArea()](#gettoprightarea) |  |
| [getValuesField()](#getvaluesfield) |  |
| [hasBlankRows()](#hasblankrows) | Indicates whether to add blank rows. This property only applies for the PivotTable auto format types which needs to add  |
| [isAutoFormat()](#isautoformat) | Indicates whether the PivotTable report is automatically formatted. Checkbox "autoformat table " which is in pivottable  |
| [isExcel2003Compatible()](#isexcel2003compatible) | Specifies whether the PivotTable is compatible for Excel2003 when refreshing PivotTable, if true, a string must be less  |
| [isGridDropZones()](#isgriddropzones) | Indicates whether the PivotTable report displays classic pivottable layout. (enables dragging fields in the grid) |
| [isMultipleFieldFilters()](#ismultiplefieldfilters) | Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. |
| [isSelected()](#isselected) | Indicates whether this PivotTable is selected. |
| [move(row, column)](#move) | Moves the PivotTable to a different location in the worksheet. |
| [move(destCellName)](#move-1) | Moves the PivotTable to a different location in the worksheet. |
| [moveTo()](#moveto) |  |
| [moveTo()](#moveto-1) |  |
| [refreshData()](#refreshdata) | Refreshes pivottable's data and setting from it's data source. We will gather data from data source to a pivot cache ,th |
| [refreshData(option)](#refreshdata-1) | Refreshes pivottable's data and setting from it's data source with options. |
| [removeField(fieldType, fieldName)](#removefield) | Removes a field from specific field area removeField(int, com.aspose.cells.PivotField) |
| [removeField(fieldType, baseFieldIndex)](#removefield-1) | Removes a field from specific field area removeField(int, com.aspose.cells.PivotField) |
| [removeField(fieldType, pivotField)](#removefield-2) | Remove field from specific field area |
| [selectArea()](#selectarea) |  |
| [setAllowMultipleFiltersPerField()](#setallowmultiplefiltersperfield) |  |
| [setAltTextDescription()](#setalttextdescription) | Gets the description of the alt text |
| [setAltTextTitle()](#setalttexttitle) | Gets the title of the altertext |
| [setAutoFormat()](#setautoformat) | Indicates whether the PivotTable report is automatically formatted. Checkbox "autoformat table " which is in pivottable  |
| [setAutoFormatType()](#setautoformattype) | Gets and sets the auto format type of PivotTable. The value of the property is PivotTableAutoFormatType integer constant |
| [setAutoGroupField()](#setautogroupfield) | Sets auto field group by the PivotTable. baseFieldIndex - The row or column field index in the base fields NOTE: This me |
| [setAutoGroupField(pivotField)](#setautogroupfield-1) | Sets auto field group by the PivotTable. NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() met |
| [setAutofitColumnWidthOnUpdate()](#setautofitcolumnwidthonupdate) | Indicates whether autofitting column width on update |
| [setColumnGrand()](#setcolumngrand) | Indicates whether the PivotTable report shows grand totals for columns. |
| [setColumnHeaderCaption()](#setcolumnheadercaption) | Gets the Column Header Caption of the PivotTable. |
| [setCustomListSort()](#setcustomlistsort) | Indicates whether consider built-in custom list when sort data |
| [setDataFieldHeaderName()](#setdatafieldheadername) | Gets and sets the name of the value area field header in the PivotTable. |
| [setDataSource()](#setdatasource) | Gets and sets the data source of the pivot table. |
| [setDisplayErrorString()](#setdisplayerrorstring) | Indicates whether the PivotTable report displays a custom string in cells that contain errors. |
| [setDisplayImmediateItems()](#setdisplayimmediateitems) | Indicates whether items in the row and column areas are visible when the data area of the PivotTable is empty. The defau |
| [setDisplayNullString()](#setdisplaynullstring) | Indicates whether the PivotTable report displays a custom string if the value is null. |
| [setEnableDataValueEditing()](#setenabledatavalueediting) | Specifies a boolean value that indicates whether the user is allowed to edit the cells in the data area of the pivottabl |
| [setEnableDrilldown()](#setenabledrilldown) | Gets whether drilldown is enabled. |
| [setEnableFieldDialog()](#setenablefielddialog) | Indicates whether the PivotTable Field dialog box is available when the user double-clicks the PivotTable field. |
| [setEnableFieldList()](#setenablefieldlist) | Gets whether enable the field list for the PivotTable. |
| [setEnableWizard()](#setenablewizard) | Indicates whether the PivotTable Wizard is available. |
| [setErrorString()](#seterrorstring) | Gets the string displayed in cells that contain errors when the DisplayErrorString property is true.The default value is |
| [setExcel2003Compatible()](#setexcel2003compatible) | Specifies whether the PivotTable is compatible for Excel2003 when refreshing PivotTable, if true, a string must be less  |
| [setFieldListSortAscending()](#setfieldlistsortascending) | Indicates whether fields in the PivotTable are sorted in non-default order in the field list. |
| [setGrandTotalName()](#setgrandtotalname) | Returns the text string label that is displayed in the grand total column or row heading. The default value is the strin |
| [setGridDropZones()](#setgriddropzones) | Indicates whether the PivotTable report displays classic pivottable layout. (enables dragging fields in the grid) |
| [setHasBlankRows()](#sethasblankrows) | Indicates whether to add blank rows. This property only applies for the PivotTable auto format types which needs to add  |
| [setIndent()](#setindent) | Specifies the indentation increment for compact axis and can be used to set the Report Layout to Compact Form. |
| [setItemPrintTitles()](#setitemprinttitles) | Indicates whether PivotItem names should be repeated at the top of each printed page. |
| [setManualGroupField(baseFieldIndex, startVal, endVal, groupByList, intervalNum)](#setmanualgroupfield) | Sets manual field group by the PivotTable. NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() m |
| [setManualGroupField(pivotField, startVal, endVal, groupByList, intervalNum)](#setmanualgroupfield-1) | Sets manual field group by the PivotTable. NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() m |
| [setManualGroupField(baseFieldIndex, startVal, endVal, groupByList, intervalNum)](#setmanualgroupfield-2) | Sets manual field group by the PivotTable. NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() m |
| [setManualGroupField(pivotField, startVal, endVal, groupByList, intervalNum)](#setmanualgroupfield-3) | Sets manual field group by the PivotTable. NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() m |
| [setManualUpdate()](#setmanualupdate) | Indicates whether the PivotTable report is recalculated only at the user's request. |
| [setMergeLabels()](#setmergelabels) | True if the specified PivotTable report's outer-row item, column item, subtotal, and grand total labels use merged cells |
| [setMissingItemsLimit()](#setmissingitemslimit) | Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. The v |
| [setMultipleFieldFilters()](#setmultiplefieldfilters) | Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. |
| [setName()](#setname) | Gets the name of the PivotTable |
| [setNullString()](#setnullstring) | Gets the string displayed in cells that contain null values when the DisplayNullString property is true.The default valu |
| [setPageFieldOrder()](#setpagefieldorder) | Gets the order in which page fields are added to the PivotTable report's layout. The value of the property is PrintOrder |
| [setPageFieldWrapCount()](#setpagefieldwrapcount) | Gets the number of page fields in each column or row in the PivotTable report. |
| [setPivotTableStyle()](#setpivottablestyle) |  |
| [setPivotTableStyleName()](#setpivottablestylename) | Gets and sets the pivottable style name. |
| [setPivotTableStyleType()](#setpivottablestyletype) | Gets and sets the built-in pivot table style. The value of the property is PivotTableStyleType integer constant. |
| [setPreserveFormatting()](#setpreserveformatting) | Indicates whether formatting is preserved when the PivotTable is refreshed or recalculated. |
| [setPrintDrill()](#setprintdrill) | Specifies a boolean value that indicates whether drill indicators should be printed. print expand/collapse buttons when  |
| [setPrintTitles()](#setprinttitles) | Indicates whether the print titles for the worksheet are set based on the PivotTable report. The default value is false. |
| [setRefreshDataFlag()](#setrefreshdataflag) | Indicates whether Refreshing Data or not. |
| [setRefreshDataOnOpeningFile()](#setrefreshdataonopeningfile) | Indicates whether Refresh Data when Opening File. |
| [setRepeatItemsOnEachPrintedPage()](#setrepeatitemsoneachprintedpage) |  |
| [setRowGrand()](#setrowgrand) | Indicates whether the PivotTable report shows grand totals for rows. |
| [setRowHeaderCaption()](#setrowheadercaption) | Gets the Row Header Caption of the PivotTable. |
| [setSaveData()](#setsavedata) | Indicates whether data for the PivotTable report is saved with the workbook. |
| [setSelected()](#setselected) | Indicates whether this PivotTable is selected. |
| [setShowColumnGrandTotals()](#setshowcolumngrandtotals) |  |
| [setShowDataTips()](#setshowdatatips) | Specifies a boolean value that indicates whether tooltips should be displayed for PivotTable data cells. |
| [setShowDrill()](#setshowdrill) | Gets and sets whether showing expand/collapse buttons. |
| [setShowEmptyCol()](#setshowemptycol) | Specifies a boolean value that indicates whether to include empty columns in the table |
| [setShowEmptyRow()](#setshowemptyrow) | Specifies a boolean value that indicates whether to include empty rows in the table. |
| [setShowMemberPropertyTips()](#setshowmemberpropertytips) | Specifies a boolean value that indicates whether member property information should be omitted from PivotTable tooltips. |
| [setShowPivotStyleColumnHeader()](#setshowpivotstylecolumnheader) | Indicates whether the column header in the pivot table should have the style applied. |
| [setShowPivotStyleColumnStripes()](#setshowpivotstylecolumnstripes) | Indicates whether stripe formatting is applied for column. |
| [setShowPivotStyleLastColumn()](#setshowpivotstylelastcolumn) | Indicates whether the column formatting is applied. |
| [setShowPivotStyleRowHeader()](#setshowpivotstylerowheader) | Indicates whether the row header in the pivot table should have the style applied. |
| [setShowPivotStyleRowStripes()](#setshowpivotstylerowstripes) | Indicates whether row stripe formatting is applied. |
| [setShowRowGrandTotals()](#setshowrowgrandtotals) |  |
| [setShowRowHeaderCaption()](#setshowrowheadercaption) | Indicates whether row header caption is shown in the PivotTable report Indicates whether Display field captions and filt |
| [setShowValuesRow()](#setshowvaluesrow) | Specifies a boolean value that indicates whether show values row. show the values row |
| [setSubtotalHiddenPageItems()](#setsubtotalhiddenpageitems) | Indicates whether hidden page field items in the PivotTable report are included in row and column subtotals, block total |
| [setTag()](#settag) | Gets a string saved with the PivotTable report. |
| [setUngroup(baseFieldIndex)](#setungroup) | Sets ungroup by the PivotTable NOTE: This method is now obsolete. Instead, please use PivotField.Ungroup() method. This  |
| [setUngroup(pivotField)](#setungroup-1) | Sets ungroup by the PivotTable NOTE: This method is now obsolete. Instead, please use PivotField.Ungroup() method. This  |
| [showDetail()](#showdetail) |  |
| [showInCompactForm()](#showincompactform) | Layouts the PivotTable in compact form. |
| [showInOutlineForm()](#showinoutlineform) | Layouts the PivotTable in outline form. |
| [showInTabularForm()](#showintabularform) | Layouts the PivotTable in tabular form. |
| [showReportFilterPage(pageField)](#showreportfilterpage) | Show all the report filter pages according to PivotField, the PivotField must be located in the PageFields. |
| [showReportFilterPageByIndex(posIndex)](#showreportfilterpagebyindex) | Show all the report filter pages according to the position index in the PageFields |
| [showReportFilterPageByName(fieldName)](#showreportfilterpagebyname) | Show all the report filter pages according to PivotField's name, the PivotField must be located in the PageFields. |

### addCalculatedField(name, formula, dragToDataArea) {#addcalculatedfield}

Adds a calculated field to pivot field.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the calculated field |
| formula | String | The formula of the calculated field. |
| dragToDataArea | boolean | True,drag this field to data area immediately |

### addCalculatedField(name, formula) {#addcalculatedfield-1}

Adds a calculated field to pivot field and drag it to data area.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the calculated field |
| formula | String | The formula of the calculated field. |

### addFieldToArea(fieldType, fieldName) {#addfieldtoarea}

Adds the field to the specific area. addFieldToArea(int, com.aspose.cells.PivotField)

| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | Number | PivotFieldType |
| fieldName | String | The name in the base fields. |

**Returns:** Number — `Number` The field position in the specific fields.If there is no field named as it, return -1.

### addFieldToArea(fieldType, baseFieldIndex) {#addfieldtoarea-1}

Adds the field to the specific area. addFieldToArea(int, com.aspose.cells.PivotField)

| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | Number | PivotFieldType |
| baseFieldIndex | Number | The field index in the base fields. |

**Returns:** Number — `Number` The field position in the specific fields.

### addFieldToArea(fieldType, pivotField) {#addfieldtoarea-2}

Adds the field to the specific area.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | Number | PivotFieldType |
| pivotField | PivotField | the field in the base fields. |

**Returns:** Number — `Number` the field position in the specific fields.

### calculateData() {#calculatedata}

Calculates pivottable's data to cells. Cell.Value in the pivot range could not return the correct result if the method is not been called. This method calculates data with an inner pivot cache,not original data source. So if the data source is changed, please call RefreshData() method first.

### calculateData() {#calculatedata-1}

### calculateRange() {#calculaterange}

Calculates pivottable's range. If this method is not been called,maybe the pivottable range is not corrected.

### changeDataSource() {#changedatasource}

Set pivottable's source data. Sheet1!$A$1:$C$3

### clearAll() {#clearall}

### clearData() {#cleardata}

Clear PivotTable's data and formatting If this method is not called before you add or delete PivotField, Maybe the PivotTable data is not corrected

### clearFilters() {#clearfilters}

### copyStyle(pivotTable) {#copystyle}

Copies named style from another pivot table.

| Parameter | Type | Description |
| --- | --- | --- |
| pivotTable | PivotTable | Source pivot table. |

### dispose() {#dispose}

Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources.

### fields(fieldType) {#fields}

Gets the specific fields by the field type. NOTE: This method is now obsolete. Instead, please use PivotField.GetFields() method. This method will be removed 12 months later since May 2024. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | Number | PivotFieldType |

**Returns:** PivotFieldCollection — `PivotFieldCollection` the specific field collection

### format(pivotArea, style) {#format}

Formats selected area of the PivotTable.

| Parameter | Type | Description |
| --- | --- | --- |
| pivotArea | PivotArea |  |
| style | Style |  |

### format() {#format-1}

### format(row, column, style) {#format-2}

Format the cell in the pivottable area

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row Index of the cell |
| column | Number | Column index of the cell |
| style | Style | Style which is to format the cell |

### formatAll(style) {#formatall}

Format all the cell in the pivottable area

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | Style which is to format |

### formatRow(row, style) {#formatrow}

Format the row data in the pivottable area

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row Index of the Row object |
| style | Style | Style which is to format |

### getAllowMultipleFiltersPerField() {#getallowmultiplefiltersperfield}

### getAltTextDescription() {#getalttextdescription}

Gets the description of the alt text

### getAltTextTitle() {#getalttexttitle}

Gets the title of the altertext

### getAutoFormatType() {#getautoformattype}

Gets and sets the auto format type of PivotTable. The value of the property is PivotTableAutoFormatType integer constant.PivotTableAutoFormatType

### getAutofitColumnWidthOnUpdate() {#getautofitcolumnwidthonupdate}

Indicates whether autofitting column width on update

### getBaseFields() {#getbasefields}

Returns all base pivot fields in the PivotTable.

### getButtonArea() {#getbuttonarea}

### getCellByDisplayName(displayName) {#getcellbydisplayname}

Gets the Cell object by the display name of PivotField.

| Parameter | Type | Description |
| --- | --- | --- |
| displayName | String | the DisplayName of PivotField |

**Returns:** Cell — `Cell` the Cell object

### getChildren() {#getchildren}

Gets the Children Pivot Tables which use this PivotTable data as data source.

**Returns:** Array ofPivotTable — `Array ofPivotTable` the PivotTable array object

### getColumnFields() {#getcolumnfields}

Returns a PivotFields object that are currently shown as column fields.

### getColumnGrand() {#getcolumngrand}

Indicates whether the PivotTable report shows grand totals for columns.

### getColumnHeaderCaption() {#getcolumnheadercaption}

Gets the Column Header Caption of the PivotTable.

### getColumnRange() {#getcolumnrange}

Returns a CellArea object that represents the range that contains the column area in the PivotTable report. Read-only.

### getConditionalFormats() {#getconditionalformats}

### getCustomListSort() {#getcustomlistsort}

Indicates whether consider built-in custom list when sort data

### getDataBodyRange() {#getdatabodyrange}

Returns a CellArea object that represents the range that contains the data area in the list between the header row and the insert row. Read-only.

### getDataField() {#getdatafield}

Gets a PivotField object that represents all the data fields in a PivotTable. Read-only. It would only be created when there are two or more data fields in the Data region. Defaultly it is in row region. You can drag it to the row/column region with PivotTable.AddFieldToArea() method .

### getDataFieldHeaderName() {#getdatafieldheadername}

Gets and sets the name of the value area field header in the PivotTable.

### getDataFields() {#getdatafields}

Gets a PivotField object that represents all the data fields in a PivotTable. Read-only.It would be init only when there are two or more data fields in the DataPiovtFiels. It only use to add DataPivotField to the PivotTable row/column area . Default is in row area.

### getDataSource() {#getdatasource}

Gets and sets the data source of the pivot table.

### getDependentPivotTables() {#getdependentpivottables}

### getDisplayErrorString() {#getdisplayerrorstring}

Indicates whether the PivotTable report displays a custom string in cells that contain errors.

### getDisplayImmediateItems() {#getdisplayimmediateitems}

Indicates whether items in the row and column areas are visible when the data area of the PivotTable is empty. The default value is true.

### getDisplayNullString() {#getdisplaynullstring}

Indicates whether the PivotTable report displays a custom string if the value is null.

### getEnableDataValueEditing() {#getenabledatavalueediting}

Specifies a boolean value that indicates whether the user is allowed to edit the cells in the data area of the pivottable. Enable cell editing in the values area

### getEnableDrilldown() {#getenabledrilldown}

Gets whether drilldown is enabled.

### getEnableFieldDialog() {#getenablefielddialog}

Indicates whether the PivotTable Field dialog box is available when the user double-clicks the PivotTable field.

### getEnableFieldList() {#getenablefieldlist}

Gets whether enable the field list for the PivotTable.

### getEnableWizard() {#getenablewizard}

Indicates whether the PivotTable Wizard is available.

### getErrorString() {#geterrorstring}

Gets the string displayed in cells that contain errors when the DisplayErrorString property is true.The default value is an empty string.

### getExternalConnectionDataSource() {#getexternalconnectiondatasource}

Gets the external connection data source.

### getFieldListSortAscending() {#getfieldlistsortascending}

Indicates whether fields in the PivotTable are sorted in non-default order in the field list.

### getFields(fieldType) {#getfields}

Gets the specific pivot field list by the region.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | Number | PivotFieldType |

**Returns:** PivotFieldCollection — `PivotFieldCollection` the specific pivot field collection

### getFilterArea() {#getfilterarea}

### getGrandTotalName() {#getgrandtotalname}

Returns the text string label that is displayed in the grand total column or row heading. The default value is the string "Grand Total".

### getHorizontalBreaks() {#gethorizontalbreaks}

get pivot table row index list of horizontal pagebreaks

**Returns:** ArrayList — `ArrayList`

### getHorizontalPageBreaks() {#gethorizontalpagebreaks}

### getIndent() {#getindent}

Specifies the indentation increment for compact axis and can be used to set the Report Layout to Compact Form.

### getItemPrintTitles() {#getitemprinttitles}

Indicates whether PivotItem names should be repeated at the top of each printed page.

### getManualUpdate() {#getmanualupdate}

Indicates whether the PivotTable report is recalculated only at the user's request.

### getMergeLabels() {#getmergelabels}

True if the specified PivotTable report's outer-row item, column item, subtotal, and grand total labels use merged cells.

### getMissingItemsLimit() {#getmissingitemslimit}

Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. The value of the property is PivotMissingItemLimitType integer constant.

### getName() {#getname}

Gets the name of the PivotTable

### getNamesOfSourceDataConnections() {#getnamesofsourcedataconnections}

### getNullString() {#getnullstring}

Gets the string displayed in cells that contain null values when the DisplayNullString property is true.The default value is an empty string.

### getPageFieldOrder() {#getpagefieldorder}

Gets the order in which page fields are added to the PivotTable report's layout. The value of the property is PrintOrderType integer constant.

### getPageFieldWrapCount() {#getpagefieldwrapcount}

Gets the number of page fields in each column or row in the PivotTable report.

### getPageFields() {#getpagefields}

Returns a PivotFields object that are currently shown as page fields.

### getPivotCache() {#getpivotcache}

### getPivotFilters() {#getpivotfilters}

Returns a list of pivot filters.

### getPivotFormatConditions() {#getpivotformatconditions}

Gets the Format Conditions of the pivot table.

### getPivotFormats() {#getpivotformats}

Gets the collection of formats applied to PivotTable.

### getPivotTableStyle() {#getpivottablestyle}

### getPivotTableStyleName() {#getpivottablestylename}

Gets and sets the pivottable style name.

### getPivotTableStyleType() {#getpivottablestyletype}

Gets and sets the built-in pivot table style. The value of the property is PivotTableStyleType integer constant.

### getPivotTablesWithSamePivotCache() {#getpivottableswithsamepivotcache}

### getPreserveFormatting() {#getpreserveformatting}

Indicates whether formatting is preserved when the PivotTable is refreshed or recalculated.

### getPrintDrill() {#getprintdrill}

Specifies a boolean value that indicates whether drill indicators should be printed. print expand/collapse buttons when displayed on pivottable.

### getPrintTitles() {#getprinttitles}

Indicates whether the print titles for the worksheet are set based on the PivotTable report. The default value is false.

### getRefreshDataFlag() {#getrefreshdataflag}

Indicates whether Refreshing Data or not.

### getRefreshDataOnOpeningFile() {#getrefreshdataonopeningfile}

Indicates whether Refresh Data when Opening File.

### getRefreshDate() {#getrefreshdate}

Gets the last date time when the PivotTable was refreshed.

### getRefreshedByWho() {#getrefreshedbywho}

Gets the name of the last user who refreshed this PivotTable

### getRepeatItemsOnEachPrintedPage() {#getrepeatitemsoneachprintedpage}

### getRowFields() {#getrowfields}

Returns a PivotFields object that are currently shown as row fields.

### getRowGrand() {#getrowgrand}

Indicates whether the PivotTable report shows grand totals for rows.

### getRowHeaderCaption() {#getrowheadercaption}

Gets the Row Header Caption of the PivotTable.

### getRowRange() {#getrowrange}

Returns a CellArea object that represents the range that contains the row area in the PivotTable report. Read-only.

### getSaveData() {#getsavedata}

Indicates whether data for the PivotTable report is saved with the workbook.

### getShowColumnGrandTotals() {#getshowcolumngrandtotals}

### getShowDataTips() {#getshowdatatips}

Specifies a boolean value that indicates whether tooltips should be displayed for PivotTable data cells.

### getShowDrill() {#getshowdrill}

Gets and sets whether showing expand/collapse buttons.

### getShowEmptyCol() {#getshowemptycol}

Specifies a boolean value that indicates whether to include empty columns in the table

### getShowEmptyRow() {#getshowemptyrow}

Specifies a boolean value that indicates whether to include empty rows in the table.

### getShowMemberPropertyTips() {#getshowmemberpropertytips}

Specifies a boolean value that indicates whether member property information should be omitted from PivotTable tooltips.

### getShowPivotStyleColumnHeader() {#getshowpivotstylecolumnheader}

Indicates whether the column header in the pivot table should have the style applied.

### getShowPivotStyleColumnStripes() {#getshowpivotstylecolumnstripes}

Indicates whether stripe formatting is applied for column.

### getShowPivotStyleLastColumn() {#getshowpivotstylelastcolumn}

Indicates whether the column formatting is applied.

### getShowPivotStyleRowHeader() {#getshowpivotstylerowheader}

Indicates whether the row header in the pivot table should have the style applied.

### getShowPivotStyleRowStripes() {#getshowpivotstylerowstripes}

Indicates whether row stripe formatting is applied.

### getShowRowGrandTotals() {#getshowrowgrandtotals}

### getShowRowHeaderCaption() {#getshowrowheadercaption}

Indicates whether row header caption is shown in the PivotTable report Indicates whether Display field captions and filter drop downs

### getShowValuesRow() {#getshowvaluesrow}

Specifies a boolean value that indicates whether show values row. show the values row

### getSource() {#getsource}

Get pivottable's source data.

### getSource() {#getsource-1}

### getSourceDataConnections() {#getsourcedataconnections}

### getSourceType() {#getsourcetype}

The value of the property is PivotTableSourceType integer constant.

### getSubtotalHiddenPageItems() {#getsubtotalhiddenpageitems}

Indicates whether hidden page field items in the PivotTable report are included in row and column subtotals, block totals, and grand totals. The default value is False.

### getTableRange1() {#gettablerange1}

Returns a CellArea object that represents the range containing the entire PivotTable report, but doesn't include page fields. Read-only.

### getTableRange2() {#gettablerange2}

Returns a CellArea object that represents the range containing the entire PivotTable report, includes page fields. Read-only.

### getTag() {#gettag}

Gets a string saved with the PivotTable report.

### getTopRightArea() {#gettoprightarea}

### getValuesField() {#getvaluesfield}

### hasBlankRows() {#hasblankrows}

Indicates whether to add blank rows. This property only applies for the PivotTable auto format types which needs to add blank rows.

### isAutoFormat() {#isautoformat}

Indicates whether the PivotTable report is automatically formatted. Checkbox "autoformat table " which is in pivottable option for Excel 2003

### isExcel2003Compatible() {#isexcel2003compatible}

Specifies whether the PivotTable is compatible for Excel2003 when refreshing PivotTable, if true, a string must be less than or equal to 255 characters, so if the string is greater than 255 characters, it will be truncated. if false, a string will not have the aforementioned restriction. The default value is true.

### isGridDropZones() {#isgriddropzones}

Indicates whether the PivotTable report displays classic pivottable layout. (enables dragging fields in the grid)

### isMultipleFieldFilters() {#ismultiplefieldfilters}

Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them.

### isSelected() {#isselected}

Indicates whether this PivotTable is selected.

### move(row, column) {#move}

Moves the PivotTable to a different location in the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | row index. |
| column | Number | column index. |

### move(destCellName) {#move-1}

Moves the PivotTable to a different location in the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| destCellName | String | the dest cell name. |

### moveTo() {#moveto}

### moveTo() {#moveto-1}

### refreshData() {#refreshdata}

Refreshes pivottable's data and setting from it's data source. We will gather data from data source to a pivot cache ,then calculate the data in the cache to the cells. This method is only used to gather all data to a pivot cache.

### refreshData(option) {#refreshdata-1}

Refreshes pivottable's data and setting from it's data source with options.

| Parameter | Type | Description |
| --- | --- | --- |
| option | PivotTableRefreshOption | The options for refreshing data source of pivot table. |

### removeField(fieldType, fieldName) {#removefield}

Removes a field from specific field area removeField(int, com.aspose.cells.PivotField)

| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | Number | PivotFieldType |
| fieldName | String | The name in the base fields. |

### removeField(fieldType, baseFieldIndex) {#removefield-1}

Removes a field from specific field area removeField(int, com.aspose.cells.PivotField)

| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | Number | PivotFieldType |
| baseFieldIndex | Number | The field index in the base fields. |

### removeField(fieldType, pivotField) {#removefield-2}

Remove field from specific field area

| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | Number | PivotFieldType |
| pivotField | PivotField | the field in the base fields. |

### selectArea() {#selectarea}

### setAllowMultipleFiltersPerField() {#setallowmultiplefiltersperfield}

### setAltTextDescription() {#setalttextdescription}

Gets the description of the alt text

### setAltTextTitle() {#setalttexttitle}

Gets the title of the altertext

### setAutoFormat() {#setautoformat}

Indicates whether the PivotTable report is automatically formatted. Checkbox "autoformat table " which is in pivottable option for Excel 2003

### setAutoFormatType() {#setautoformattype}

Gets and sets the auto format type of PivotTable. The value of the property is PivotTableAutoFormatType integer constant.PivotTableAutoFormatType

### setAutoGroupField() {#setautogroupfield}

Sets auto field group by the PivotTable. baseFieldIndex - The row or column field index in the base fields NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

### setAutoGroupField(pivotField) {#setautogroupfield-1}

Sets auto field group by the PivotTable. NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| pivotField | PivotField | The row or column field in the specific fields |

### setAutofitColumnWidthOnUpdate() {#setautofitcolumnwidthonupdate}

Indicates whether autofitting column width on update

### setColumnGrand() {#setcolumngrand}

Indicates whether the PivotTable report shows grand totals for columns.

### setColumnHeaderCaption() {#setcolumnheadercaption}

Gets the Column Header Caption of the PivotTable.

### setCustomListSort() {#setcustomlistsort}

Indicates whether consider built-in custom list when sort data

### setDataFieldHeaderName() {#setdatafieldheadername}

Gets and sets the name of the value area field header in the PivotTable.

### setDataSource() {#setdatasource}

Gets and sets the data source of the pivot table.

### setDisplayErrorString() {#setdisplayerrorstring}

Indicates whether the PivotTable report displays a custom string in cells that contain errors.

### setDisplayImmediateItems() {#setdisplayimmediateitems}

Indicates whether items in the row and column areas are visible when the data area of the PivotTable is empty. The default value is true.

### setDisplayNullString() {#setdisplaynullstring}

Indicates whether the PivotTable report displays a custom string if the value is null.

### setEnableDataValueEditing() {#setenabledatavalueediting}

Specifies a boolean value that indicates whether the user is allowed to edit the cells in the data area of the pivottable. Enable cell editing in the values area

### setEnableDrilldown() {#setenabledrilldown}

Gets whether drilldown is enabled.

### setEnableFieldDialog() {#setenablefielddialog}

Indicates whether the PivotTable Field dialog box is available when the user double-clicks the PivotTable field.

### setEnableFieldList() {#setenablefieldlist}

Gets whether enable the field list for the PivotTable.

### setEnableWizard() {#setenablewizard}

Indicates whether the PivotTable Wizard is available.

### setErrorString() {#seterrorstring}

Gets the string displayed in cells that contain errors when the DisplayErrorString property is true.The default value is an empty string.

### setExcel2003Compatible() {#setexcel2003compatible}

Specifies whether the PivotTable is compatible for Excel2003 when refreshing PivotTable, if true, a string must be less than or equal to 255 characters, so if the string is greater than 255 characters, it will be truncated. if false, a string will not have the aforementioned restriction. The default value is true.

### setFieldListSortAscending() {#setfieldlistsortascending}

Indicates whether fields in the PivotTable are sorted in non-default order in the field list.

### setGrandTotalName() {#setgrandtotalname}

Returns the text string label that is displayed in the grand total column or row heading. The default value is the string "Grand Total".

### setGridDropZones() {#setgriddropzones}

Indicates whether the PivotTable report displays classic pivottable layout. (enables dragging fields in the grid)

### setHasBlankRows() {#sethasblankrows}

Indicates whether to add blank rows. This property only applies for the PivotTable auto format types which needs to add blank rows.

### setIndent() {#setindent}

Specifies the indentation increment for compact axis and can be used to set the Report Layout to Compact Form.

### setItemPrintTitles() {#setitemprinttitles}

Indicates whether PivotItem names should be repeated at the top of each printed page.

### setManualGroupField(baseFieldIndex, startVal, endVal, groupByList, intervalNum) {#setmanualgroupfield}

Sets manual field group by the PivotTable. NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | Number | The row or column field index in the base fields |
| startVal | Number | Specifies the starting value for numeric grouping. |
| endVal | Number | Specifies the ending value for numeric grouping. |
| groupByList | ArrayList | Specifies the grouping type list. Specified by PivotTableGroupType |
| intervalNum | Number | Specifies the interval number group by numeric grouping. |

### setManualGroupField(pivotField, startVal, endVal, groupByList, intervalNum) {#setmanualgroupfield-1}

Sets manual field group by the PivotTable. NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| pivotField | PivotField | The row or column field in the base fields |
| startVal | Number | Specifies the starting value for numeric grouping. |
| endVal | Number | Specifies the ending value for numeric grouping. |
| groupByList | ArrayList | Specifies the grouping type list. Specified by PivotTableGroupType |
| intervalNum | Number | Specifies the interval number group by numeric grouping. |

### setManualGroupField(baseFieldIndex, startVal, endVal, groupByList, intervalNum) {#setmanualgroupfield-2}

Sets manual field group by the PivotTable. NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | Number | The row or column field index in the base fields |
| startVal | DateTime | Specifies the starting value for date grouping. |
| endVal | DateTime | Specifies the ending value for date grouping. |
| groupByList | ArrayList | Specifies the grouping type list. Specified by PivotTableGroupType |
| intervalNum | Number | Specifies the interval number group by in days grouping.The number of days must be positive integer of nonzero |

### setManualGroupField(pivotField, startVal, endVal, groupByList, intervalNum) {#setmanualgroupfield-3}

Sets manual field group by the PivotTable. NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| pivotField | PivotField | The row or column field in the base fields |
| startVal | DateTime | Specifies the starting value for date grouping. |
| endVal | DateTime | Specifies the ending value for date grouping. |
| groupByList | ArrayList | Specifies the grouping type list. Specified by PivotTableGroupType |
| intervalNum | Number | Specifies the interval number group by in days grouping.The number of days must be positive integer of nonzero |

### setManualUpdate() {#setmanualupdate}

Indicates whether the PivotTable report is recalculated only at the user's request.

### setMergeLabels() {#setmergelabels}

True if the specified PivotTable report's outer-row item, column item, subtotal, and grand total labels use merged cells.

### setMissingItemsLimit() {#setmissingitemslimit}

Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. The value of the property is PivotMissingItemLimitType integer constant.

### setMultipleFieldFilters() {#setmultiplefieldfilters}

Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them.

### setName() {#setname}

Gets the name of the PivotTable

### setNullString() {#setnullstring}

Gets the string displayed in cells that contain null values when the DisplayNullString property is true.The default value is an empty string.

### setPageFieldOrder() {#setpagefieldorder}

Gets the order in which page fields are added to the PivotTable report's layout. The value of the property is PrintOrderType integer constant.

### setPageFieldWrapCount() {#setpagefieldwrapcount}

Gets the number of page fields in each column or row in the PivotTable report.

### setPivotTableStyle() {#setpivottablestyle}

### setPivotTableStyleName() {#setpivottablestylename}

Gets and sets the pivottable style name.

### setPivotTableStyleType() {#setpivottablestyletype}

Gets and sets the built-in pivot table style. The value of the property is PivotTableStyleType integer constant.

### setPreserveFormatting() {#setpreserveformatting}

Indicates whether formatting is preserved when the PivotTable is refreshed or recalculated.

### setPrintDrill() {#setprintdrill}

Specifies a boolean value that indicates whether drill indicators should be printed. print expand/collapse buttons when displayed on pivottable.

### setPrintTitles() {#setprinttitles}

Indicates whether the print titles for the worksheet are set based on the PivotTable report. The default value is false.

### setRefreshDataFlag() {#setrefreshdataflag}

Indicates whether Refreshing Data or not.

### setRefreshDataOnOpeningFile() {#setrefreshdataonopeningfile}

Indicates whether Refresh Data when Opening File.

### setRepeatItemsOnEachPrintedPage() {#setrepeatitemsoneachprintedpage}

### setRowGrand() {#setrowgrand}

Indicates whether the PivotTable report shows grand totals for rows.

### setRowHeaderCaption() {#setrowheadercaption}

Gets the Row Header Caption of the PivotTable.

### setSaveData() {#setsavedata}

Indicates whether data for the PivotTable report is saved with the workbook.

### setSelected() {#setselected}

Indicates whether this PivotTable is selected.

### setShowColumnGrandTotals() {#setshowcolumngrandtotals}

### setShowDataTips() {#setshowdatatips}

Specifies a boolean value that indicates whether tooltips should be displayed for PivotTable data cells.

### setShowDrill() {#setshowdrill}

Gets and sets whether showing expand/collapse buttons.

### setShowEmptyCol() {#setshowemptycol}

Specifies a boolean value that indicates whether to include empty columns in the table

### setShowEmptyRow() {#setshowemptyrow}

Specifies a boolean value that indicates whether to include empty rows in the table.

### setShowMemberPropertyTips() {#setshowmemberpropertytips}

Specifies a boolean value that indicates whether member property information should be omitted from PivotTable tooltips.

### setShowPivotStyleColumnHeader() {#setshowpivotstylecolumnheader}

Indicates whether the column header in the pivot table should have the style applied.

### setShowPivotStyleColumnStripes() {#setshowpivotstylecolumnstripes}

Indicates whether stripe formatting is applied for column.

### setShowPivotStyleLastColumn() {#setshowpivotstylelastcolumn}

Indicates whether the column formatting is applied.

### setShowPivotStyleRowHeader() {#setshowpivotstylerowheader}

Indicates whether the row header in the pivot table should have the style applied.

### setShowPivotStyleRowStripes() {#setshowpivotstylerowstripes}

Indicates whether row stripe formatting is applied.

### setShowRowGrandTotals() {#setshowrowgrandtotals}

### setShowRowHeaderCaption() {#setshowrowheadercaption}

Indicates whether row header caption is shown in the PivotTable report Indicates whether Display field captions and filter drop downs

### setShowValuesRow() {#setshowvaluesrow}

Specifies a boolean value that indicates whether show values row. show the values row

### setSubtotalHiddenPageItems() {#setsubtotalhiddenpageitems}

Indicates whether hidden page field items in the PivotTable report are included in row and column subtotals, block totals, and grand totals. The default value is False.

### setTag() {#settag}

Gets a string saved with the PivotTable report.

### setUngroup(baseFieldIndex) {#setungroup}

Sets ungroup by the PivotTable NOTE: This method is now obsolete. Instead, please use PivotField.Ungroup() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | Number | The row or column field index in the base fields |

### setUngroup(pivotField) {#setungroup-1}

Sets ungroup by the PivotTable NOTE: This method is now obsolete. Instead, please use PivotField.Ungroup() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| pivotField | PivotField | The row or column field in the base fields |

### showDetail() {#showdetail}

### showInCompactForm() {#showincompactform}

Layouts the PivotTable in compact form.

### showInOutlineForm() {#showinoutlineform}

Layouts the PivotTable in outline form.

### showInTabularForm() {#showintabularform}

Layouts the PivotTable in tabular form.

### showReportFilterPage(pageField) {#showreportfilterpage}

Show all the report filter pages according to PivotField, the PivotField must be located in the PageFields.

| Parameter | Type | Description |
| --- | --- | --- |
| pageField | PivotField | The PivotField object |

### showReportFilterPageByIndex(posIndex) {#showreportfilterpagebyindex}

Show all the report filter pages according to the position index in the PageFields

| Parameter | Type | Description |
| --- | --- | --- |
| posIndex | Number | The position index in the PageFields |

### showReportFilterPageByName(fieldName) {#showreportfilterpagebyname}

Show all the report filter pages according to PivotField's name, the PivotField must be located in the PageFields.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldName | String | The name of PivotField |
