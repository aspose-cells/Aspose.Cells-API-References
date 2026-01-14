---
title: AutoFilter
second_title: Aspose.Cells for Java API Reference
description: Represents autofiltering for the specified worksheet.
type: docs
url: /java/com.aspose.cells/autofilter/
---

**Inheritance:**
java.lang.Object
```
public class AutoFilter
```

Represents autofiltering for the specified worksheet.

**Example**

```
         //Creating a file stream containing the Excel file to be opened
         //Instantiating a Workbook object
         Workbook workbook = new Workbook("template.xlsx");
         //Accessing the first worksheet in the Excel file
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Creating AutoFilter by giving the cells range of the heading row
         worksheet.getAutoFilter().setRange("A1:B1");
         //Filtering columns with specified values
         worksheet.getAutoFilter().filter(1, "Bananas");
         //Saving the modified Excel file.
         workbook.save("output.xls");
```
## Methods

| Method | Description |
| --- | --- |
| [addDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)](#addDateFilter-int-int-int-int-int-int-int-int-) | Adds a date filter. |
| [addFillColorFilter(int fieldIndex, int pattern, CellsColor foregroundColor, CellsColor backgroundColor)](#addFillColorFilter-int-int-com.aspose.cells.CellsColor-com.aspose.cells.CellsColor-) | Adds a fill color filter. |
| [addFilter(int fieldIndex, String criteria)](#addFilter-int-java.lang.String-) | Adds a filter for a filter column. |
| [addFontColorFilter(int fieldIndex, CellsColor color)](#addFontColorFilter-int-com.aspose.cells.CellsColor-) | Adds a font color filter. |
| [addIconFilter(int fieldIndex, int iconSetType, int iconId)](#addIconFilter-int-int-int-) | Adds an icon filter. |
| [custom(int fieldIndex, int operatorType1, Object criteria1)](#custom-int-int-java.lang.Object-) | Filters a list with a custom criterion. |
| [custom(int fieldIndex, int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2)](#custom-int-int-java.lang.Object-boolean-int-java.lang.Object-) | Filters a list with custom criteria. |
| [dynamicFilter(int fieldIndex, int dynamicFilterType)](#dynamicFilter-int-int-) | Adds a dynamic filter. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter(int fieldIndex, String criteria)](#filter-int-java.lang.String-) | Filters a list with specified criteria. |
| [filterTop10(int fieldIndex, boolean isTop, boolean isPercent, int itemCount)](#filterTop10-int-boolean-boolean-int-) | Filter the top 10 items in the list |
| [getCellArea()](#getCellArea--) | Gets the [CellArea](../../com.aspose.cells/cellarea) where the this AutoFilter applies to. |
| [getCellArea(boolean refreshAppliedRange)](#getCellArea-boolean-) | Gets the [CellArea](../../com.aspose.cells/cellarea) where the specified AutoFilter applies. |
| [getClass()](#getClass--) |  |
| [getFilterColumns()](#getFilterColumns--) | Gets the collection of the filter columns. |
| [getRange()](#getRange--) | Represents the range to which the specified AutoFilter applies. |
| [getShowFilterButton()](#getShowFilterButton--) | Indicates whether the AutoFilter button for this column is visible. |
| [getSorter()](#getSorter--) | Gets the data sorter. |
| [hashCode()](#hashCode--) |  |
| [matchBlanks(int fieldIndex)](#matchBlanks-int-) | Match all blank cells in the list. |
| [matchNonBlanks(int fieldIndex)](#matchNonBlanks-int-) | Match all not-blank cells in the list. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | Refresh auto filters to hide or unhide the rows. |
| [refresh(boolean hideRows)](#refresh-boolean-) | Gets all hidden rows' indexes. |
| [removeDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)](#removeDateFilter-int-int-int-int-int-int-int-int-) | Removes a date filter. |
| [removeFilter(int fieldIndex)](#removeFilter-int-) | Remove the specific filter. |
| [removeFilter(int fieldIndex, String criteria)](#removeFilter-int-java.lang.String-) | Removes a filter for a filter column. |
| [setRange(int row, int startColumn, int endColumn)](#setRange-int-int-int-) | Sets the range to which the specified AutoFilter applies. |
| [setRange(String value)](#setRange-java.lang.String-) | Represents the range to which the specified AutoFilter applies. |
| [setShowFilterButton(boolean value)](#setShowFilterButton-boolean-) | Indicates whether the AutoFilter button for this column is visible. |
| [showAll()](#showAll--) | Unhide all rows. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second) {#addDateFilter-int-int-int-int-int-int-int-int-}
```
public void addDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)
```


Adds a date filter.

**Remarks**

If DateTimeGroupingType is Year, only the param year effects. If DateTiemGroupingType is Month, only the param year and month effect.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| dateTimeGroupingType | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). The grouping type |
| year | int | The year. |
| month | int | The month. |
| day | int | The day. |
| hour | int | The hour. |
| minute | int | The minute. |
| second | int | The second. |

### addFillColorFilter(int fieldIndex, int pattern, CellsColor foregroundColor, CellsColor backgroundColor) {#addFillColorFilter-int-int-com.aspose.cells.CellsColor-com.aspose.cells.CellsColor-}
```
public void addFillColorFilter(int fieldIndex, int pattern, CellsColor foregroundColor, CellsColor backgroundColor)
```


Adds a fill color filter.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| pattern | int | [BackgroundType](../../com.aspose.cells/backgroundtype). The background pattern type. |
| foregroundColor | [CellsColor](../../com.aspose.cells/cellscolor) | The foreground color. |
| backgroundColor | [CellsColor](../../com.aspose.cells/cellscolor) | The background color. |

### addFilter(int fieldIndex, String criteria) {#addFilter-int-java.lang.String-}
```
public void addFilter(int fieldIndex, String criteria)
```


Adds a filter for a filter column.

**Remarks**

MS Excel 2007 supports multiple selection in a filter column.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| criteria | java.lang.String | The specified criteria (a string; for example, "101"). It only can be null or be one of the cells' value in this column. |

### addFontColorFilter(int fieldIndex, CellsColor color) {#addFontColorFilter-int-com.aspose.cells.CellsColor-}
```
public void addFontColorFilter(int fieldIndex, CellsColor color)
```


Adds a font color filter.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| color | [CellsColor](../../com.aspose.cells/cellscolor) | The [CellsColor](../../com.aspose.cells/cellscolor) object. |

### addIconFilter(int fieldIndex, int iconSetType, int iconId) {#addIconFilter-int-int-int-}
```
public void addIconFilter(int fieldIndex, int iconSetType, int iconId)
```


Adds an icon filter.

**Remarks**

Only supports to add the icon filter. Not supports checking which row is visible if the filter is icon filter.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| iconSetType | int | [IconSetType](../../com.aspose.cells/iconsettype). The icon set type. |
| iconId | int | The icon id. |

### custom(int fieldIndex, int operatorType1, Object criteria1) {#custom-int-int-java.lang.Object-}
```
public void custom(int fieldIndex, int operatorType1, Object criteria1)
```


Filters a list with a custom criterion.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| operatorType1 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). The filter operator type |
| criteria1 | java.lang.Object | The custom criteria |

### custom(int fieldIndex, int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2) {#custom-int-int-java.lang.Object-boolean-int-java.lang.Object-}
```
public void custom(int fieldIndex, int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2)
```


Filters a list with custom criteria.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| operatorType1 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). The filter operator type |
| criteria1 | java.lang.Object | The custom criteria |
| isAnd | boolean |  |
| operatorType2 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). The filter operator type |
| criteria2 | java.lang.Object | The custom criteria |

### dynamicFilter(int fieldIndex, int dynamicFilterType) {#dynamicFilter-int-int-}
```
public void dynamicFilter(int fieldIndex, int dynamicFilterType)
```


Adds a dynamic filter.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| dynamicFilterType | int | [DynamicFilterType](../../com.aspose.cells/dynamicfiltertype). Dynamic filter type. |

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
### filter(int fieldIndex, String criteria) {#filter-int-java.lang.String-}
```
public void filter(int fieldIndex, String criteria)
```


Filters a list with specified criteria.

**Remarks**

Aspose.Cells will remove all other filter setting on this field as Ms Excel 97-2003.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| criteria | java.lang.String | The specified criteria (a string; for example, "101"). |

### filterTop10(int fieldIndex, boolean isTop, boolean isPercent, int itemCount) {#filterTop10-int-boolean-boolean-int-}
```
public void filterTop10(int fieldIndex, boolean isTop, boolean isPercent, int itemCount)
```


Filter the top 10 items in the list

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| isTop | boolean | Indicates whether filter from top or bottom |
| isPercent | boolean | Indicates whether the items is percent or count |
| itemCount | int | The item count |

### getCellArea() {#getCellArea--}
```
public CellArea getCellArea()
```


Gets the [CellArea](../../com.aspose.cells/cellarea) where the this AutoFilter applies to.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the area this filter applies to
### getCellArea(boolean refreshAppliedRange) {#getCellArea-boolean-}
```
public CellArea getCellArea(boolean refreshAppliedRange)
```


Gets the [CellArea](../../com.aspose.cells/cellarea) where the specified AutoFilter applies.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| refreshAppliedRange | boolean | Whether refresh the applied range. For the applied range of auto filter, the last row may change when cells data changes. If this flag is true, then the last row of the range will be re-calculated according to current cells data. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the area this filter applies to
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFilterColumns() {#getFilterColumns--}
```
public FilterColumnCollection getFilterColumns()
```


Gets the collection of the filter columns.

**Returns:**
[FilterColumnCollection](../../com.aspose.cells/filtercolumncollection)
### getRange() {#getRange--}
```
public String getRange()
```


Represents the range to which the specified AutoFilter applies.

**Returns:**
java.lang.String
### getShowFilterButton() {#getShowFilterButton--}
```
public boolean getShowFilterButton()
```


Indicates whether the AutoFilter button for this column is visible.

**Returns:**
boolean
### getSorter() {#getSorter--}
```
public DataSorter getSorter()
```


Gets the data sorter.

**Returns:**
[DataSorter](../../com.aspose.cells/datasorter)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### matchBlanks(int fieldIndex) {#matchBlanks-int-}
```
public void matchBlanks(int fieldIndex)
```


Match all blank cells in the list.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |

### matchNonBlanks(int fieldIndex) {#matchNonBlanks-int-}
```
public void matchNonBlanks(int fieldIndex)
```


Match all not-blank cells in the list.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refresh() {#refresh--}
```
public int[] refresh()
```


Refresh auto filters to hide or unhide the rows.

**Returns:**
int[] - Returns all hidden rows' indexes.
### refresh(boolean hideRows) {#refresh-boolean-}
```
public int[] refresh(boolean hideRows)
```


Gets all hidden rows' indexes.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| hideRows | boolean | If true, hide the filtered rows. |

**Returns:**
int[] - Returns all hidden rows indexes.
### removeDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second) {#removeDateFilter-int-int-int-int-int-int-int-int-}
```
public void removeDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)
```


Removes a date filter.

**Remarks**

If DateTimeGroupingType is Year, only the param year effects. If DateTiemGroupingType is Month, only the param year and month effect.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| dateTimeGroupingType | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). The grouping type |
| year | int | The year. |
| month | int | The month. |
| day | int | The day. |
| hour | int | The hour. |
| minute | int | The minute. |
| second | int | The second. |

### removeFilter(int fieldIndex) {#removeFilter-int-}
```
public void removeFilter(int fieldIndex)
```


Remove the specific filter.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | The specific filter index |

### removeFilter(int fieldIndex, String criteria) {#removeFilter-int-java.lang.String-}
```
public void removeFilter(int fieldIndex, String criteria)
```


Removes a filter for a filter column.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| criteria | java.lang.String | The specified criteria (a string; for example, "101"). It only can be null or be one of the cells' value in this column. |

### setRange(int row, int startColumn, int endColumn) {#setRange-int-int-int-}
```
public void setRange(int row, int startColumn, int endColumn)
```


Sets the range to which the specified AutoFilter applies.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index. |
| startColumn | int | Start column index. |
| endColumn | int | End column Index. |

### setRange(String value) {#setRange-java.lang.String-}
```
public void setRange(String value)
```


Represents the range to which the specified AutoFilter applies.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setShowFilterButton(boolean value) {#setShowFilterButton-boolean-}
```
public void setShowFilterButton(boolean value)
```


Indicates whether the AutoFilter button for this column is visible.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### showAll() {#showAll--}
```
public void showAll()
```


Unhide all rows.

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

