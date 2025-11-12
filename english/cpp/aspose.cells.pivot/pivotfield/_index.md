---
title: Aspose::Cells::Pivot::PivotField class
linktitle: PivotField
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Pivot::PivotField class. Represents a field in a PivotTable report in C++.'
type: docs
weight: 1000
url: /cpp/aspose.cells.pivot/pivotfield/
---
## PivotField class


Represents a field in a [PivotTable](../pivottable/) report.

```cpp
class PivotField
```

## Methods

| Method | Description |
| --- | --- |
| [AddCalculatedItem(const U16String\& name, const U16String\& formula)](./addcalculateditem/) | Add a calculated formula item to the pivot field. |
| [AddCalculatedItem(const char16_t* name, const char16_t* formula)](./addcalculateditem/) | Add a calculated formula item to the pivot field. |
| [ClearFilter()](./clearfilter/) | Clears filter setting on this pivot field. |
| [FilterByDate(PivotFilterType type, const Date\& dateTime1, const Date\& dateTime2)](./filterbydate/) | Filters by date values of row or column pivot field. |
| [FilterByLabel(PivotFilterType type, const U16String\& label1, const U16String\& label2)](./filterbylabel/) | Filters by captions of row or column pivot field. |
| [FilterByLabel(PivotFilterType type, const char16_t* label1, const char16_t* label2)](./filterbylabel/) | Filters by captions of row or column pivot field. |
| [FilterByValue(int32_t valueFieldIndex, PivotFilterType type, double value1, double value2)](./filterbyvalue/) | Filters by values of data pivot field. |
| [FilterTop10(int32_t valueFieldIndex, PivotFilterType type, bool isTop, int32_t itemCount)](./filtertop10/) | Filters by values of data pivot field. |
| [Get_NumberFormat()](./get_numberformat/) | Represents the custom display format of numbers and dates. |
| [GetAutoShowCount()](./getautoshowcount/) | Represent the number of top or bottom items that are automatically shown in the specified [PivotTable](../pivottable/) field. |
| [GetAutoShowField()](./getautoshowfield/) | Represents auto show field index. -1 means [PivotField](./) itself. It should be the index of the data fields. |
| [GetAutoSortField()](./getautosortfield/) | Represents the index of field which is auto sorted. -1 means [PivotField](./) itself,others means the position of the data fields. |
| [GetBaseIndex()](./getbaseindex/) | Represents the index in the source pivot fields. |
| [GetCurrentPageItem()](./getcurrentpageitem/) | Represents the current selected page item of the page field to filter data. Only valid for page fields. |
| [GetDisplayName()](./getdisplayname/) | Represents the display name of pivot field in the pivot table view. |
| [GetDragToColumn()](./getdragtocolumn/) | Indicates whether the specified field can be dragged to the column position. The default value is true. |
| [GetDragToData()](./getdragtodata/) | Indicates whether the specified field can be dragged to the values region. The default value is true. |
| [GetDragToHide()](./getdragtohide/) | Indicates whether the specified field can be dragged to the hide region. The default value is true. |
| [GetDragToPage()](./getdragtopage/) | Indicates whether the specified field can be dragged to the page position. The default value is true. |
| [GetDragToRow()](./getdragtorow/) | Indicates whether the specified field can be dragged to the row region. The default value is true. |
| [GetFilters()](./getfilters/) | Gets all pivot filters applied for this pivot field. |
| [GetFormula()](./getformula/) | Gets the formula of the calculated field . Only works for calculated field. |
| [GetFunction()](./getfunction/) | Represents the function used to summarize this [PivotTable](../pivottable/) data field. |
| [GetGroupSettings()](./getgroupsettings/) | Gets the group settings of the pivot field. |
| [GetInsertBlankRow()](./getinsertblankrow/) | Indicates whether to insert a blank line after each item. |
| [GetItemCount()](./getitemcount/) | Gets the count of the base items in this pivot field. |
| [GetItems()](./getitems/) | Get all labels of pivot items in this field. |
| [GetName()](./getname/) | Represents the name of [PivotField](./). |
| [GetNonAutoSortDefault()](./getnonautosortdefault/) | Indicates whether a sort operation that will be applied to this pivot field is an autosort operation or a simple data sort. |
| [GetNumber()](./getnumber/) | Represents the built-in display format of numbers and dates. |
| [GetOriginalItems()](./getoriginalitems/) | Get the original base items;. |
| [GetPivotFilterByType(PivotFilterType type)](./getpivotfilterbytype/) | Gets the pivot filter of the pivot field by type. |
| [GetPivotItems()](./getpivotitems/) | Gets the pivot items of the pivot field. |
| [GetPosition()](./getposition/) | Represents the index of [PivotField](./) in the region. |
| [GetRegionType()](./getregiontype/) | Specifies the region of the [PivotTable](../pivottable/) that this field is displayed. |
| [GetShowAllItems()](./getshowallitems/) | Indicates whether to display all items in the [PivotTable](../pivottable/) view, even if they don't contain summary data. The default value is false. |
| [GetShowCompact()](./getshowcompact/) | Indicates whether to display labels of the next field in the same column on the [Pivot](../) Table view. |
| [GetShowInOutlineForm()](./getshowinoutlineform/) | Indicates whether to layout this field in outline form on the [Pivot](../) Table view. |
| [GetShowSubtotalAtTop()](./getshowsubtotalattop/) | Indicates whether to display subtotals at the top or bottom of items when ShowInOutlineForm is true, then. |
| [GetShowValuesSetting()](./getshowvaluessetting/) | Gets the settings of showing values as when the ShowDataAs calculation is in use. |
| [GetSortSetting()](./getsortsetting/) | Gets all settings of auto sorting. |
| [GetSubtotals(PivotFieldSubtotalType subtotalType)](./getsubtotals/) | Indicates whether to show specified subtotal for this pivot field. |
| [GroupBy(double interval, bool newField)](./groupby/) | Automatically group the field with internal. |
| [GroupBy(const Date\& start, const Date\& end, const Vector \<PivotGroupByType\>\& groups, double interval, bool firstAsNewField)](./groupby/) | Group the file by the date group types. |
| [GroupBy(double start, double end, double interval, bool newField)](./groupby/) | Group the file by number. |
| [GroupBy(const Vector \<CustomPiovtFieldGroupItem\>\& customGroupItems, bool newField)](./groupby/) | Custom group the field. |
| [HideDetail(bool isHiddenDetail)](./hidedetail/) | Sets whether the detail of all PivotItems in a pivot field are hidden. That is collapse/expand this field. |
| [HideItem(int32_t index, bool isHidden)](./hideitem/) | Sets whether the specific [PivotItem](../pivotitem/) in a data field is hidden. |
| [HideItem(const U16String\& itemValue, bool isHidden)](./hideitem/) | Sets whether the specific [PivotItem](../pivotitem/) in a data field is hidden. |
| [HideItem(const char16_t* itemValue, bool isHidden)](./hideitem/) | Sets whether the specific [PivotItem](../pivotitem/) in a data field is hidden. |
| [HideItemDetail(int32_t index, bool isHiddenDetail)](./hideitemdetail/) | Sets whether the specific [PivotItem](../pivotitem/) in a pivot field is hidden detail. |
| [InitPivotItems()](./initpivotitems/) | Init the pivot items of the pivot field. |
| [IsAscendShow()](./isascendshow/) | Indicates whether the specified [PivotTable](../pivottable/) field is autoshown ascending. |
| [IsAscendSort()](./isascendsort/) | Indicates whether the items of this pivot field is autosorted ascending. |
| [IsAutoShow()](./isautoshow/) | Indicates whether the specified [PivotTable](../pivottable/) field is automatically shown. |
| [IsAutoSort()](./isautosort/) | Indicates whether the items of this [PivotTable](../pivottable/) field are automatically sorted. |
| [IsAutoSubtotals()](./isautosubtotals/) | Indicates whether the specified field shows automatic subtotals. Default is true. |
| [IsCalculatedField()](./iscalculatedfield/) | Indicates whether the this pivot field is calculated field. |
| [IsHiddenItem(int32_t index)](./ishiddenitem/) | Gets whether the specific [PivotItem](../pivotitem/) is hidden. |
| [IsHiddenItemDetail(int32_t index)](./ishiddenitemdetail/) | Gets whether to hide the detail of the specific [PivotItem](../pivotitem/).. |
| [IsIncludeNewItemsInFilter()](./isincludenewitemsinfilter/) | Indicates whether to include new items to the field in manual filter. The default value is false. |
| [IsInsertPageBreaksBetweenItems()](./isinsertpagebreaksbetweenitems/) | Indicates whether to insert page breaks after each item. The default value is false. |
| [IsMultipleItemSelectionAllowed()](./ismultipleitemselectionallowed/) | Indicates whether multiple items could be selected in the page field. The default value is false. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsRepeatItemLabels()](./isrepeatitemlabels/) | Indicates whether to repeat labels of the field in the region. The default value is false. |
| [IsValuesField()](./isvaluesfield/) | Indicates whether this field represents values field. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const PivotField\& src)](./operator_asm/) | operator= |
| [PivotField(PivotField_Impl* impl)](./pivotfield/) | Constructs from an implementation object. |
| [PivotField(const PivotField\& src)](./pivotfield/) | Copy constructor. |
| [SetAutoShowCount(int32_t value)](./setautoshowcount/) | Represent the number of top or bottom items that are automatically shown in the specified [PivotTable](../pivottable/) field. |
| [SetAutoShowField(int32_t value)](./setautoshowfield/) | Represents auto show field index. -1 means [PivotField](./) itself. It should be the index of the data fields. |
| [SetAutoSortField(int32_t value)](./setautosortfield/) | Represents the index of field which is auto sorted. -1 means [PivotField](./) itself,others means the position of the data fields. |
| [SetBaseIndex(int32_t value)](./setbaseindex/) | Represents the index in the source pivot fields. |
| [SetCurrentPageItem(int16_t value)](./setcurrentpageitem/) | Represents the current selected page item of the page field to filter data. Only valid for page fields. |
| [SetDisplayName(const U16String\& value)](./setdisplayname/) | Represents the display name of pivot field in the pivot table view. |
| [SetDisplayName(const char16_t* value)](./setdisplayname/) | Represents the display name of pivot field in the pivot table view. |
| [SetDragToColumn(bool value)](./setdragtocolumn/) | Indicates whether the specified field can be dragged to the column position. The default value is true. |
| [SetDragToData(bool value)](./setdragtodata/) | Indicates whether the specified field can be dragged to the values region. The default value is true. |
| [SetDragToHide(bool value)](./setdragtohide/) | Indicates whether the specified field can be dragged to the hide region. The default value is true. |
| [SetDragToPage(bool value)](./setdragtopage/) | Indicates whether the specified field can be dragged to the page position. The default value is true. |
| [SetDragToRow(bool value)](./setdragtorow/) | Indicates whether the specified field can be dragged to the row region. The default value is true. |
| [SetFunction(ConsolidationFunction value)](./setfunction/) | Represents the function used to summarize this [PivotTable](../pivottable/) data field. |
| [SetInsertBlankRow(bool value)](./setinsertblankrow/) | Indicates whether to insert a blank line after each item. |
| [SetIsAscendShow(bool value)](./setisascendshow/) | Indicates whether the specified [PivotTable](../pivottable/) field is autoshown ascending. |
| [SetIsAscendSort(bool value)](./setisascendsort/) | Indicates whether the items of this pivot field is autosorted ascending. |
| [SetIsAutoShow(bool value)](./setisautoshow/) | Indicates whether the specified [PivotTable](../pivottable/) field is automatically shown. |
| [SetIsAutoSort(bool value)](./setisautosort/) | Indicates whether the items of this [PivotTable](../pivottable/) field are automatically sorted. |
| [SetIsAutoSubtotals(bool value)](./setisautosubtotals/) | Indicates whether the specified field shows automatic subtotals. Default is true. |
| [SetIsIncludeNewItemsInFilter(bool value)](./setisincludenewitemsinfilter/) | Indicates whether to include new items to the field in manual filter. The default value is false. |
| [SetIsInsertPageBreaksBetweenItems(bool value)](./setisinsertpagebreaksbetweenitems/) | Indicates whether to insert page breaks after each item. The default value is false. |
| [SetIsMultipleItemSelectionAllowed(bool value)](./setismultipleitemselectionallowed/) | Indicates whether multiple items could be selected in the page field. The default value is false. |
| [SetIsRepeatItemLabels(bool value)](./setisrepeatitemlabels/) | Indicates whether to repeat labels of the field in the region. The default value is false. |
| [SetName(const U16String\& value)](./setname/) | Represents the name of [PivotField](./). |
| [SetName(const char16_t* value)](./setname/) | Represents the name of [PivotField](./). |
| [SetNonAutoSortDefault(bool value)](./setnonautosortdefault/) | Indicates whether a sort operation that will be applied to this pivot field is an autosort operation or a simple data sort. |
| [SetNumber(int32_t value)](./setnumber/) | Represents the built-in display format of numbers and dates. |
| [SetNumberFormat(const U16String\& value)](./setnumberformat/) | Represents the custom display format of numbers and dates. |
| [SetNumberFormat(const char16_t* value)](./setnumberformat/) | Represents the custom display format of numbers and dates. |
| [SetShowAllItems(bool value)](./setshowallitems/) | Indicates whether to display all items in the [PivotTable](../pivottable/) view, even if they don't contain summary data. The default value is false. |
| [SetShowCompact(bool value)](./setshowcompact/) | Indicates whether to display labels of the next field in the same column on the [Pivot](../) Table view. |
| [SetShowInOutlineForm(bool value)](./setshowinoutlineform/) | Indicates whether to layout this field in outline form on the [Pivot](../) Table view. |
| [SetShowSubtotalAtTop(bool value)](./setshowsubtotalattop/) | Indicates whether to display subtotals at the top or bottom of items when ShowInOutlineForm is true, then. |
| [SetSubtotals(PivotFieldSubtotalType subtotalType, bool shown)](./setsubtotals/) | Sets how to subtotal the specified field. |
| [ShowValuesAs(PivotFieldDataDisplayFormat displayFormat, int32_t baseField, PivotItemPositionType baseItemPositionType, int32_t baseItem)](./showvaluesas/) | Shows values of data field as different display format when the ShowDataAs calculation is in use. |
| [SortBy(SortOrder sortType, int32_t fieldSortedBy)](./sortby/) | Sorts this pivot field. |
| [SortBy(SortOrder sortType, int32_t fieldSortedBy, PivotLineType dataType, const U16String\& cellName)](./sortby/) | Sorts this pivot field. |
| [SortBy(SortOrder sortType, int32_t fieldSortedBy, PivotLineType dataType, const char16_t* cellName)](./sortby/) | Sorts this pivot field. |
| [Ungroup()](./ungroup/) | Ungroup the pivot field. |
| [~PivotField()](./~pivotfield/) | Destructor. |
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

pivot.RefreshData();
pivot.CalculateData();


book.Save("out.xlsx");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Pivot](../)
* Library [Aspose.Cells for C++](../../)
