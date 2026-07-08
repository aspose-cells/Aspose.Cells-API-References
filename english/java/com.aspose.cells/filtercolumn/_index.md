---
title: FilterColumn
second_title: Aspose.Cells for Java API Reference
description: Represents a filter for a single column or a column in the table.
type: docs
url: /java/com.aspose.cells/filtercolumn/
---

**Inheritance:**
java.lang.Object
```
public class FilterColumn
```

Represents a filter for a single column or a column in the table.
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColorFilter()](#getColorFilter--) | Gets [ColorFilter](../../com.aspose.cells/colorfilter) for filtering data by color. |
| [getCustomFilters()](#getCustomFilters--) | Gets [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) for filtering data by custom criteria. |
| [getDynamicFilter()](#getDynamicFilter--) | Gets [getDynamicFilter()](../../com.aspose.cells/filtercolumn\#getDynamicFilter--) for filtering with dynamic criteria. |
| [getFieldIndex()](#getFieldIndex--) | Gets the column offset in the range. |
| [getFilter()](#getFilter--) | Gets the condition of filtering data. |
| [getFilterType()](#getFilterType--) | Gets the type fo filtering data. |
| [getFilterValues()](#getFilterValues--) | Gets [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) for filtering data by labels or date time. |
| [getIconFilter()](#getIconFilter--) | Gets [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--) for filtering data by icon. |
| [getMultipleFilters()](#getMultipleFilters--) | Gets [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) for filtering data by labels or date time. |
| [getTop10Filter()](#getTop10Filter--) | Gets [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--) for filtering data by rank of data. |
| [hashCode()](#hashCode--) |  |
| [isDropdownVisible()](#isDropdownVisible--) | Indicates whether the AutoFilter button for this column is visible. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [selectAll()](#selectAll--) | Selects all. |
| [setCustomFilters(CustomFilterCollection value)](#setCustomFilters-com.aspose.cells.CustomFilterCollection-) | Gets [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) for filtering data by custom criteria. |
| [setDropdownVisible(boolean value)](#setDropdownVisible-boolean-) | Indicates whether the AutoFilter button for this column is visible. |
| [setFieldIndex(int value)](#setFieldIndex-int-) | Sets the column offset in the range. |
| [setFilter(Object value)](#setFilter-java.lang.Object-) | Sets the condition of filtering data. |
| [setFilterType(int value)](#setFilterType-int-) | Sets the type fo filtering data. |
| [setMultipleFilters(MultipleFilterCollection value)](#setMultipleFilters-com.aspose.cells.MultipleFilterCollection-) | Gets [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) for filtering data by labels or date time. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColorFilter() {#getColorFilter--}
```
public ColorFilter getColorFilter()
```


Gets [ColorFilter](../../com.aspose.cells/colorfilter) for filtering data by color.

**Remarks**

Sets [FilterType](../../com.aspose.cells/filtertype) as [FilterType.COLOR\_FILTER](../../com.aspose.cells/filtertype\#COLOR-FILTER) first,otherwise Null will be returned.

**Returns:**
[ColorFilter](../../com.aspose.cells/colorfilter)
### getCustomFilters() {#getCustomFilters--}
```
public CustomFilterCollection getCustomFilters()
```


Gets [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) for filtering data by custom criteria.

**Remarks**

NOTE: This setter of this propery is now obsolete. Instead,please use property [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) by setting it as [FilterType.CUSTOM\_FILTERS](../../com.aspose.cells/filtertype\#CUSTOM-FILTERS). This property will be removed 12 months later since June 2026. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
[CustomFilterCollection](../../com.aspose.cells/customfiltercollection)
### getDynamicFilter() {#getDynamicFilter--}
```
public DynamicFilter getDynamicFilter()
```


Gets [getDynamicFilter()](../../com.aspose.cells/filtercolumn\#getDynamicFilter--) for filtering with dynamic criteria.

**Remarks**

Before using this property, please make sure [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) is [FilterType.DYNAMIC\_FILTER](../../com.aspose.cells/filtertype\#DYNAMIC-FILTER), otherwise null will be returned.

**Returns:**
[DynamicFilter](../../com.aspose.cells/dynamicfilter)
### getFieldIndex() {#getFieldIndex--}
```
public int getFieldIndex()
```


Gets the column offset in the range.

**Returns:**
int
### getFilter() {#getFilter--}
```
public Object getFilter()
```


Gets the condition of filtering data.

**Remarks**

NOTE: This member is now obsolete. Instead,please use FilterColumn.MultipleFilters,CustomFilters and so on... property according to differnt type of filter /// This property will be removed 12 months later since October 2025. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
java.lang.Object
### getFilterType() {#getFilterType--}
```
public int getFilterType()
```


Gets the type fo filtering data.

See [FilterType](../../com.aspose.cells/filtertype).

**Remarks**

The corresponding filter object will be created when this property is set.

**Returns:**
int
### getFilterValues() {#getFilterValues--}
```
public FilterValueCollection getFilterValues()
```


Gets [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) for filtering data by labels or date time.

**Remarks**

Sets [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) as [FilterType.MULTIPLE\_FILTERS](../../com.aspose.cells/filtertype\#MULTIPLE-FILTERS) first,otherwise Null will be returned.

**Returns:**
[FilterValueCollection](../../com.aspose.cells/filtervaluecollection)
### getIconFilter() {#getIconFilter--}
```
public IconFilter getIconFilter()
```


Gets [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--) for filtering data by icon.

**Remarks**

Before using this property, please make sure [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) is [FilterType.ICON\_FILTER](../../com.aspose.cells/filtertype\#ICON-FILTER), otherwise null will be returned.

**Returns:**
[IconFilter](../../com.aspose.cells/iconfilter)
### getMultipleFilters() {#getMultipleFilters--}
```
public MultipleFilterCollection getMultipleFilters()
```


Gets [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) for filtering data by labels or date time.

**Remarks**

NOTE: This member is now obsolete. Instead,please use FilterColumn.FilterValues property . This property will be removed 12 months later since June 2026. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
[MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection)
### getTop10Filter() {#getTop10Filter--}
```
public Top10Filter getTop10Filter()
```


Gets [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--) for filtering data by rank of data.

**Remarks**

Before using this property, please make sure [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) is [FilterType.TOP\_10](../../com.aspose.cells/filtertype\#TOP-10), otherwise null will be returned.

**Returns:**
[Top10Filter](../../com.aspose.cells/top10filter)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isDropdownVisible() {#isDropdownVisible--}
```
public boolean isDropdownVisible()
```


Indicates whether the AutoFilter button for this column is visible.

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




### selectAll() {#selectAll--}
```
public void selectAll()
```


Selects all.

### setCustomFilters(CustomFilterCollection value) {#setCustomFilters-com.aspose.cells.CustomFilterCollection-}
```
public void setCustomFilters(CustomFilterCollection value)
```


Gets [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) for filtering data by custom criteria.

**Remarks**

NOTE: This setter of this propery is now obsolete. Instead,please use property [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) by setting it as [FilterType.CUSTOM\_FILTERS](../../com.aspose.cells/filtertype\#CUSTOM-FILTERS). This property will be removed 12 months later since June 2026. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) |  |

### setDropdownVisible(boolean value) {#setDropdownVisible-boolean-}
```
public void setDropdownVisible(boolean value)
```


Indicates whether the AutoFilter button for this column is visible.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFieldIndex(int value) {#setFieldIndex-int-}
```
public void setFieldIndex(int value)
```


Sets the column offset in the range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setFilter(Object value) {#setFilter-java.lang.Object-}
```
public void setFilter(Object value)
```


Sets the condition of filtering data.

**Remarks**

NOTE: This member is now obsolete. Instead,please use FilterColumn.MultipleFilters,CustomFilters and so on... property according to differnt type of filter /// This property will be removed 12 months later since October 2025. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Object |  |

### setFilterType(int value) {#setFilterType-int-}
```
public void setFilterType(int value)
```


Sets the type fo filtering data.

See [FilterType](../../com.aspose.cells/filtertype).

**Remarks**

The corresponding filter object will be created when this property is set.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setMultipleFilters(MultipleFilterCollection value) {#setMultipleFilters-com.aspose.cells.MultipleFilterCollection-}
```
public void setMultipleFilters(MultipleFilterCollection value)
```


Gets [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) for filtering data by labels or date time.

**Remarks**

NOTE: This member is now obsolete. Instead,please use FilterColumn.FilterValues property . This property will be removed 12 months later since June 2026. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) |  |

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

