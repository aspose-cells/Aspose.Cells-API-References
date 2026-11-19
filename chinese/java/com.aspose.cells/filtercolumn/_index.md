---
title: "FilterColumn"
second_title: "Aspose.Cells for Java API 参考"
description: "表示单列或表中列的过滤器。"
type: docs
url: /zh/java/com.aspose.cells/filtercolumn/
---

**Inheritance:**
java.lang.Object
```
public class FilterColumn
```

表示单列或表中列的过滤器。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColorFilter()](#getColorFilter--) | 获取用于按颜色过滤数据的 [ColorFilter](../../com.aspose.cells/colorfilter)。 |
| [getCustomFilters()](#getCustomFilters--) | 获取用于按自定义条件过滤数据的 [CustomFilterCollection](../../com.aspose.cells/customfiltercollection)。 |
| [getDynamicFilter()](#getDynamicFilter--) | 获取用于使用动态条件过滤的 [getDynamicFilter()](../../com.aspose.cells/filtercolumn\#getDynamicFilter--)。 |
| [getFieldIndex()](#getFieldIndex--) | 获取范围内的列偏移量。 |
| [getFilter()](#getFilter--) | 获取过滤数据的条件。 |
| [getFilterType()](#getFilterType--) | 获取过滤数据的类型。 |
| [getFilterValues()](#getFilterValues--) | 获取用于按标签或日期时间过滤数据的 [FilterValueCollection](../../com.aspose.cells/filtervaluecollection)。 |
| [getIconFilter()](#getIconFilter--) | 获取用于按图标过滤数据的 [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--)。 |
| [getMultipleFilters()](#getMultipleFilters--) | 获取用于按标签或日期时间过滤数据的 [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection)。 |
| [getTop10Filter()](#getTop10Filter--) | 获取用于按数据排名过滤的 [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--)。 |
| [hashCode()](#hashCode--) |  |
| [isDropdownVisible()](#isDropdownVisible--) | 指示此列的自动筛选按钮是否可见。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [selectAll()](#selectAll--) | 选择全部。 |
| [setCustomFilters(CustomFilterCollection value)](#setCustomFilters-com.aspose.cells.CustomFilterCollection-) | 获取用于按自定义条件过滤数据的 [CustomFilterCollection](../../com.aspose.cells/customfiltercollection)。 |
| [setDropdownVisible(boolean value)](#setDropdownVisible-boolean-) | 指示此列的自动筛选按钮是否可见。 |
| [setFieldIndex(int value)](#setFieldIndex-int-) | 设置范围内的列偏移量。 |
| [setFilter(Object value)](#setFilter-java.lang.Object-) | 设置过滤数据的条件。 |
| [setFilterType(int value)](#setFilterType-int-) | 设置过滤数据的类型。 |
| [setMultipleFilters(MultipleFilterCollection value)](#setMultipleFilters-com.aspose.cells.MultipleFilterCollection-) | 获取用于按标签或日期时间过滤数据的 [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection)。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
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


获取用于按颜色过滤数据的 [ColorFilter](../../com.aspose.cells/colorfilter)。

**Remarks**

首先将 [getFilterType()](../../com.aspose.cells/filtercolumn\\#getFilterType--) 设置为 [FilterType.COLOR\\_FILTER](../../com.aspose.cells/filtertype\\#COLOR-FILTER)，否则将返回 Null。

**Returns:**
[ColorFilter](../../com.aspose.cells/colorfilter)
### getCustomFilters() {#getCustomFilters--}
```
public CustomFilterCollection getCustomFilters()
```


获取用于按自定义条件过滤数据的 [CustomFilterCollection](../../com.aspose.cells/customfiltercollection)。

**Remarks**

注意：此属性的 setter 已过时。请改为使用属性 [getFilterType()](../../com.aspose.cells/filtercolumn\\#getFilterType--) 并将其设置为 [FilterType.CUSTOM\\_FILTERS](../../com.aspose.cells/filtertype\\#CUSTOM-FILTERS)。此属性将在自 2026 年 6 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
[CustomFilterCollection](../../com.aspose.cells/customfiltercollection)
### getDynamicFilter() {#getDynamicFilter--}
```
public DynamicFilter getDynamicFilter()
```


获取用于使用动态条件过滤的 [getDynamicFilter()](../../com.aspose.cells/filtercolumn\#getDynamicFilter--)。

**Remarks**

在使用此属性之前，请确保 [getFilterType()](../../com.aspose.cells/filtercolumn\\#getFilterType--) 为 [FilterType.DYNAMIC\\_FILTER](../../com.aspose.cells/filtertype\\#DYNAMIC-FILTER)，否则将返回 null。

**Returns:**
[DynamicFilter](../../com.aspose.cells/dynamicfilter)
### getFieldIndex() {#getFieldIndex--}
```
public int getFieldIndex()
```


获取范围内的列偏移量。

**Returns:**
int
### getFilter() {#getFilter--}
```
public Object getFilter()
```


获取过滤数据的条件。

**Remarks**

注意：此成员已过时。请改为根据 [getFilterType()](../../com.aspose.cells/filtercolumn\\#getFilterType--) 使用相应的属性。对于过滤类型 [FilterType.MULTIPLE\\_FILTERS](../../com.aspose.cells/filtertype\\#MULTIPLE-FILTERS)，返回的对象现在是 [FilterValueCollection](../../com.aspose.cells/filtervaluecollection)，而不是 [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection)。此属性将在自 2025 年 10 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
java.lang.Object
### getFilterType() {#getFilterType--}
```
public int getFilterType()
```


获取过滤数据的类型。

参见 [FilterType](../../com.aspose.cells/filtertype)。

**Remarks**

当设置此属性时，将创建相应的过滤对象，随后应使用对应的属性来获取该过滤对象：

| FilterType | 属性 |
| --------------- | ---------------------------------------------------------------------------- |
| MultipleFilters | [getFilterValues()](../../com.aspose.cells/filtercolumn\\#getFilterValues--) |
| CustomFilters | [getCustomFilters()](../../com.aspose.cells/filtercolumn\\#getCustomFilters--) |
| ColorFilter | [getColorFilter()](../../com.aspose.cells/filtercolumn\\#getColorFilter--) |
| DynamicFilter | [getDynamicFilter()](../../com.aspose.cells/filtercolumn\\#getDynamicFilter--) |
| IconFilter | [getIconFilter()](../../com.aspose.cells/filtercolumn\\#getIconFilter--) |
| Top10 | [getTop10Filter()](../../com.aspose.cells/filtercolumn\\#getTop10Filter--) |

**Returns:**
int
### getFilterValues() {#getFilterValues--}
```
public FilterValueCollection getFilterValues()
```


获取用于按标签或日期时间过滤数据的 [FilterValueCollection](../../com.aspose.cells/filtervaluecollection)。

**Remarks**

首先将 [getFilterType()](../../com.aspose.cells/filtercolumn\\#getFilterType--) 设置为 [FilterType.MULTIPLE\\_FILTERS](../../com.aspose.cells/filtertype\\#MULTIPLE-FILTERS)，否则将返回 Null。

**Returns:**
[FilterValueCollection](../../com.aspose.cells/filtervaluecollection)
### getIconFilter() {#getIconFilter--}
```
public IconFilter getIconFilter()
```


获取用于按图标过滤数据的 [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--)。

**Remarks**

在使用此属性之前，请确保 [getFilterType()](../../com.aspose.cells/filtercolumn\\#getFilterType--) 为 [FilterType.ICON\\_FILTER](../../com.aspose.cells/filtertype\\#ICON-FILTER)，否则将返回 null。

**Returns:**
[IconFilter](../../com.aspose.cells/iconfilter)
### getMultipleFilters() {#getMultipleFilters--}
```
public MultipleFilterCollection getMultipleFilters()
```


获取用于按标签或日期时间过滤数据的 [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection)。

**Remarks**

注意：此成员已过时。请改为使用 FilterColumn.FilterValues 属性。此属性将在自 2026 年 6 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
[MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection)
### getTop10Filter() {#getTop10Filter--}
```
public Top10Filter getTop10Filter()
```


获取用于按数据排名过滤的 [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--)。

**Remarks**

在使用此属性之前，请确保 [getFilterType()](../../com.aspose.cells/filtercolumn\\#getFilterType--) 为 [FilterType.TOP\\_10](../../com.aspose.cells/filtertype\\#TOP-10)，否则将返回 null。

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


指示此列的自动筛选按钮是否可见。

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


选择全部。

### setCustomFilters(CustomFilterCollection value) {#setCustomFilters-com.aspose.cells.CustomFilterCollection-}
```
public void setCustomFilters(CustomFilterCollection value)
```


获取用于按自定义条件过滤数据的 [CustomFilterCollection](../../com.aspose.cells/customfiltercollection)。

**Remarks**

注意：此属性的 setter 已过时。请改为使用属性 [getFilterType()](../../com.aspose.cells/filtercolumn\\#getFilterType--) 并将其设置为 [FilterType.CUSTOM\\_FILTERS](../../com.aspose.cells/filtertype\\#CUSTOM-FILTERS)。此属性将在自 2026 年 6 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) |  |

### setDropdownVisible(boolean value) {#setDropdownVisible-boolean-}
```
public void setDropdownVisible(boolean value)
```


指示此列的自动筛选按钮是否可见。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFieldIndex(int value) {#setFieldIndex-int-}
```
public void setFieldIndex(int value)
```


设置范围内的列偏移量。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setFilter(Object value) {#setFilter-java.lang.Object-}
```
public void setFilter(Object value)
```


设置过滤数据的条件。

**Remarks**

注意：此成员已过时。请改为根据 [getFilterType()](../../com.aspose.cells/filtercolumn\\#getFilterType--) 使用相应的属性。对于过滤类型 [FilterType.MULTIPLE\\_FILTERS](../../com.aspose.cells/filtertype\\#MULTIPLE-FILTERS)，返回的对象现在是 [FilterValueCollection](../../com.aspose.cells/filtervaluecollection)，而不是 [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection)。此属性将在自 2025 年 10 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Object |  |

### setFilterType(int value) {#setFilterType-int-}
```
public void setFilterType(int value)
```


设置过滤数据的类型。

参见 [FilterType](../../com.aspose.cells/filtertype)。

**Remarks**

当设置此属性时，将创建相应的过滤对象，随后应使用对应的属性来获取该过滤对象：

| FilterType | 属性 |
| --------------- | ---------------------------------------------------------------------------- |
| MultipleFilters | [getFilterValues()](../../com.aspose.cells/filtercolumn\\#getFilterValues--) |
| CustomFilters | [getCustomFilters()](../../com.aspose.cells/filtercolumn\\#getCustomFilters--) |
| ColorFilter | [getColorFilter()](../../com.aspose.cells/filtercolumn\\#getColorFilter--) |
| DynamicFilter | [getDynamicFilter()](../../com.aspose.cells/filtercolumn\\#getDynamicFilter--) |
| IconFilter | [getIconFilter()](../../com.aspose.cells/filtercolumn\\#getIconFilter--) |
| Top10 | [getTop10Filter()](../../com.aspose.cells/filtercolumn\\#getTop10Filter--) |

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMultipleFilters(MultipleFilterCollection value) {#setMultipleFilters-com.aspose.cells.MultipleFilterCollection-}
```
public void setMultipleFilters(MultipleFilterCollection value)
```


获取用于按标签或日期时间过滤数据的 [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection)。

**Remarks**

注意：此成员已过时。请改为使用 FilterColumn.FilterValues 属性。此属性将在自 2026 年 6 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

