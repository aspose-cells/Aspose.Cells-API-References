---
title: PivotField
second_title: Aspose.Cells for Java API Reference
description: Represents a field in a PivotTable report.
type: docs
url: /java/com.aspose.cells/pivotfield/
---

**Inheritance:**
java.lang.Object
```
public class PivotField
```

Represents a field in a PivotTable report.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         int pivotIndex = pivots.add("=Sheet1!A1:C9", "A12", "TestPivotTable");
         PivotTable pivot = pivots.get(pivotIndex);
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         //Change PivotField's attributes
         PivotField rowField = pivot.getRowFields().get(0);
         rowField.setDisplayName("custom display name");
 
         pivot.refreshData();
         pivot.calculateData();
 
         //do your business
 
         book.save("out.xlsx");
```
## Methods

| Method | Description |
| --- | --- |
| [addCalculatedItem(String name, String formula)](#addCalculatedItem-java.lang.String-java.lang.String-) | Add a calculated formula item to the pivot field. |
| [clearFilter()](#clearFilter--) | Clears filter setting on this pivot field. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filterByDate(int type, DateTime dateTime1, DateTime dateTime2)](#filterByDate-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-) | Filters by date values of row or column pivot field. |
| [filterByLabel(int type, String label1, String label2)](#filterByLabel-int-java.lang.String-java.lang.String-) | Filters by captions of row or column pivot field. |
| [filterByValue(int valueFieldIndex, int type, double value1, double value2)](#filterByValue-int-int-double-double-) | Filters by values of data pivot field. |
| [filterTop10(int valueFieldIndex, int type, boolean isTop, int itemCount)](#filterTop10-int-int-boolean-int-) | Filters by values of data pivot field. |
| [getAutoShowCount()](#getAutoShowCount--) | Represent the number of top or bottom items that are automatically shown in the specified PivotTable field. |
| [getAutoShowField()](#getAutoShowField--) | Represents auto show field index. -1 means PivotField itself. |
| [getAutoSortField()](#getAutoSortField--) | Represents the index of field which is auto sorted |
| [getBaseFieldIndex()](#getBaseFieldIndex--) | Represents the base field for a custom calculation when the ShowDataAs calculation is in use. |
| [getBaseIndex()](#getBaseIndex--) | Represents the index in the source pivot fields. |
| [getBaseItemIndex()](#getBaseItemIndex--) | Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. |
| [getBaseItemPosition()](#getBaseItemPosition--) | Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. |
| [getCalculatedFieldFormula()](#getCalculatedFieldFormula--) | Get the formula string of the specified calculated field . |
| [getClass()](#getClass--) |  |
| [getCurrentPageItem()](#getCurrentPageItem--) | Represents the current selected page item of the page field to filter data. |
| [getDataDisplayFormat()](#getDataDisplayFormat--) | Represents how to display the values in a data field of the pivot report. |
| [getDisplayName()](#getDisplayName--) | Represents the display name of pivot field in the pivot table view. |
| [getDragToColumn()](#getDragToColumn--) | Indicates whether the specified field can be dragged to the column position. |
| [getDragToData()](#getDragToData--) | Indicates whether the specified field can be dragged to the values region. |
| [getDragToHide()](#getDragToHide--) | Indicates whether the specified field can be dragged to the hide region. |
| [getDragToPage()](#getDragToPage--) | Indicates whether the specified field can be dragged to the page position. |
| [getDragToRow()](#getDragToRow--) | Indicates whether the specified field can be dragged to the row region. |
| [getFilters()](#getFilters--) | Gets all pivot filters applied for this pivot field. |
| [getFormula()](#getFormula--) | Gets the formula of the calculated field . |
| [getFunction()](#getFunction--) | Represents the function used to summarize this PivotTable data field. |
| [getGroupSettings()](#getGroupSettings--) | Gets the group settings of the pivot field. |
| [getInsertBlankRow()](#getInsertBlankRow--) | Indicates whether to insert a blank line after each item. |
| [getItemCount()](#getItemCount--) | Gets the count of the base items in this pivot field. |
| [getItems()](#getItems--) | Get all labels of pivot items in this field. |
| [getMaxValue()](#getMaxValue--) | Gets the max value of this field. |
| [getMinValue()](#getMinValue--) | Gets the max value of this field. |
| [getName()](#getName--) | Represents the name of PivotField. |
| [getNonAutoSortDefault()](#getNonAutoSortDefault--) | Indicates whether a sort operation that will be applied to this pivot field is an autosort operation or a simple data sort. |
| [getNumber()](#getNumber--) | Represents the built-in display format of numbers and dates. |
| [getNumberFormat()](#getNumberFormat--) | Represents the custom display format of numbers and dates. |
| [getOriginalItems()](#getOriginalItems--) | Get the original base items; |
| [getPivotFilterByType(int type)](#getPivotFilterByType-int-) | Gets the pivot filter of the pivot field by type |
| [getPivotFilters()](#getPivotFilters--) | Gets the pivot filters of the pivot field |
| [getPivotItems()](#getPivotItems--) | Gets the pivot items of the pivot field |
| [getPosition()](#getPosition--) | Represents the index of [PivotField](../../com.aspose.cells/pivotfield) in the region. |
| [getRegionType()](#getRegionType--) | Specifies the region of the PivotTable that this field is displayed. |
| [getShowAllItems()](#getShowAllItems--) | Indicates whether to display all items in the PivotTable view, even if they don't contain summary data. |
| [getShowCompact()](#getShowCompact--) | Indicates whether to display labels of the next field in the same column on the Pivot Table view |
| [getShowInOutlineForm()](#getShowInOutlineForm--) | Indicates whether to layout this field in outline form on the Pivot Table view. |
| [getShowSubtotalAtTop()](#getShowSubtotalAtTop--) | Indicates whether to display subtotals at the top or bottom of items when ShowInOutlineForm is true, then |
| [getShowValuesSetting()](#getShowValuesSetting--) | Gets the settings of showing values as when the ShowDataAs calculation is in use. |
| [getSortSetting()](#getSortSetting--) | Gets all settings of auto sorting |
| [getSubtotals(int subtotalType)](#getSubtotals-int-) | Indicates whether to show specified subtotal for this pivot field. |
| [groupBy(boolean isAutoStart, DateTime start, boolean isAutoEnd, DateTime end, int[] groups, double interval, boolean firstAsNewField)](#groupBy-boolean-com.aspose.cells.DateTime-boolean-com.aspose.cells.DateTime-int---double-boolean-) | Group the file by the date group types. |
| [groupBy(boolean isAutoStart, double start, boolean isAutoEnd, double end, double interval, boolean newField)](#groupBy-boolean-double-boolean-double-double-boolean-) | Group the file by number. |
| [groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField)](#groupBy-com.aspose.cells.CustomPiovtFieldGroupItem---boolean-) | Custom group the field. |
| [groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField)](#groupBy-com.aspose.cells.DateTime-com.aspose.cells.DateTime-int---double-boolean-) | Group the file by the date group types. |
| [groupBy(double interval, boolean newField)](#groupBy-double-boolean-) | Automatically group the field with internal |
| [groupBy(double start, double end, double interval, boolean newField)](#groupBy-double-double-double-boolean-) | Group the file by number. |
| [groupBy(int[] groups, double interval, boolean newField)](#groupBy-int---double-boolean-) | Automatically group the field with internal |
| [hashCode()](#hashCode--) |  |
| [hideDetail(boolean isHiddenDetail)](#hideDetail-boolean-) | Sets whether the detail of all PivotItems in a pivot field are hidden. |
| [hideItem(int index, boolean isHidden)](#hideItem-int-boolean-) | Sets whether the specific PivotItem in a data field is hidden. |
| [hideItem(String itemValue, boolean isHidden)](#hideItem-java.lang.String-boolean-) | Sets whether the specific PivotItem in a data field is hidden. |
| [hideItemDetail(int index, boolean isHiddenDetail)](#hideItemDetail-int-boolean-) | Sets whether the specific PivotItem in a pivot field is hidden detail. |
| [initPivotItems()](#initPivotItems--) | Init the pivot items of the pivot field |
| [isAscendShow()](#isAscendShow--) | Indicates whether the specified PivotTable field is autoshown ascending. |
| [isAscendSort()](#isAscendSort--) | Indicates whether the items of this pivot field is autosorted ascending. |
| [isAutoShow()](#isAutoShow--) | Indicates whether the specified PivotTable field is automatically shown. |
| [isAutoSort()](#isAutoSort--) | Indicates whether the items of this PivotTable field are automatically sorted. |
| [isAutoSubtotals()](#isAutoSubtotals--) | Indicates whether the specified field shows automatic subtotals. |
| [isCalculatedField()](#isCalculatedField--) | Indicates whether the this pivot field is calculated field. |
| [isHiddenItem(int index)](#isHiddenItem-int-) | Gets whether the specific PivotItem is hidden. |
| [isHiddenItemDetail(int index)](#isHiddenItemDetail-int-) | Gets whether to hide the detail of the specific PivotItem.. |
| [isIncludeNewItemsInFilter()](#isIncludeNewItemsInFilter--) | Indicates whether to include new items to the field in manual filter. |
| [isInsertPageBreaksBetweenItems()](#isInsertPageBreaksBetweenItems--) | Indicates whether to insert page breaks after each item. |
| [isMultipleItemSelectionAllowed()](#isMultipleItemSelectionAllowed--) | Indicates whether multiple items could be selected in the page field. |
| [isRepeatItemLabels()](#isRepeatItemLabels--) | Indicates whether to repeat labels of the field in the region. |
| [isValueFields()](#isValueFields--) | Indicates whether this field represents values fields. |
| [isValuesField()](#isValuesField--) | Indicates whether this field represents values field. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAscendShow(boolean value)](#setAscendShow-boolean-) | Indicates whether the specified PivotTable field is autoshown ascending. |
| [setAscendSort(boolean value)](#setAscendSort-boolean-) | Indicates whether the items of this pivot field is autosorted ascending. |
| [setAutoShow(boolean value)](#setAutoShow-boolean-) | Indicates whether the specified PivotTable field is automatically shown. |
| [setAutoShowCount(int value)](#setAutoShowCount-int-) | Represent the number of top or bottom items that are automatically shown in the specified PivotTable field. |
| [setAutoShowField(int value)](#setAutoShowField-int-) | Represents auto show field index. -1 means PivotField itself. |
| [setAutoSort(boolean value)](#setAutoSort-boolean-) | Indicates whether the items of this PivotTable field are automatically sorted. |
| [setAutoSortField(int value)](#setAutoSortField-int-) | Represents the index of field which is auto sorted |
| [setAutoSubtotals(boolean value)](#setAutoSubtotals-boolean-) | Indicates whether the specified field shows automatic subtotals. |
| [setBaseFieldIndex(int value)](#setBaseFieldIndex-int-) | Represents the base field for a custom calculation when the ShowDataAs calculation is in use. |
| [setBaseIndex(int value)](#setBaseIndex-int-) | Represents the index in the source pivot fields. |
| [setBaseItemIndex(int value)](#setBaseItemIndex-int-) | Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. |
| [setBaseItemPosition(int value)](#setBaseItemPosition-int-) | Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. |
| [setCurrentPageItem(short value)](#setCurrentPageItem-short-) | Represents the current selected page item of the page field to filter data. |
| [setDataDisplayFormat(int value)](#setDataDisplayFormat-int-) | Represents how to display the values in a data field of the pivot report. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Represents the display name of pivot field in the pivot table view. |
| [setDragToColumn(boolean value)](#setDragToColumn-boolean-) | Indicates whether the specified field can be dragged to the column position. |
| [setDragToData(boolean value)](#setDragToData-boolean-) | Indicates whether the specified field can be dragged to the values region. |
| [setDragToHide(boolean value)](#setDragToHide-boolean-) | Indicates whether the specified field can be dragged to the hide region. |
| [setDragToPage(boolean value)](#setDragToPage-boolean-) | Indicates whether the specified field can be dragged to the page position. |
| [setDragToRow(boolean value)](#setDragToRow-boolean-) | Indicates whether the specified field can be dragged to the row region. |
| [setFunction(int value)](#setFunction-int-) | Represents the function used to summarize this PivotTable data field. |
| [setIncludeNewItemsInFilter(boolean value)](#setIncludeNewItemsInFilter-boolean-) | Indicates whether to include new items to the field in manual filter. |
| [setInsertBlankRow(boolean value)](#setInsertBlankRow-boolean-) | Indicates whether to insert a blank line after each item. |
| [setInsertPageBreaksBetweenItems(boolean value)](#setInsertPageBreaksBetweenItems-boolean-) | Indicates whether to insert page breaks after each item. |
| [setMultipleItemSelectionAllowed(boolean value)](#setMultipleItemSelectionAllowed-boolean-) | Indicates whether multiple items could be selected in the page field. |
| [setName(String value)](#setName-java.lang.String-) | Represents the name of PivotField. |
| [setNonAutoSortDefault(boolean value)](#setNonAutoSortDefault-boolean-) | Indicates whether a sort operation that will be applied to this pivot field is an autosort operation or a simple data sort. |
| [setNumber(int value)](#setNumber-int-) | Represents the built-in display format of numbers and dates. |
| [setNumberFormat(String value)](#setNumberFormat-java.lang.String-) | Represents the custom display format of numbers and dates. |
| [setRepeatItemLabels(boolean value)](#setRepeatItemLabels-boolean-) | Indicates whether to repeat labels of the field in the region. |
| [setShowAllItems(boolean value)](#setShowAllItems-boolean-) | Indicates whether to display all items in the PivotTable view, even if they don't contain summary data. |
| [setShowCompact(boolean value)](#setShowCompact-boolean-) | Indicates whether to display labels of the next field in the same column on the Pivot Table view |
| [setShowInOutlineForm(boolean value)](#setShowInOutlineForm-boolean-) | Indicates whether to layout this field in outline form on the Pivot Table view. |
| [setShowSubtotalAtTop(boolean value)](#setShowSubtotalAtTop-boolean-) | Indicates whether to display subtotals at the top or bottom of items when ShowInOutlineForm is true, then |
| [setSubtotals(int subtotalType, boolean shown)](#setSubtotals-int-boolean-) | Sets how to subtotal the specified field. |
| [showValuesAs(int displayFormat, int baseField, int baseItemPositionType, int baseItem)](#showValuesAs-int-int-int-int-) | Shows values of data field as different display format when the ShowDataAs calculation is in use. |
| [sortBy(int sortType, int fieldSortedBy)](#sortBy-int-int-) | Sorts this pivot field. |
| [sortBy(int sortType, int fieldSortedBy, int dataType, String cellName)](#sortBy-int-int-int-java.lang.String-) | Sorts this pivot field. |
| [toString()](#toString--) |  |
| [ungroup()](#ungroup--) | Ungroup the pivot field. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addCalculatedItem(String name, String formula) {#addCalculatedItem-java.lang.String-java.lang.String-}
```
public void addCalculatedItem(String name, String formula)
```


Add a calculated formula item to the pivot field.

**Remarks**

Only supports to add calculated item to Row/Column field.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The item's name. |
| formula | java.lang.String | The formula of pivot item. |

### clearFilter() {#clearFilter--}
```
public void clearFilter()
```


Clears filter setting on this pivot field.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### filterByDate(int type, DateTime dateTime1, DateTime dateTime2) {#filterByDate-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-}
```
public PivotFilter filterByDate(int type, DateTime dateTime1, DateTime dateTime2)
```


Filters by date values of row or column pivot field.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). The type of filtering data. |
| dateTime1 | [DateTime](../../com.aspose.cells/datetime) | The date label of filter condition |
| dateTime2 | [DateTime](../../com.aspose.cells/datetime) | The upper-bound date label of between filter condition |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### filterByLabel(int type, String label1, String label2) {#filterByLabel-int-java.lang.String-java.lang.String-}
```
public PivotFilter filterByLabel(int type, String label1, String label2)
```


Filters by captions of row or column pivot field.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). The type of filtering data. |
| label1 | java.lang.String | The label of filter condition |
| label2 | java.lang.String | The upper-bound label of between filter condition |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### filterByValue(int valueFieldIndex, int type, double value1, double value2) {#filterByValue-int-int-double-double-}
```
public PivotFilter filterByValue(int valueFieldIndex, int type, double value1, double value2)
```


Filters by values of data pivot field.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| valueFieldIndex | int | The index of value field in the value region. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). The type of filtering data. |
| value1 | double | The value of filter condition |
| value2 | double | The upper-bound value of between filter condition |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### filterTop10(int valueFieldIndex, int type, boolean isTop, int itemCount) {#filterTop10-int-int-boolean-int-}
```
public PivotFilter filterTop10(int valueFieldIndex, int type, boolean isTop, int itemCount)
```


Filters by values of data pivot field.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| valueFieldIndex | int | The index of data field in the data region. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). The type of filtering data. Only can be Count,Sum and Percent. |
| isTop | boolean | Indicates whether filter from top or bottom |
| itemCount | int | The item count |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### getAutoShowCount() {#getAutoShowCount--}
```
public int getAutoShowCount()
```


Represent the number of top or bottom items that are automatically shown in the specified PivotTable field.

**Returns:**
int
### getAutoShowField() {#getAutoShowField--}
```
public int getAutoShowField()
```


Represents auto show field index. -1 means PivotField itself. It should be the index of the data fields.

**Returns:**
int
### getAutoSortField() {#getAutoSortField--}
```
public int getAutoSortField()
```


Represents the index of field which is auto sorted. -1 means PivotField itself,others means the position of the data fields.

**Returns:**
int
### getBaseFieldIndex() {#getBaseFieldIndex--}
```
public int getBaseFieldIndex()
```


Represents the base field for a custom calculation when the ShowDataAs calculation is in use.

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotField.ShowValuesSetting.BaseFieldIndex property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getBaseIndex() {#getBaseIndex--}
```
public int getBaseIndex()
```


Represents the index in the source pivot fields.

**Returns:**
int
### getBaseItemIndex() {#getBaseItemIndex--}
```
public int getBaseItemIndex()
```


Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for data fields.

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotField.ShowValuesSetting.BaseItemIndex property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getBaseItemPosition() {#getBaseItemPosition--}
```
public int getBaseItemPosition()
```


Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for data fields. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute.

See [PivotItemPosition](../../com.aspose.cells/pivotitemposition).

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotField.ShowValuesSetting.BaseItemPositionType property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getCalculatedFieldFormula() {#getCalculatedFieldFormula--}
```
public String getCalculatedFieldFormula()
```


Get the formula string of the specified calculated field .

**Remarks**

NOTE: This method is now obsolete. Instead, please use PivotField.GetFormula() method. This method will be removed 12 months later since August 2024. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrentPageItem() {#getCurrentPageItem--}
```
public short getCurrentPageItem()
```


Represents the current selected page item of the page field to filter data. Only valid for page fields.

**Returns:**
short
### getDataDisplayFormat() {#getDataDisplayFormat--}
```
public int getDataDisplayFormat()
```


Represents how to display the values in a data field of the pivot report.

See [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat).

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotField.ShowValuesSetting.CalculationType property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Represents the display name of pivot field in the pivot table view.

**Returns:**
java.lang.String
### getDragToColumn() {#getDragToColumn--}
```
public boolean getDragToColumn()
```


Indicates whether the specified field can be dragged to the column position. The default value is true.

**Returns:**
boolean
### getDragToData() {#getDragToData--}
```
public boolean getDragToData()
```


Indicates whether the specified field can be dragged to the values region. The default value is true.

**Returns:**
boolean
### getDragToHide() {#getDragToHide--}
```
public boolean getDragToHide()
```


Indicates whether the specified field can be dragged to the hide region. The default value is true.

**Returns:**
boolean
### getDragToPage() {#getDragToPage--}
```
public boolean getDragToPage()
```


Indicates whether the specified field can be dragged to the page position. The default value is true.

**Returns:**
boolean
### getDragToRow() {#getDragToRow--}
```
public boolean getDragToRow()
```


Indicates whether the specified field can be dragged to the row region. The default value is true.

**Returns:**
boolean
### getFilters() {#getFilters--}
```
public PivotFilter[] getFilters()
```


Gets all pivot filters applied for this pivot field.

**Returns:**
com.aspose.cells.PivotFilter[]
### getFormula() {#getFormula--}
```
public String getFormula()
```


Gets the formula of the calculated field . Only works for calculated field.

**Returns:**
java.lang.String
### getFunction() {#getFunction--}
```
public int getFunction()
```


Represents the function used to summarize this PivotTable data field.

See [ConsolidationFunction](../../com.aspose.cells/consolidationfunction).

**Returns:**
int
### getGroupSettings() {#getGroupSettings--}
```
public PivotFieldGroupSettings getGroupSettings()
```


Gets the group settings of the pivot field.

**Remarks**

If this field is not grouped, Null will be returned.

**Returns:**
[PivotFieldGroupSettings](../../com.aspose.cells/pivotfieldgroupsettings)
### getInsertBlankRow() {#getInsertBlankRow--}
```
public boolean getInsertBlankRow()
```


Indicates whether to insert a blank line after each item.

**Returns:**
boolean
### getItemCount() {#getItemCount--}
```
public int getItemCount()
```


Gets the count of the base items in this pivot field.

**Returns:**
int
### getItems() {#getItems--}
```
public String[] getItems()
```


Get all labels of pivot items in this field.

**Returns:**
java.lang.String[]
### getMaxValue() {#getMaxValue--}
```
public CellValue getMaxValue()
```


Gets the max value of this field.

**Remarks**

Only works for row or column fields which value must be date time, number or blank.

**Returns:**
[CellValue](../../com.aspose.cells/cellvalue) - 
### getMinValue() {#getMinValue--}
```
public CellValue getMinValue()
```


Gets the max value of this field.

**Remarks**

Only works for row or column fields which value must be date time, number or blank.

**Returns:**
[CellValue](../../com.aspose.cells/cellvalue) - 
### getName() {#getName--}
```
public String getName()
```


Represents the name of PivotField.

**Returns:**
java.lang.String
### getNonAutoSortDefault() {#getNonAutoSortDefault--}
```
public boolean getNonAutoSortDefault()
```


Indicates whether a sort operation that will be applied to this pivot field is an autosort operation or a simple data sort.

**Returns:**
boolean
### getNumber() {#getNumber--}
```
public int getNumber()
```


Represents the built-in display format of numbers and dates.

**Returns:**
int
### getNumberFormat() {#getNumberFormat--}
```
public String getNumberFormat()
```


Represents the custom display format of numbers and dates.

**Returns:**
java.lang.String
### getOriginalItems() {#getOriginalItems--}
```
public String[] getOriginalItems()
```


Get the original base items;

**Returns:**
java.lang.String[]
### getPivotFilterByType(int type) {#getPivotFilterByType-int-}
```
public PivotFilter getPivotFilterByType(int type)
```


Gets the pivot filter of the pivot field by type

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int |  |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### getPivotFilters() {#getPivotFilters--}
```
public ArrayList getPivotFilters()
```


Gets the pivot filters of the pivot field

**Remarks**

NOTE: This method is now obsolete. Instead, please use PivotField.GetFilters() method. This method will be removed 12 months later since November 2023. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
java.util.ArrayList
### getPivotItems() {#getPivotItems--}
```
public PivotItemCollection getPivotItems()
```


Gets the pivot items of the pivot field

**Returns:**
[PivotItemCollection](../../com.aspose.cells/pivotitemcollection)
### getPosition() {#getPosition--}
```
public int getPosition()
```


Represents the index of [PivotField](../../com.aspose.cells/pivotfield) in the region.

**Returns:**
int
### getRegionType() {#getRegionType--}
```
public int getRegionType()
```


Specifies the region of the PivotTable that this field is displayed.

See [PivotFieldType](../../com.aspose.cells/pivotfieldtype).

**Returns:**
int
### getShowAllItems() {#getShowAllItems--}
```
public boolean getShowAllItems()
```


Indicates whether to display all items in the PivotTable view, even if they don't contain summary data. The default value is false.

**Returns:**
boolean
### getShowCompact() {#getShowCompact--}
```
public boolean getShowCompact()
```


Indicates whether to display labels of the next field in the same column on the Pivot Table view

**Returns:**
boolean
### getShowInOutlineForm() {#getShowInOutlineForm--}
```
public boolean getShowInOutlineForm()
```


Indicates whether to layout this field in outline form on the Pivot Table view.

**Returns:**
boolean
### getShowSubtotalAtTop() {#getShowSubtotalAtTop--}
```
public boolean getShowSubtotalAtTop()
```


Indicates whether to display subtotals at the top or bottom of items when ShowInOutlineForm is true, then

**Remarks**

Only works when ShowInOutlineForm is true.

**Returns:**
boolean
### getShowValuesSetting() {#getShowValuesSetting--}
```
public PivotShowValuesSetting getShowValuesSetting()
```


Gets the settings of showing values as when the ShowDataAs calculation is in use.

**Returns:**
[PivotShowValuesSetting](../../com.aspose.cells/pivotshowvaluessetting)
### getSortSetting() {#getSortSetting--}
```
public PivotFieldSortSetting getSortSetting()
```


Gets all settings of auto sorting

**Returns:**
[PivotFieldSortSetting](../../com.aspose.cells/pivotfieldsortsetting)
### getSubtotals(int subtotalType) {#getSubtotals-int-}
```
public boolean getSubtotals(int subtotalType)
```


Indicates whether to show specified subtotal for this pivot field.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). Subtotal type. |

**Returns:**
boolean - Returns whether showing specified subtotal.
### groupBy(boolean isAutoStart, DateTime start, boolean isAutoEnd, DateTime end, int[] groups, double interval, boolean firstAsNewField) {#groupBy-boolean-com.aspose.cells.DateTime-boolean-com.aspose.cells.DateTime-int---double-boolean-}
```
public boolean groupBy(boolean isAutoStart, DateTime start, boolean isAutoEnd, DateTime end, int[] groups, double interval, boolean firstAsNewField)
```


Group the file by the date group types.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isAutoStart | boolean | Indicates whether to auto detect the start date time value. |
| start | [DateTime](../../com.aspose.cells/datetime) | The start datetime |
| isAutoEnd | boolean | Indicates whether to auto detect the end date time value. |
| end | [DateTime](../../com.aspose.cells/datetime) | The end of datetime |
| groups | int[] | [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype). Group types |
| interval | double | The interval |
| firstAsNewField | boolean | Indicates whether adding a new field to the pivottable. Only for the first group item. |

**Returns:**
boolean - False means this field could not be grouped by date time.
### groupBy(boolean isAutoStart, double start, boolean isAutoEnd, double end, double interval, boolean newField) {#groupBy-boolean-double-boolean-double-double-boolean-}
```
public boolean groupBy(boolean isAutoStart, double start, boolean isAutoEnd, double end, double interval, boolean newField)
```


Group the file by number.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isAutoStart | boolean | Indicates whether to auto detect the start value. |
| start | double | The start value |
| isAutoEnd | boolean | Indicates whether to auto detect the end value. |
| end | double | The end of value |
| interval | double | The interval |
| newField | boolean | Indicates whether adding a new field to the pivottable |

**Returns:**
boolean - False means this field could not be grouped by date time.
### groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField) {#groupBy-com.aspose.cells.CustomPiovtFieldGroupItem---boolean-}
```
public boolean groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField)
```


Custom group the field.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| customGroupItems | [CustomPiovtFieldGroupItem\[\]](../../com.aspose.cells/custompiovtfieldgroupitem) | The custom group items. |
| newField | boolean | Indicates whether adding a new field to the pivottable |

**Returns:**
boolean - False means this field could not be grouped by date time.
### groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField) {#groupBy-com.aspose.cells.DateTime-com.aspose.cells.DateTime-int---double-boolean-}
```
public boolean groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField)
```


Group the file by the date group types.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| start | [DateTime](../../com.aspose.cells/datetime) | The start datetime |
| end | [DateTime](../../com.aspose.cells/datetime) | The end of datetime |
| groups | int[] | [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype). Group types |
| interval | double | The interval |
| firstAsNewField | boolean | Indicates whether adding a new field to the pivottable. Only for the first group item. |

**Returns:**
boolean - False means this field could not be grouped by date time.
### groupBy(double interval, boolean newField) {#groupBy-double-boolean-}
```
public void groupBy(double interval, boolean newField)
```


Automatically group the field with internal

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| interval | double | The internal of group. Automatic value will be assigned if it's zero, |
| newField | boolean | Indicates whether adding a new field to the pivottable. |

### groupBy(double start, double end, double interval, boolean newField) {#groupBy-double-double-double-boolean-}
```
public boolean groupBy(double start, double end, double interval, boolean newField)
```


Group the file by number.

**Remarks**

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| start | double | The start value |
| end | double | The end of value |
| interval | double | The interval |
| newField | boolean | Indicates whether adding a new field to the pivottable |

**Returns:**
boolean - False means this field could not be grouped by date time.
### groupBy(int[] groups, double interval, boolean newField) {#groupBy-int---double-boolean-}
```
public void groupBy(int[] groups, double interval, boolean newField)
```


Automatically group the field with internal

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| groups | int[] | [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype). Group types |
| interval | double | The internal of group. Automatic value will be assigned if it's zero, |
| newField | boolean | Indicates whether adding a new field to the pivottable. |

### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### hideDetail(boolean isHiddenDetail) {#hideDetail-boolean-}
```
public void hideDetail(boolean isHiddenDetail)
```


Sets whether the detail of all PivotItems in a pivot field are hidden. That is collapse/expand this field.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isHiddenDetail | boolean | Whether hide the detail of the pivot field. |

### hideItem(int index, boolean isHidden) {#hideItem-int-boolean-}
```
public void hideItem(int index, boolean isHidden)
```


Sets whether the specific PivotItem in a data field is hidden.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | the index of the pivotItem in the pivotField. |
| isHidden | boolean | whether the specific PivotItem is hidden |

### hideItem(String itemValue, boolean isHidden) {#hideItem-java.lang.String-boolean-}
```
public void hideItem(String itemValue, boolean isHidden)
```


Sets whether the specific PivotItem in a data field is hidden.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| itemValue | java.lang.String | The name of the pivotItem in the pivotField. |
| isHidden | boolean | Whether the specific PivotItem is hidden |

### hideItemDetail(int index, boolean isHiddenDetail) {#hideItemDetail-int-boolean-}
```
public void hideItemDetail(int index, boolean isHiddenDetail)
```


Sets whether the specific PivotItem in a pivot field is hidden detail.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | the index of the pivotItem in the pivotField. |
| isHiddenDetail | boolean | whether the specific PivotItem is hidden |

### initPivotItems() {#initPivotItems--}
```
public void initPivotItems()
```


Init the pivot items of the pivot field

### isAscendShow() {#isAscendShow--}
```
public boolean isAscendShow()
```


Indicates whether the specified PivotTable field is autoshown ascending.

**Returns:**
boolean
### isAscendSort() {#isAscendSort--}
```
public boolean isAscendSort()
```


Indicates whether the items of this pivot field is autosorted ascending.

**Returns:**
boolean
### isAutoShow() {#isAutoShow--}
```
public boolean isAutoShow()
```


Indicates whether the specified PivotTable field is automatically shown.

**Remarks**

Only valid for excel 2003.

**Returns:**
boolean
### isAutoSort() {#isAutoSort--}
```
public boolean isAutoSort()
```


Indicates whether the items of this PivotTable field are automatically sorted.

**Returns:**
boolean
### isAutoSubtotals() {#isAutoSubtotals--}
```
public boolean isAutoSubtotals()
```


Indicates whether the specified field shows automatic subtotals. Default is true.

**Returns:**
boolean
### isCalculatedField() {#isCalculatedField--}
```
public boolean isCalculatedField()
```


Indicates whether the this pivot field is calculated field.

**Returns:**
boolean
### isHiddenItem(int index) {#isHiddenItem-int-}
```
public boolean isHiddenItem(int index)
```


Gets whether the specific PivotItem is hidden.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The index of the pivotItem in the pivotField. |

**Returns:**
boolean - whether the specific PivotItem is hidden
### isHiddenItemDetail(int index) {#isHiddenItemDetail-int-}
```
public boolean isHiddenItemDetail(int index)
```


Gets whether to hide the detail of the specific PivotItem..

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The index of the pivotItem in the pivotField. |

**Returns:**
boolean - whether the specific PivotItem is hidden detail
### isIncludeNewItemsInFilter() {#isIncludeNewItemsInFilter--}
```
public boolean isIncludeNewItemsInFilter()
```


Indicates whether to include new items to the field in manual filter. The default value is false.

**Returns:**
boolean
### isInsertPageBreaksBetweenItems() {#isInsertPageBreaksBetweenItems--}
```
public boolean isInsertPageBreaksBetweenItems()
```


Indicates whether to insert page breaks after each item. The default value is false.

**Returns:**
boolean
### isMultipleItemSelectionAllowed() {#isMultipleItemSelectionAllowed--}
```
public boolean isMultipleItemSelectionAllowed()
```


Indicates whether multiple items could be selected in the page field. The default value is false.

**Returns:**
boolean
### isRepeatItemLabels() {#isRepeatItemLabels--}
```
public boolean isRepeatItemLabels()
```


Indicates whether to repeat labels of the field in the region. The default value is false.

**Returns:**
boolean
### isValueFields() {#isValueFields--}
```
public boolean isValueFields()
```


Indicates whether this field represents values fields.

**Remarks**

NOTE: This method is now obsolete. Instead, please use PivotField.IsValuesField property. This method will be removed 12 months later since November 2023. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### isValuesField() {#isValuesField--}
```
public boolean isValuesField()
```


Indicates whether this field represents values field.

**Remarks**

Only works when there are two or more data fields in the pivot table view.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAscendShow(boolean value) {#setAscendShow-boolean-}
```
public void setAscendShow(boolean value)
```


Indicates whether the specified PivotTable field is autoshown ascending.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAscendSort(boolean value) {#setAscendSort-boolean-}
```
public void setAscendSort(boolean value)
```


Indicates whether the items of this pivot field is autosorted ascending.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutoShow(boolean value) {#setAutoShow-boolean-}
```
public void setAutoShow(boolean value)
```


Indicates whether the specified PivotTable field is automatically shown.

**Remarks**

Only valid for excel 2003.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutoShowCount(int value) {#setAutoShowCount-int-}
```
public void setAutoShowCount(int value)
```


Represent the number of top or bottom items that are automatically shown in the specified PivotTable field.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setAutoShowField(int value) {#setAutoShowField-int-}
```
public void setAutoShowField(int value)
```


Represents auto show field index. -1 means PivotField itself. It should be the index of the data fields.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setAutoSort(boolean value) {#setAutoSort-boolean-}
```
public void setAutoSort(boolean value)
```


Indicates whether the items of this PivotTable field are automatically sorted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutoSortField(int value) {#setAutoSortField-int-}
```
public void setAutoSortField(int value)
```


Represents the index of field which is auto sorted. -1 means PivotField itself,others means the position of the data fields.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setAutoSubtotals(boolean value) {#setAutoSubtotals-boolean-}
```
public void setAutoSubtotals(boolean value)
```


Indicates whether the specified field shows automatic subtotals. Default is true.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setBaseFieldIndex(int value) {#setBaseFieldIndex-int-}
```
public void setBaseFieldIndex(int value)
```


Represents the base field for a custom calculation when the ShowDataAs calculation is in use.

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotField.ShowValuesSetting.BaseFieldIndex property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBaseIndex(int value) {#setBaseIndex-int-}
```
public void setBaseIndex(int value)
```


Represents the index in the source pivot fields.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBaseItemIndex(int value) {#setBaseItemIndex-int-}
```
public void setBaseItemIndex(int value)
```


Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for data fields.

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotField.ShowValuesSetting.BaseItemIndex property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBaseItemPosition(int value) {#setBaseItemPosition-int-}
```
public void setBaseItemPosition(int value)
```


Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for data fields. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute.

See [PivotItemPosition](../../com.aspose.cells/pivotitemposition).

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotField.ShowValuesSetting.BaseItemPositionType property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setCurrentPageItem(short value) {#setCurrentPageItem-short-}
```
public void setCurrentPageItem(short value)
```


Represents the current selected page item of the page field to filter data. Only valid for page fields.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | short |  |

### setDataDisplayFormat(int value) {#setDataDisplayFormat-int-}
```
public void setDataDisplayFormat(int value)
```


Represents how to display the values in a data field of the pivot report.

See [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat).

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotField.ShowValuesSetting.CalculationType property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Represents the display name of pivot field in the pivot table view.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setDragToColumn(boolean value) {#setDragToColumn-boolean-}
```
public void setDragToColumn(boolean value)
```


Indicates whether the specified field can be dragged to the column position. The default value is true.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDragToData(boolean value) {#setDragToData-boolean-}
```
public void setDragToData(boolean value)
```


Indicates whether the specified field can be dragged to the values region. The default value is true.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDragToHide(boolean value) {#setDragToHide-boolean-}
```
public void setDragToHide(boolean value)
```


Indicates whether the specified field can be dragged to the hide region. The default value is true.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDragToPage(boolean value) {#setDragToPage-boolean-}
```
public void setDragToPage(boolean value)
```


Indicates whether the specified field can be dragged to the page position. The default value is true.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDragToRow(boolean value) {#setDragToRow-boolean-}
```
public void setDragToRow(boolean value)
```


Indicates whether the specified field can be dragged to the row region. The default value is true.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFunction(int value) {#setFunction-int-}
```
public void setFunction(int value)
```


Represents the function used to summarize this PivotTable data field.

See [ConsolidationFunction](../../com.aspose.cells/consolidationfunction).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setIncludeNewItemsInFilter(boolean value) {#setIncludeNewItemsInFilter-boolean-}
```
public void setIncludeNewItemsInFilter(boolean value)
```


Indicates whether to include new items to the field in manual filter. The default value is false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setInsertBlankRow(boolean value) {#setInsertBlankRow-boolean-}
```
public void setInsertBlankRow(boolean value)
```


Indicates whether to insert a blank line after each item.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setInsertPageBreaksBetweenItems(boolean value) {#setInsertPageBreaksBetweenItems-boolean-}
```
public void setInsertPageBreaksBetweenItems(boolean value)
```


Indicates whether to insert page breaks after each item. The default value is false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setMultipleItemSelectionAllowed(boolean value) {#setMultipleItemSelectionAllowed-boolean-}
```
public void setMultipleItemSelectionAllowed(boolean value)
```


Indicates whether multiple items could be selected in the page field. The default value is false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Represents the name of PivotField.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setNonAutoSortDefault(boolean value) {#setNonAutoSortDefault-boolean-}
```
public void setNonAutoSortDefault(boolean value)
```


Indicates whether a sort operation that will be applied to this pivot field is an autosort operation or a simple data sort.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setNumber(int value) {#setNumber-int-}
```
public void setNumber(int value)
```


Represents the built-in display format of numbers and dates.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setNumberFormat(String value) {#setNumberFormat-java.lang.String-}
```
public void setNumberFormat(String value)
```


Represents the custom display format of numbers and dates.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setRepeatItemLabels(boolean value) {#setRepeatItemLabels-boolean-}
```
public void setRepeatItemLabels(boolean value)
```


Indicates whether to repeat labels of the field in the region. The default value is false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowAllItems(boolean value) {#setShowAllItems-boolean-}
```
public void setShowAllItems(boolean value)
```


Indicates whether to display all items in the PivotTable view, even if they don't contain summary data. The default value is false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowCompact(boolean value) {#setShowCompact-boolean-}
```
public void setShowCompact(boolean value)
```


Indicates whether to display labels of the next field in the same column on the Pivot Table view

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowInOutlineForm(boolean value) {#setShowInOutlineForm-boolean-}
```
public void setShowInOutlineForm(boolean value)
```


Indicates whether to layout this field in outline form on the Pivot Table view.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowSubtotalAtTop(boolean value) {#setShowSubtotalAtTop-boolean-}
```
public void setShowSubtotalAtTop(boolean value)
```


Indicates whether to display subtotals at the top or bottom of items when ShowInOutlineForm is true, then

**Remarks**

Only works when ShowInOutlineForm is true.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSubtotals(int subtotalType, boolean shown) {#setSubtotals-int-boolean-}
```
public void setSubtotals(int subtotalType, boolean shown)
```


Sets how to subtotal the specified field.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) |
| shown | boolean | Whether the specified field shows that subtotals. |

### showValuesAs(int displayFormat, int baseField, int baseItemPositionType, int baseItem) {#showValuesAs-int-int-int-int-}
```
public void showValuesAs(int displayFormat, int baseField, int baseItemPositionType, int baseItem)
```


Shows values of data field as different display format when the ShowDataAs calculation is in use.

**Remarks**

Only for data field.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| displayFormat | int | [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat). The data display format type. |
| baseField | int | The index to the field which ShowDataAs calculation bases on. |
| baseItemPositionType | int | [PivotItemPositionType](../../com.aspose.cells/pivotitempositiontype). The position type of base iteam. |
| baseItem | int | The index to the base item which ShowDataAs calculation bases on. Only works when baseItemPositionType is custom. |

### sortBy(int sortType, int fieldSortedBy) {#sortBy-int-int-}
```
public void sortBy(int sortType, int fieldSortedBy)
```


Sorts this pivot field.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). The type of sorting this field. |
| fieldSortedBy | int | The index of pivot field sorted by. -1 means sorting by data labels of this field, others mean the index of data field sorted by. |

### sortBy(int sortType, int fieldSortedBy, int dataType, String cellName) {#sortBy-int-int-int-java.lang.String-}
```
public void sortBy(int sortType, int fieldSortedBy, int dataType, String cellName)
```


Sorts this pivot field.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). The type of sorting this field. |
| fieldSortedBy | int | The index of pivot field sorted by. -1 means sorting by data labels of this field, others mean the index of data field sorted by. |
| dataType | int | [PivotLineType](../../com.aspose.cells/pivotlinetype). The type of data sorted by. |
| cellName | java.lang.String | Sort by values in the row or column |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### ungroup() {#ungroup--}
```
public void ungroup()
```


Ungroup the pivot field.

### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

