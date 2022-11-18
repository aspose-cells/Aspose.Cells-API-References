---
title: PivotField
second_title: Aspose.Cells for Java API Reference
description: Represents a field in a PivotTable report.
type: docs
weight: 396
url: /java/com.aspose.cells/pivotfield/
---

**Inheritance:**
java.lang.Object
```
public class PivotField
```

Represents a field in a PivotTable report.

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
| [getShowAllItems()](#getShowAllItems--) | Indicates whether all items in the PivotTable report are displayed, even if they don't contain summary data. |
| [getShowCompact()](#getShowCompact--) | Indicates whether display labels from the next field in the same column on the Pivot Table view |
| [getShowInOutlineForm()](#getShowInOutlineForm--) | Indicates whether layout this field in outline form on the Pivot Table view |
| [getShowSubtotalAtTop()](#getShowSubtotalAtTop--) | when ShowInOutlineForm is true, then display subtotals at the top of the list of items instead of at the bottom |
| [getSubtotals(int subtotalType)](#getSubtotals-int-) | Gets whether the specified field shows that subtotals. |
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
| [setAscendShow(boolean value)](#setAscendShow-boolean-) | Please see the getter of this property: [isAscendShow()](../../com.aspose.cells/pivotfield\#isAscendShow--) |
| [setAscendSort(boolean value)](#setAscendSort-boolean-) | Please see the getter of this property: [isAscendSort()](../../com.aspose.cells/pivotfield\#isAscendSort--) |
| [setAutoShow(boolean value)](#setAutoShow-boolean-) | Please see the getter of this property: [isAutoShow()](../../com.aspose.cells/pivotfield\#isAutoShow--) |
| [setAutoShowCount(int value)](#setAutoShowCount-int-) | Please see the getter of this property: [getAutoShowCount()](../../com.aspose.cells/pivotfield\#getAutoShowCount--) |
| [setAutoShowField(int value)](#setAutoShowField-int-) | Please see the getter of this property: [getAutoShowField()](../../com.aspose.cells/pivotfield\#getAutoShowField--) |
| [setAutoSort(boolean value)](#setAutoSort-boolean-) | Please see the getter of this property: [isAutoSort()](../../com.aspose.cells/pivotfield\#isAutoSort--) |
| [setAutoSortField(int value)](#setAutoSortField-int-) | Please see the getter of this property: [getAutoSortField()](../../com.aspose.cells/pivotfield\#getAutoSortField--) |
| [setAutoSubtotals(boolean value)](#setAutoSubtotals-boolean-) | Please see the getter of this property: [isAutoSubtotals()](../../com.aspose.cells/pivotfield\#isAutoSubtotals--) |
| [setBaseFieldIndex(int value)](#setBaseFieldIndex-int-) | Please see the getter of this property: [getBaseFieldIndex()](../../com.aspose.cells/pivotfield\#getBaseFieldIndex--) |
| [setBaseIndex(int value)](#setBaseIndex-int-) | Please see the getter of this property: [getBaseIndex()](../../com.aspose.cells/pivotfield\#getBaseIndex--) |
| [setBaseItemIndex(int value)](#setBaseItemIndex-int-) | Please see the getter of this property: [getBaseItemIndex()](../../com.aspose.cells/pivotfield\#getBaseItemIndex--) |
| [setBaseItemPosition(int value)](#setBaseItemPosition-int-) | Please see the getter of this property: [getBaseItemPosition()](../../com.aspose.cells/pivotfield\#getBaseItemPosition--) |
| [setCurrentPageItem(short value)](#setCurrentPageItem-short-) | Please see the getter of this property: [getCurrentPageItem()](../../com.aspose.cells/pivotfield\#getCurrentPageItem--) |
| [setDataDisplayFormat(int value)](#setDataDisplayFormat-int-) | Please see the getter of this property: [getDataDisplayFormat()](../../com.aspose.cells/pivotfield\#getDataDisplayFormat--) |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Please see the getter of this property: [getDisplayName()](../../com.aspose.cells/pivotfield\#getDisplayName--) |
| [setDragToColumn(boolean value)](#setDragToColumn-boolean-) | Please see the getter of this property: [getDragToColumn()](../../com.aspose.cells/pivotfield\#getDragToColumn--) |
| [setDragToData(boolean value)](#setDragToData-boolean-) | Please see the getter of this property: [getDragToData()](../../com.aspose.cells/pivotfield\#getDragToData--) |
| [setDragToHide(boolean value)](#setDragToHide-boolean-) | Please see the getter of this property: [getDragToHide()](../../com.aspose.cells/pivotfield\#getDragToHide--) |
| [setDragToPage(boolean value)](#setDragToPage-boolean-) | Please see the getter of this property: [getDragToPage()](../../com.aspose.cells/pivotfield\#getDragToPage--) |
| [setDragToRow(boolean value)](#setDragToRow-boolean-) | Please see the getter of this property: [getDragToRow()](../../com.aspose.cells/pivotfield\#getDragToRow--) |
| [setFunction(int value)](#setFunction-int-) | Please see the getter of this property: [getFunction()](../../com.aspose.cells/pivotfield\#getFunction--) |
| [setIncludeNewItemsInFilter(boolean value)](#setIncludeNewItemsInFilter-boolean-) | Please see the getter of this property: [isIncludeNewItemsInFilter()](../../com.aspose.cells/pivotfield\#isIncludeNewItemsInFilter--) |
| [setInsertBlankRow(boolean value)](#setInsertBlankRow-boolean-) | Please see the getter of this property: [getInsertBlankRow()](../../com.aspose.cells/pivotfield\#getInsertBlankRow--) |
| [setInsertPageBreaksBetweenItems(boolean value)](#setInsertPageBreaksBetweenItems-boolean-) | Please see the getter of this property: [isInsertPageBreaksBetweenItems()](../../com.aspose.cells/pivotfield\#isInsertPageBreaksBetweenItems--) |
| [setMultipleItemSelectionAllowed(boolean value)](#setMultipleItemSelectionAllowed-boolean-) | Please see the getter of this property: [isMultipleItemSelectionAllowed()](../../com.aspose.cells/pivotfield\#isMultipleItemSelectionAllowed--) |
| [setNonAutoSortDefault(boolean value)](#setNonAutoSortDefault-boolean-) | Please see the getter of this property: [getNonAutoSortDefault()](../../com.aspose.cells/pivotfield\#getNonAutoSortDefault--) |
| [setNumber(int value)](#setNumber-int-) | Please see the getter of this property: [getNumber()](../../com.aspose.cells/pivotfield\#getNumber--) |
| [setNumberFormat(String value)](#setNumberFormat-java.lang.String-) | Please see the getter of this property: [getNumberFormat()](../../com.aspose.cells/pivotfield\#getNumberFormat--) |
| [setRepeatItemLabels(boolean value)](#setRepeatItemLabels-boolean-) | Please see the getter of this property: [isRepeatItemLabels()](../../com.aspose.cells/pivotfield\#isRepeatItemLabels--) |
| [setShowAllItems(boolean value)](#setShowAllItems-boolean-) | Please see the getter of this property: [getShowAllItems()](../../com.aspose.cells/pivotfield\#getShowAllItems--) |
| [setShowCompact(boolean value)](#setShowCompact-boolean-) | Please see the getter of this property: [getShowCompact()](../../com.aspose.cells/pivotfield\#getShowCompact--) |
| [setShowInOutlineForm(boolean value)](#setShowInOutlineForm-boolean-) | Please see the getter of this property: [getShowInOutlineForm()](../../com.aspose.cells/pivotfield\#getShowInOutlineForm--) |
| [setShowSubtotalAtTop(boolean value)](#setShowSubtotalAtTop-boolean-) | Please see the getter of this property: [getShowSubtotalAtTop()](../../com.aspose.cells/pivotfield\#getShowSubtotalAtTop--) |
| [setSubtotals(int subtotalType, boolean shown)](#setSubtotals-int-boolean-) | Sets whether the specified field shows that subtotals. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addCalculatedItem(String name, String formula) {#addCalculatedItem-java.lang.String-java.lang.String-}
```
public void addCalculatedItem(String name, String formula)
```


Add a calculated item to the pivot field. Only supports to add calculated item to Row/Column field.

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

**Returns:**
int
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

**Returns:**
[SxRng](../../com.aspose.cells/sxrng)
### getShowAllItems() {#getShowAllItems--}
```
public boolean getShowAllItems()
```


Indicates whether all items in the PivotTable report are displayed, even if they don't contain summary data. show items with no data The default value is false.

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
| subtotalType | int | subtotals type. |

**Returns:**
boolean - whether the specified field shows that subtotals.
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


Please see the getter of this property: [isAscendShow()](../../com.aspose.cells/pivotfield\#isAscendShow--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAscendSort(boolean value) {#setAscendSort-boolean-}
```
public void setAscendSort(boolean value)
```


Please see the getter of this property: [isAscendSort()](../../com.aspose.cells/pivotfield\#isAscendSort--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutoShow(boolean value) {#setAutoShow-boolean-}
```
public void setAutoShow(boolean value)
```


Please see the getter of this property: [isAutoShow()](../../com.aspose.cells/pivotfield\#isAutoShow--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutoShowCount(int value) {#setAutoShowCount-int-}
```
public void setAutoShowCount(int value)
```


Please see the getter of this property: [getAutoShowCount()](../../com.aspose.cells/pivotfield\#getAutoShowCount--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setAutoShowField(int value) {#setAutoShowField-int-}
```
public void setAutoShowField(int value)
```


Please see the getter of this property: [getAutoShowField()](../../com.aspose.cells/pivotfield\#getAutoShowField--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setAutoSort(boolean value) {#setAutoSort-boolean-}
```
public void setAutoSort(boolean value)
```


Please see the getter of this property: [isAutoSort()](../../com.aspose.cells/pivotfield\#isAutoSort--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutoSortField(int value) {#setAutoSortField-int-}
```
public void setAutoSortField(int value)
```


Please see the getter of this property: [getAutoSortField()](../../com.aspose.cells/pivotfield\#getAutoSortField--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setAutoSubtotals(boolean value) {#setAutoSubtotals-boolean-}
```
public void setAutoSubtotals(boolean value)
```


Please see the getter of this property: [isAutoSubtotals()](../../com.aspose.cells/pivotfield\#isAutoSubtotals--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setBaseFieldIndex(int value) {#setBaseFieldIndex-int-}
```
public void setBaseFieldIndex(int value)
```


Please see the getter of this property: [getBaseFieldIndex()](../../com.aspose.cells/pivotfield\#getBaseFieldIndex--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBaseIndex(int value) {#setBaseIndex-int-}
```
public void setBaseIndex(int value)
```


Please see the getter of this property: [getBaseIndex()](../../com.aspose.cells/pivotfield\#getBaseIndex--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBaseItemIndex(int value) {#setBaseItemIndex-int-}
```
public void setBaseItemIndex(int value)
```


Please see the getter of this property: [getBaseItemIndex()](../../com.aspose.cells/pivotfield\#getBaseItemIndex--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBaseItemPosition(int value) {#setBaseItemPosition-int-}
```
public void setBaseItemPosition(int value)
```


Please see the getter of this property: [getBaseItemPosition()](../../com.aspose.cells/pivotfield\#getBaseItemPosition--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setCurrentPageItem(short value) {#setCurrentPageItem-short-}
```
public void setCurrentPageItem(short value)
```


Please see the getter of this property: [getCurrentPageItem()](../../com.aspose.cells/pivotfield\#getCurrentPageItem--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | short |  |

### setDataDisplayFormat(int value) {#setDataDisplayFormat-int-}
```
public void setDataDisplayFormat(int value)
```


Please see the getter of this property: [getDataDisplayFormat()](../../com.aspose.cells/pivotfield\#getDataDisplayFormat--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Please see the getter of this property: [getDisplayName()](../../com.aspose.cells/pivotfield\#getDisplayName--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setDragToColumn(boolean value) {#setDragToColumn-boolean-}
```
public void setDragToColumn(boolean value)
```


Please see the getter of this property: [getDragToColumn()](../../com.aspose.cells/pivotfield\#getDragToColumn--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDragToData(boolean value) {#setDragToData-boolean-}
```
public void setDragToData(boolean value)
```


Please see the getter of this property: [getDragToData()](../../com.aspose.cells/pivotfield\#getDragToData--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDragToHide(boolean value) {#setDragToHide-boolean-}
```
public void setDragToHide(boolean value)
```


Please see the getter of this property: [getDragToHide()](../../com.aspose.cells/pivotfield\#getDragToHide--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDragToPage(boolean value) {#setDragToPage-boolean-}
```
public void setDragToPage(boolean value)
```


Please see the getter of this property: [getDragToPage()](../../com.aspose.cells/pivotfield\#getDragToPage--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDragToRow(boolean value) {#setDragToRow-boolean-}
```
public void setDragToRow(boolean value)
```


Please see the getter of this property: [getDragToRow()](../../com.aspose.cells/pivotfield\#getDragToRow--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFunction(int value) {#setFunction-int-}
```
public void setFunction(int value)
```


Please see the getter of this property: [getFunction()](../../com.aspose.cells/pivotfield\#getFunction--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setIncludeNewItemsInFilter(boolean value) {#setIncludeNewItemsInFilter-boolean-}
```
public void setIncludeNewItemsInFilter(boolean value)
```


Please see the getter of this property: [isIncludeNewItemsInFilter()](../../com.aspose.cells/pivotfield\#isIncludeNewItemsInFilter--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setInsertBlankRow(boolean value) {#setInsertBlankRow-boolean-}
```
public void setInsertBlankRow(boolean value)
```


Please see the getter of this property: [getInsertBlankRow()](../../com.aspose.cells/pivotfield\#getInsertBlankRow--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setInsertPageBreaksBetweenItems(boolean value) {#setInsertPageBreaksBetweenItems-boolean-}
```
public void setInsertPageBreaksBetweenItems(boolean value)
```


Please see the getter of this property: [isInsertPageBreaksBetweenItems()](../../com.aspose.cells/pivotfield\#isInsertPageBreaksBetweenItems--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setMultipleItemSelectionAllowed(boolean value) {#setMultipleItemSelectionAllowed-boolean-}
```
public void setMultipleItemSelectionAllowed(boolean value)
```


Please see the getter of this property: [isMultipleItemSelectionAllowed()](../../com.aspose.cells/pivotfield\#isMultipleItemSelectionAllowed--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setNonAutoSortDefault(boolean value) {#setNonAutoSortDefault-boolean-}
```
public void setNonAutoSortDefault(boolean value)
```


Please see the getter of this property: [getNonAutoSortDefault()](../../com.aspose.cells/pivotfield\#getNonAutoSortDefault--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setNumber(int value) {#setNumber-int-}
```
public void setNumber(int value)
```


Please see the getter of this property: [getNumber()](../../com.aspose.cells/pivotfield\#getNumber--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setNumberFormat(String value) {#setNumberFormat-java.lang.String-}
```
public void setNumberFormat(String value)
```


Please see the getter of this property: [getNumberFormat()](../../com.aspose.cells/pivotfield\#getNumberFormat--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setRepeatItemLabels(boolean value) {#setRepeatItemLabels-boolean-}
```
public void setRepeatItemLabels(boolean value)
```


Please see the getter of this property: [isRepeatItemLabels()](../../com.aspose.cells/pivotfield\#isRepeatItemLabels--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowAllItems(boolean value) {#setShowAllItems-boolean-}
```
public void setShowAllItems(boolean value)
```


Please see the getter of this property: [getShowAllItems()](../../com.aspose.cells/pivotfield\#getShowAllItems--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowCompact(boolean value) {#setShowCompact-boolean-}
```
public void setShowCompact(boolean value)
```


Please see the getter of this property: [getShowCompact()](../../com.aspose.cells/pivotfield\#getShowCompact--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowInOutlineForm(boolean value) {#setShowInOutlineForm-boolean-}
```
public void setShowInOutlineForm(boolean value)
```


Please see the getter of this property: [getShowInOutlineForm()](../../com.aspose.cells/pivotfield\#getShowInOutlineForm--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowSubtotalAtTop(boolean value) {#setShowSubtotalAtTop-boolean-}
```
public void setShowSubtotalAtTop(boolean value)
```


Please see the getter of this property: [getShowSubtotalAtTop()](../../com.aspose.cells/pivotfield\#getShowSubtotalAtTop--)

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
| subtotalType | int | subtotals type. |
| shown | boolean | whether the specified field shows that subtotals. |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
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

