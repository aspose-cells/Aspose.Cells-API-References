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
| [addCalculatedItem(String name, String formula)](#addCalculatedItem-java.lang.String-java.lang.String-) | Add a calculated item to the pivot field. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoShowCount()](#getAutoShowCount--) | Represent the number of top or bottom items that are automatically shown in the specified PivotTable field. |
| [getAutoShowField()](#getAutoShowField--) | Represents auto show field index. -1 means PivotField itself. |
| [getAutoSortField()](#getAutoSortField--) | Represents auto sort field index |
| [getBaseFieldIndex()](#getBaseFieldIndex--) | Represents the base field for a custom calculation. |
| [getBaseIndex()](#getBaseIndex--) | Represents the PivotField index in the base PivotFields. |
| [getBaseItemIndex()](#getBaseItemIndex--) | Represents the item in the base field for a custom calculation. |
| [getBaseItemPosition()](#getBaseItemPosition--) | Represents the item in the base field for a custom calculation. |
| [getCalculatedFieldFormula()](#getCalculatedFieldFormula--) | Get the formula string of the specified calculated field . |
| [getClass()](#getClass--) |  |
| [getCurrentPageItem()](#getCurrentPageItem--) | Represents the current page item showing for the page field (valid only for page fields). |
| [getDataDisplayFormat()](#getDataDisplayFormat--) | Represents how to display the values contained in a data field. |
| [getDisplayName()](#getDisplayName--) | Represents the PivotField display name. |
| [getDragToColumn()](#getDragToColumn--) | Indicates whether the specified field can be dragged to the column position. |
| [getDragToData()](#getDragToData--) | Indicates whether the specified field can be dragged to the data position. |
| [getDragToHide()](#getDragToHide--) | Indicates whether the specified field can be dragged to the hide position. |
| [getDragToPage()](#getDragToPage--) | Indicates whether the specified field can be dragged to the page position. |
| [getDragToRow()](#getDragToRow--) | Indicates whether the specified field can be dragged to the row position. |
| [getFunction()](#getFunction--) | Represents the function used to summarize the PivotTable data field. |
| [getGroupSettings()](#getGroupSettings--) | Gets the group settings of the pivot field. |
| [getInsertBlankRow()](#getInsertBlankRow--) | Indicates whether inserting blank line after each item. |
| [getItemCount()](#getItemCount--) | Gets the base item count of this pivot field. |
| [getItems()](#getItems--) | Get all base items; |
| [getName()](#getName--) | Represents the PivotField name. |
| [getNonAutoSortDefault()](#getNonAutoSortDefault--) | Indicates whether a sort operation that will be applied to this pivot field is an autosort operation or a simple data sort. |
| [getNumber()](#getNumber--) | Represents the built-in display format of numbers and dates. |
| [getNumberFormat()](#getNumberFormat--) | Represents the custom display format of numbers and dates. |
| [getOriginalItems()](#getOriginalItems--) | Get the original base items; |
| [getPivotFilterByType(int type)](#getPivotFilterByType-int-) | Gets the pivot filter of the pivot field by type |
| [getPivotFilters()](#getPivotFilters--) | Gets the pivot filters of the pivot field |
| [getPivotItems()](#getPivotItems--) | Gets the pivot items of the pivot field |
| [getPosition()](#getPosition--) | Represents the PivotField index in the PivotFields. |
| [getRange()](#getRange--) | Gets the group range of the pivot field |
| [getShowAllItems()](#getShowAllItems--) | Indicates whether all items displays in the PivotTable report, even if they don't contain summary data. |
| [getShowCompact()](#getShowCompact--) | Indicates whether display labels from the next field in the same column on the Pivot Table view |
| [getShowInOutlineForm()](#getShowInOutlineForm--) | Indicates whether layout this field in outline form on the Pivot Table view |
| [getShowSubtotalAtTop()](#getShowSubtotalAtTop--) | when ShowInOutlineForm is true, then display subtotals at the top of the list of items instead of at the bottom |
| [getSubtotals(int subtotalType)](#getSubtotals-int-) | Gets whether the specified field shows that subtotals. |
| [groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField)](#groupBy-com.aspose.cells.CustomPiovtFieldGroupItem---boolean-) | Custom group the field. |
| [groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField)](#groupBy-com.aspose.cells.DateTime-com.aspose.cells.DateTime-int---double-boolean-) | Group the file by the date group types. |
| [groupBy(double start, double end, double interval, boolean newField)](#groupBy-double-double-double-boolean-) | Group the file by number. |
| [hashCode()](#hashCode--) |  |
| [hideDetail(boolean isHiddenDetail)](#hideDetail-boolean-) | Sets whether the PivotItems in a pivot field is hidden detail.That is collapse/expand this field. |
| [hideItem(int index, boolean isHidden)](#hideItem-int-boolean-) | Sets whether the specific PivotItem in a data field is hidden. |
| [hideItem(String itemValue, boolean isHidden)](#hideItem-java.lang.String-boolean-) | Sets whether the specific PivotItem in a data field is hidden. |
| [hideItemDetail(int index, boolean isHiddenDetail)](#hideItemDetail-int-boolean-) | Sets whether the specific PivotItem in a pivot field is hidden detail. |
| [initPivotItems()](#initPivotItems--) | Init the pivot items of the pivot field |
| [isAscendShow()](#isAscendShow--) | Indicates whether the specified PivotTable field is autoshown ascending. |
| [isAscendSort()](#isAscendSort--) | Indicates whether the specified PivotTable field is autosorted ascending. |
| [isAutoShow()](#isAutoShow--) | Indicates whether the specified PivotTable field is automatically shown,only valid for excel 2003. |
| [isAutoSort()](#isAutoSort--) | Indicates whether the specified PivotTable field is automatically sorted. |
| [isAutoSubtotals()](#isAutoSubtotals--) | Indicates whether the specified field shows automatic subtotals. |
| [isCalculatedField()](#isCalculatedField--) | Indicates whether the specified PivotTable field is calculated field. |
| [isHiddenItem(int index)](#isHiddenItem-int-) | Indicates whether the specific PivotItem is hidden. |
| [isHiddenItemDetail(int index)](#isHiddenItemDetail-int-) | Indicates whether the specific PivotItem is hidden detail. |
| [isIncludeNewItemsInFilter()](#isIncludeNewItemsInFilter--) | indicates whether the field can include new items in manual filter The default value is false. |
| [isInsertPageBreaksBetweenItems()](#isInsertPageBreaksBetweenItems--) | indicates whether the field can insert page breaks between items insert page break after each item The default value is false. |
| [isMultipleItemSelectionAllowed()](#isMultipleItemSelectionAllowed--) | indicates whether the field can have multiple items selected in the page field The default value is false. |
| [isRepeatItemLabels()](#isRepeatItemLabels--) | indicates whether the field can repeat items labels The default value is false. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAscendShow(boolean value)](#setAscendShow-boolean-) | Indicates whether the specified PivotTable field is autoshown ascending. |
| [setAscendSort(boolean value)](#setAscendSort-boolean-) | Indicates whether the specified PivotTable field is autosorted ascending. |
| [setAutoShow(boolean value)](#setAutoShow-boolean-) | Indicates whether the specified PivotTable field is automatically shown,only valid for excel 2003. |
| [setAutoShowCount(int value)](#setAutoShowCount-int-) | Represent the number of top or bottom items that are automatically shown in the specified PivotTable field. |
| [setAutoShowField(int value)](#setAutoShowField-int-) | Represents auto show field index. -1 means PivotField itself. |
| [setAutoSort(boolean value)](#setAutoSort-boolean-) | Indicates whether the specified PivotTable field is automatically sorted. |
| [setAutoSortField(int value)](#setAutoSortField-int-) | Represents auto sort field index |
| [setAutoSubtotals(boolean value)](#setAutoSubtotals-boolean-) | Indicates whether the specified field shows automatic subtotals. |
| [setBaseFieldIndex(int value)](#setBaseFieldIndex-int-) | Represents the base field for a custom calculation. |
| [setBaseIndex(int value)](#setBaseIndex-int-) | Represents the PivotField index in the base PivotFields. |
| [setBaseItemIndex(int value)](#setBaseItemIndex-int-) | Represents the item in the base field for a custom calculation. |
| [setBaseItemPosition(int value)](#setBaseItemPosition-int-) | Represents the item in the base field for a custom calculation. |
| [setCurrentPageItem(short value)](#setCurrentPageItem-short-) | Represents the current page item showing for the page field (valid only for page fields). |
| [setDataDisplayFormat(int value)](#setDataDisplayFormat-int-) | Represents how to display the values contained in a data field. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Represents the PivotField display name. |
| [setDragToColumn(boolean value)](#setDragToColumn-boolean-) | Indicates whether the specified field can be dragged to the column position. |
| [setDragToData(boolean value)](#setDragToData-boolean-) | Indicates whether the specified field can be dragged to the data position. |
| [setDragToHide(boolean value)](#setDragToHide-boolean-) | Indicates whether the specified field can be dragged to the hide position. |
| [setDragToPage(boolean value)](#setDragToPage-boolean-) | Indicates whether the specified field can be dragged to the page position. |
| [setDragToRow(boolean value)](#setDragToRow-boolean-) | Indicates whether the specified field can be dragged to the row position. |
| [setFunction(int value)](#setFunction-int-) | Represents the function used to summarize the PivotTable data field. |
| [setIncludeNewItemsInFilter(boolean value)](#setIncludeNewItemsInFilter-boolean-) | indicates whether the field can include new items in manual filter The default value is false. |
| [setInsertBlankRow(boolean value)](#setInsertBlankRow-boolean-) | Indicates whether inserting blank line after each item. |
| [setInsertPageBreaksBetweenItems(boolean value)](#setInsertPageBreaksBetweenItems-boolean-) | indicates whether the field can insert page breaks between items insert page break after each item The default value is false. |
| [setMultipleItemSelectionAllowed(boolean value)](#setMultipleItemSelectionAllowed-boolean-) | indicates whether the field can have multiple items selected in the page field The default value is false. |
| [setName(String value)](#setName-java.lang.String-) | Represents the PivotField name. |
| [setNonAutoSortDefault(boolean value)](#setNonAutoSortDefault-boolean-) | Indicates whether a sort operation that will be applied to this pivot field is an autosort operation or a simple data sort. |
| [setNumber(int value)](#setNumber-int-) | Represents the built-in display format of numbers and dates. |
| [setNumberFormat(String value)](#setNumberFormat-java.lang.String-) | Represents the custom display format of numbers and dates. |
| [setRepeatItemLabels(boolean value)](#setRepeatItemLabels-boolean-) | indicates whether the field can repeat items labels The default value is false. |
| [setShowAllItems(boolean value)](#setShowAllItems-boolean-) | Indicates whether all items displays in the PivotTable report, even if they don't contain summary data. |
| [setShowCompact(boolean value)](#setShowCompact-boolean-) | Indicates whether display labels from the next field in the same column on the Pivot Table view |
| [setShowInOutlineForm(boolean value)](#setShowInOutlineForm-boolean-) | Indicates whether layout this field in outline form on the Pivot Table view |
| [setShowSubtotalAtTop(boolean value)](#setShowSubtotalAtTop-boolean-) | when ShowInOutlineForm is true, then display subtotals at the top of the list of items instead of at the bottom |
| [setSubtotals(int subtotalType, boolean shown)](#setSubtotals-int-boolean-) | Sets whether the specified field shows that subtotals. |
| [toString()](#toString--) |  |
| [ungroup()](#ungroup--) | Ungroup the pivot field. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addCalculatedItem(String name, String formula) {#addCalculatedItem-java.lang.String-java.lang.String-}
```
public void addCalculatedItem(String name, String formula)
```


Add a calculated item to the pivot field.

**Remarks**

Only supports to add calculated item to Row/Column field.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The item's name. |
| formula | java.lang.String | The item's formula |

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


Represents auto sort field index. -1 means PivotField itself,others means the position of the data fields.

**Returns:**
int
### getBaseFieldIndex() {#getBaseFieldIndex--}
```
public int getBaseFieldIndex()
```


Represents the base field for a custom calculation.

**Returns:**
int
### getBaseIndex() {#getBaseIndex--}
```
public int getBaseIndex()
```


Represents the PivotField index in the base PivotFields.

**Returns:**
int
### getBaseItemIndex() {#getBaseItemIndex--}
```
public int getBaseItemIndex()
```


Represents the item in the base field for a custom calculation. Valid only for data fields.

**Returns:**
int
### getBaseItemPosition() {#getBaseItemPosition--}
```
public int getBaseItemPosition()
```


Represents the item in the base field for a custom calculation. Valid only for data fields. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute.

See [PivotItemPosition](../../com.aspose.cells/pivotitemposition).

**Returns:**
int
### getCalculatedFieldFormula() {#getCalculatedFieldFormula--}
```
public String getCalculatedFieldFormula()
```


Get the formula string of the specified calculated field .

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


Represents the current page item showing for the page field (valid only for page fields).

**Returns:**
short
### getDataDisplayFormat() {#getDataDisplayFormat--}
```
public int getDataDisplayFormat()
```


Represents how to display the values contained in a data field.

See [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat).

**Returns:**
int
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Represents the PivotField display name.

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


Indicates whether the specified field can be dragged to the data position. The default value is true.

**Returns:**
boolean
### getDragToHide() {#getDragToHide--}
```
public boolean getDragToHide()
```


Indicates whether the specified field can be dragged to the hide position. The default value is true.

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


Indicates whether the specified field can be dragged to the row position. The default value is true.

**Returns:**
boolean
### getFunction() {#getFunction--}
```
public int getFunction()
```


Represents the function used to summarize the PivotTable data field.

See [ConsolidationFunction](../../com.aspose.cells/consolidationfunction).

**Returns:**
int
### getGroupSettings() {#getGroupSettings--}
```
public PivotFieldGroupSettings getGroupSettings()
```


Gets the group settings of the pivot field.

**Returns:**
[PivotFieldGroupSettings](../../com.aspose.cells/pivotfieldgroupsettings)
### getInsertBlankRow() {#getInsertBlankRow--}
```
public boolean getInsertBlankRow()
```


Indicates whether inserting blank line after each item.

**Returns:**
boolean
### getItemCount() {#getItemCount--}
```
public int getItemCount()
```


Gets the base item count of this pivot field.

**Returns:**
int
### getItems() {#getItems--}
```
public String[] getItems()
```


Get all base items;

**Returns:**
java.lang.String[]
### getName() {#getName--}
```
public String getName()
```


Represents the PivotField name.

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


Represents the PivotField index in the PivotFields.

**Returns:**
int
### getRange() {#getRange--}
```
public SxRng getRange()
```


Gets the group range of the pivot field

**Remarks**

NOTE: This method is now obsolete. Instead, please use PivotField.GroupSettings property. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
[SxRng](../../com.aspose.cells/sxrng)
### getShowAllItems() {#getShowAllItems--}
```
public boolean getShowAllItems()
```


Indicates whether all items displays in the PivotTable report, even if they don't contain summary data. show items with no data The default value is false.

**Returns:**
boolean
### getShowCompact() {#getShowCompact--}
```
public boolean getShowCompact()
```


Indicates whether display labels from the next field in the same column on the Pivot Table view

**Returns:**
boolean
### getShowInOutlineForm() {#getShowInOutlineForm--}
```
public boolean getShowInOutlineForm()
```


Indicates whether layout this field in outline form on the Pivot Table view

**Returns:**
boolean
### getShowSubtotalAtTop() {#getShowSubtotalAtTop--}
```
public boolean getShowSubtotalAtTop()
```


when ShowInOutlineForm is true, then display subtotals at the top of the list of items instead of at the bottom

**Returns:**
boolean
### getSubtotals(int subtotalType) {#getSubtotals-int-}
```
public boolean getSubtotals(int subtotalType)
```


Gets whether the specified field shows that subtotals.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). subtotals type. |

**Returns:**
boolean - whether the specified field shows that subtotals.
### groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField) {#groupBy-com.aspose.cells.CustomPiovtFieldGroupItem---boolean-}
```
public void groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField)
```


Custom group the field.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| customGroupItems | [CustomPiovtFieldGroupItem\[\]](../../com.aspose.cells/custompiovtfieldgroupitem) | The custom group items. |
| newField | boolean | Indicates whether adding a new field to the pivottable |

### groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField) {#groupBy-com.aspose.cells.DateTime-com.aspose.cells.DateTime-int---double-boolean-}
```
public void groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField)
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

### groupBy(double start, double end, double interval, boolean newField) {#groupBy-double-double-double-boolean-}
```
public void groupBy(double start, double end, double interval, boolean newField)
```


Group the file by number.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| start | double | The start value |
| end | double | The end of value |
| interval | double | The interval |
| newField | boolean | Indicates whether adding a new field to the pivottable |

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


Sets whether the PivotItems in a pivot field is hidden detail.That is collapse/expand this field.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isHiddenDetail | boolean | whether the PivotItems is hidden |

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
| itemValue | java.lang.String | the value of the pivotItem in the pivotField. |
| isHidden | boolean | whether the specific PivotItem is hidden |

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


Indicates whether the specified PivotTable field is autosorted ascending.

**Returns:**
boolean
### isAutoShow() {#isAutoShow--}
```
public boolean isAutoShow()
```


Indicates whether the specified PivotTable field is automatically shown,only valid for excel 2003.

**Returns:**
boolean
### isAutoSort() {#isAutoSort--}
```
public boolean isAutoSort()
```


Indicates whether the specified PivotTable field is automatically sorted.

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


Indicates whether the specified PivotTable field is calculated field.

**Returns:**
boolean
### isHiddenItem(int index) {#isHiddenItem-int-}
```
public boolean isHiddenItem(int index)
```


Indicates whether the specific PivotItem is hidden.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | the index of the pivotItem in the pivotField. |

**Returns:**
boolean - whether the specific PivotItem is hidden
### isHiddenItemDetail(int index) {#isHiddenItemDetail-int-}
```
public boolean isHiddenItemDetail(int index)
```


Indicates whether the specific PivotItem is hidden detail.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | the index of the pivotItem in the pivotField. |

**Returns:**
boolean - whether the specific PivotItem is hidden detail
### isIncludeNewItemsInFilter() {#isIncludeNewItemsInFilter--}
```
public boolean isIncludeNewItemsInFilter()
```


indicates whether the field can include new items in manual filter The default value is false.

**Returns:**
boolean
### isInsertPageBreaksBetweenItems() {#isInsertPageBreaksBetweenItems--}
```
public boolean isInsertPageBreaksBetweenItems()
```


indicates whether the field can insert page breaks between items insert page break after each item The default value is false.

**Returns:**
boolean
### isMultipleItemSelectionAllowed() {#isMultipleItemSelectionAllowed--}
```
public boolean isMultipleItemSelectionAllowed()
```


indicates whether the field can have multiple items selected in the page field The default value is false.

**Returns:**
boolean
### isRepeatItemLabels() {#isRepeatItemLabels--}
```
public boolean isRepeatItemLabels()
```


indicates whether the field can repeat items labels The default value is false.

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


Indicates whether the specified PivotTable field is autosorted ascending.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutoShow(boolean value) {#setAutoShow-boolean-}
```
public void setAutoShow(boolean value)
```


Indicates whether the specified PivotTable field is automatically shown,only valid for excel 2003.

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


Indicates whether the specified PivotTable field is automatically sorted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutoSortField(int value) {#setAutoSortField-int-}
```
public void setAutoSortField(int value)
```


Represents auto sort field index. -1 means PivotField itself,others means the position of the data fields.

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


Represents the base field for a custom calculation.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBaseIndex(int value) {#setBaseIndex-int-}
```
public void setBaseIndex(int value)
```


Represents the PivotField index in the base PivotFields.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBaseItemIndex(int value) {#setBaseItemIndex-int-}
```
public void setBaseItemIndex(int value)
```


Represents the item in the base field for a custom calculation. Valid only for data fields.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBaseItemPosition(int value) {#setBaseItemPosition-int-}
```
public void setBaseItemPosition(int value)
```


Represents the item in the base field for a custom calculation. Valid only for data fields. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute.

See [PivotItemPosition](../../com.aspose.cells/pivotitemposition).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setCurrentPageItem(short value) {#setCurrentPageItem-short-}
```
public void setCurrentPageItem(short value)
```


Represents the current page item showing for the page field (valid only for page fields).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | short |  |

### setDataDisplayFormat(int value) {#setDataDisplayFormat-int-}
```
public void setDataDisplayFormat(int value)
```


Represents how to display the values contained in a data field.

See [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Represents the PivotField display name.

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


Indicates whether the specified field can be dragged to the data position. The default value is true.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDragToHide(boolean value) {#setDragToHide-boolean-}
```
public void setDragToHide(boolean value)
```


Indicates whether the specified field can be dragged to the hide position. The default value is true.

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


Indicates whether the specified field can be dragged to the row position. The default value is true.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFunction(int value) {#setFunction-int-}
```
public void setFunction(int value)
```


Represents the function used to summarize the PivotTable data field.

See [ConsolidationFunction](../../com.aspose.cells/consolidationfunction).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setIncludeNewItemsInFilter(boolean value) {#setIncludeNewItemsInFilter-boolean-}
```
public void setIncludeNewItemsInFilter(boolean value)
```


indicates whether the field can include new items in manual filter The default value is false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setInsertBlankRow(boolean value) {#setInsertBlankRow-boolean-}
```
public void setInsertBlankRow(boolean value)
```


Indicates whether inserting blank line after each item.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setInsertPageBreaksBetweenItems(boolean value) {#setInsertPageBreaksBetweenItems-boolean-}
```
public void setInsertPageBreaksBetweenItems(boolean value)
```


indicates whether the field can insert page breaks between items insert page break after each item The default value is false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setMultipleItemSelectionAllowed(boolean value) {#setMultipleItemSelectionAllowed-boolean-}
```
public void setMultipleItemSelectionAllowed(boolean value)
```


indicates whether the field can have multiple items selected in the page field The default value is false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Represents the PivotField name.

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


indicates whether the field can repeat items labels The default value is false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowAllItems(boolean value) {#setShowAllItems-boolean-}
```
public void setShowAllItems(boolean value)
```


Indicates whether all items displays in the PivotTable report, even if they don't contain summary data. show items with no data The default value is false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowCompact(boolean value) {#setShowCompact-boolean-}
```
public void setShowCompact(boolean value)
```


Indicates whether display labels from the next field in the same column on the Pivot Table view

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowInOutlineForm(boolean value) {#setShowInOutlineForm-boolean-}
```
public void setShowInOutlineForm(boolean value)
```


Indicates whether layout this field in outline form on the Pivot Table view

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowSubtotalAtTop(boolean value) {#setShowSubtotalAtTop-boolean-}
```
public void setShowSubtotalAtTop(boolean value)
```


when ShowInOutlineForm is true, then display subtotals at the top of the list of items instead of at the bottom

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSubtotals(int subtotalType, boolean shown) {#setSubtotals-int-boolean-}
```
public void setSubtotals(int subtotalType, boolean shown)
```


Sets whether the specified field shows that subtotals.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). subtotals type. |
| shown | boolean | whether the specified field shows that subtotals. |

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

