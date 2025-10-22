##Aspose::Cells::Pivot::PivotField class
'Aspose::Cells::Pivot::PivotField class. Represents a field in a PivotTable report in C++.'
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
| [FilterByDate(PivotFilterType type, const Date\& dateTime1, const Date\& dateTime2)](./filterbydate/) | Filters by date setting of row or column pivot field. |
| [FilterByLabel(PivotFilterType type, const U16String\& label1, const U16String\& label2)](./filterbylabel/) | Filters by captions of row or column pivot field. |
| [FilterByLabel(PivotFilterType type, const char16_t* label1, const char16_t* label2)](./filterbylabel/) | Filters by captions of row or column pivot field. |
| [FilterByValue(int32_t valueFieldIndex, PivotFilterType type, double value1, double value2)](./filterbyvalue/) | Filters by values of data pivot field. |
| [FilterTop10(int32_t valueFieldIndex, PivotFilterType type, bool isTop, int32_t itemCount)](./filtertop10/) | Filters by values of data pivot field. |
| [Get_NumberFormat()](./get_numberformat/) | Represents the custom display format of numbers and dates. |
| [GetAutoShowCount()](./getautoshowcount/) | Represent the number of top or bottom items that are automatically shown in the specified [PivotTable](../pivottable/) field. |
| [GetAutoShowField()](./getautoshowfield/) | Represents auto show field index. -1 means [PivotField](./) itself. It should be the index of the data fields. |
| [GetAutoSortField()](./getautosortfield/) | Represents the index of field which is auto sorted. -1 means [PivotField](./) itself,others means the position of the data fields. |
| [GetBaseIndex()](./getbaseindex/) | Represents the [PivotField](./) index in the base PivotFields. |
| [GetCurrentPageItem()](./getcurrentpageitem/) | Represents the current page item showing for the page field (valid only for page fields). |
| [GetDisplayName()](./getdisplayname/) | Represents the [PivotField](./) display name. |
| [GetDragToColumn()](./getdragtocolumn/) | Indicates whether the specified field can be dragged to the column position. The default value is true. |
| [GetDragToData()](./getdragtodata/) | Indicates whether the specified field can be dragged to the data position. The default value is true. |
| [GetDragToHide()](./getdragtohide/) | Indicates whether the specified field can be dragged to the hide position. The default value is true. |
| [GetDragToPage()](./getdragtopage/) | Indicates whether the specified field can be dragged to the page position. The default value is true. |
| [GetDragToRow()](./getdragtorow/) | Indicates whether the specified field can be dragged to the row position. The default value is true. |
| [GetFilters()](./getfilters/) | Gets all pivot filters of this pivot field. |
| [GetFormula()](./getformula/) | Gets formula of the calculated field . |
| [GetFunction()](./getfunction/) | Represents the function used to summarize the [PivotTable](../pivottable/) data field. |
| [GetGroupSettings()](./getgroupsettings/) | Gets the group settings of the pivot field. |
| [GetInsertBlankRow()](./getinsertblankrow/) | Indicates whether inserting blank line after each item. |
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
| [GetShowAllItems()](./getshowallitems/) | Indicates whether all items displays in the [PivotTable](../pivottable/) report, even if they don't contain summary data. show items with no data The default value is false. |
| [GetShowCompact()](./getshowcompact/) | Indicates whether display labels from the next field in the same column on the [Pivot](../) Table view. |
| [GetShowInOutlineForm()](./getshowinoutlineform/) | Indicates whether layout this field in outline form on the [Pivot](../) Table view. |
| [GetShowSubtotalAtTop()](./getshowsubtotalattop/) | when ShowInOutlineForm is true, then display subtotals at the top of the list of items instead of at the bottom |
| [GetShowValuesSetting()](./getshowvaluessetting/) | Gets the settings of showing values as when the ShowDataAs calculation is in use. |
| [GetSortSetting()](./getsortsetting/) | Gets all settings of auto sorting. |
| [GetSubtotals(PivotFieldSubtotalType subtotalType)](./getsubtotals/) | Indicates whether showing specified subtotal. |
| [GroupBy(double interval, bool newField)](./groupby/) | Automatically group the field with internal. |
| [GroupBy(const Date\& start, const Date\& end, const Vector \<PivotGroupByType\>\& groups, double interval, bool firstAsNewField)](./groupby/) | Group the file by the date group types. |
| [GroupBy(double start, double end, double interval, bool newField)](./groupby/) | Group the file by number. |
| [GroupBy(const Vector \<CustomPiovtFieldGroupItem\>\& customGroupItems, bool newField)](./groupby/) | Custom group the field. |
| [HideDetail(bool isHiddenDetail)](./hidedetail/) | Sets whether the PivotItems in a pivot field is hidden detail.That is collapse/expand this field. |
| [HideItem(int32_t index, bool isHidden)](./hideitem/) | Sets whether the specific [PivotItem](../pivotitem/) in a data field is hidden. |
| [HideItem(const U16String\& itemValue, bool isHidden)](./hideitem/) | Sets whether the specific [PivotItem](../pivotitem/) in a data field is hidden. |
| [HideItem(const char16_t* itemValue, bool isHidden)](./hideitem/) | Sets whether the specific [PivotItem](../pivotitem/) in a data field is hidden. |
| [HideItemDetail(int32_t index, bool isHiddenDetail)](./hideitemdetail/) | Sets whether the specific [PivotItem](../pivotitem/) in a pivot field is hidden detail. |
| [InitPivotItems()](./initpivotitems/) | Init the pivot items of the pivot field. |
| [IsAscendShow()](./isascendshow/) | Indicates whether the specified [PivotTable](../pivottable/) field is autoshown ascending. |
| [IsAscendSort()](./isascendsort/) | Indicates whether the specified [PivotTable](../pivottable/) field is autosorted ascending. |
| [IsAutoShow()](./isautoshow/) | Indicates whether the specified [PivotTable](../pivottable/) field is automatically shown,only valid for excel 2003. |
| [IsAutoSort()](./isautosort/) | Indicates whether the specified [PivotTable](../pivottable/) field is automatically sorted. |
| [IsAutoSubtotals()](./isautosubtotals/) | Indicates whether the specified field shows automatic subtotals. Default is true. |
| [IsCalculatedField()](./iscalculatedfield/) | Indicates whether the specified [PivotTable](../pivottable/) field is calculated field. |
| [IsHiddenItem(int32_t index)](./ishiddenitem/) | Gets whether the specific [PivotItem](../pivotitem/) is hidden. |
| [IsHiddenItemDetail(int32_t index)](./ishiddenitemdetail/) | Gets whether hidding the detail of the specific [PivotItem](../pivotitem/).. |
| [IsIncludeNewItemsInFilter()](./isincludenewitemsinfilter/) | Indicates whether including new items to the field in manual filter. The default value is false. |
| [IsInsertPageBreaksBetweenItems()](./isinsertpagebreaksbetweenitems/) | Indicates whether inserting page breaks after each item. The default value is false. |
| [IsMultipleItemSelectionAllowed()](./ismultipleitemselectionallowed/) | indicates whether the field can have multiple items selected in the page field The default value is false. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsRepeatItemLabels()](./isrepeatitemlabels/) | Indicates whether repeating labels of the field in the region. The default value is false. |
| [IsValueFields()](./isvaluefields/) | Indicates whether this field represents values fields. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const PivotField\& src)](./operator_asm/) | operator= |
| [PivotField(PivotField_Impl* impl)](./pivotfield/) | Constructs from an implementation object. |
| [PivotField(const PivotField\& src)](./pivotfield/) | Copy constructor. |
| [SetAutoShowCount(int32_t value)](./setautoshowcount/) | Represent the number of top or bottom items that are automatically shown in the specified [PivotTable](../pivottable/) field. |
| [SetAutoShowField(int32_t value)](./setautoshowfield/) | Represents auto show field index. -1 means [PivotField](./) itself. It should be the index of the data fields. |
| [SetAutoSortField(int32_t value)](./setautosortfield/) | Represents the index of field which is auto sorted. -1 means [PivotField](./) itself,others means the position of the data fields. |
| [SetBaseIndex(int32_t value)](./setbaseindex/) | Represents the [PivotField](./) index in the base PivotFields. |
| [SetCurrentPageItem(int16_t value)](./setcurrentpageitem/) | Represents the current page item showing for the page field (valid only for page fields). |
| [SetDisplayName(const U16String\& value)](./setdisplayname/) | Represents the [PivotField](./) display name. |
| [SetDisplayName(const char16_t* value)](./setdisplayname/) | Represents the [PivotField](./) display name. |
| [SetDragToColumn(bool value)](./setdragtocolumn/) | Indicates whether the specified field can be dragged to the column position. The default value is true. |
| [SetDragToData(bool value)](./setdragtodata/) | Indicates whether the specified field can be dragged to the data position. The default value is true. |
| [SetDragToHide(bool value)](./setdragtohide/) | Indicates whether the specified field can be dragged to the hide position. The default value is true. |
| [SetDragToPage(bool value)](./setdragtopage/) | Indicates whether the specified field can be dragged to the page position. The default value is true. |
| [SetDragToRow(bool value)](./setdragtorow/) | Indicates whether the specified field can be dragged to the row position. The default value is true. |
| [SetFunction(ConsolidationFunction value)](./setfunction/) | Represents the function used to summarize the [PivotTable](../pivottable/) data field. |
| [SetInsertBlankRow(bool value)](./setinsertblankrow/) | Indicates whether inserting blank line after each item. |
| [SetIsAscendShow(bool value)](./setisascendshow/) | Indicates whether the specified [PivotTable](../pivottable/) field is autoshown ascending. |
| [SetIsAscendSort(bool value)](./setisascendsort/) | Indicates whether the specified [PivotTable](../pivottable/) field is autosorted ascending. |
| [SetIsAutoShow(bool value)](./setisautoshow/) | Indicates whether the specified [PivotTable](../pivottable/) field is automatically shown,only valid for excel 2003. |
| [SetIsAutoSort(bool value)](./setisautosort/) | Indicates whether the specified [PivotTable](../pivottable/) field is automatically sorted. |
| [SetIsAutoSubtotals(bool value)](./setisautosubtotals/) | Indicates whether the specified field shows automatic subtotals. Default is true. |
| [SetIsIncludeNewItemsInFilter(bool value)](./setisincludenewitemsinfilter/) | Indicates whether including new items to the field in manual filter. The default value is false. |
| [SetIsInsertPageBreaksBetweenItems(bool value)](./setisinsertpagebreaksbetweenitems/) | Indicates whether inserting page breaks after each item. The default value is false. |
| [SetIsMultipleItemSelectionAllowed(bool value)](./setismultipleitemselectionallowed/) | indicates whether the field can have multiple items selected in the page field The default value is false. |
| [SetIsRepeatItemLabels(bool value)](./setisrepeatitemlabels/) | Indicates whether repeating labels of the field in the region. The default value is false. |
| [SetName(const U16String\& value)](./setname/) | Represents the name of [PivotField](./). |
| [SetName(const char16_t* value)](./setname/) | Represents the name of [PivotField](./). |
| [SetNonAutoSortDefault(bool value)](./setnonautosortdefault/) | Indicates whether a sort operation that will be applied to this pivot field is an autosort operation or a simple data sort. |
| [SetNumber(int32_t value)](./setnumber/) | Represents the built-in display format of numbers and dates. |
| [SetNumberFormat(const U16String\& value)](./setnumberformat/) | Represents the custom display format of numbers and dates. |
| [SetNumberFormat(const char16_t* value)](./setnumberformat/) | Represents the custom display format of numbers and dates. |
| [SetShowAllItems(bool value)](./setshowallitems/) | Indicates whether all items displays in the [PivotTable](../pivottable/) report, even if they don't contain summary data. show items with no data The default value is false. |
| [SetShowCompact(bool value)](./setshowcompact/) | Indicates whether display labels from the next field in the same column on the [Pivot](../) Table view. |
| [SetShowInOutlineForm(bool value)](./setshowinoutlineform/) | Indicates whether layout this field in outline form on the [Pivot](../) Table view. |
| [SetShowSubtotalAtTop(bool value)](./setshowsubtotalattop/) | when ShowInOutlineForm is true, then display subtotals at the top of the list of items instead of at the bottom |
| [SetSubtotals(PivotFieldSubtotalType subtotalType, bool shown)](./setsubtotals/) | Sets whether the specified field shows that subtotals. |
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
