---
title: FilterColumn
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a filter for a single column or a column in the table.
type: docs
url: /nodejs-cpp/filtercolumn/
---

## FilterColumn class

Represents a filter for a single column or a column in the table.

```javascript
class FilterColumn;
```


## Properties

| Property | Type | Description |
| --- | --- | --- |
| [isDropdownVisible](#isDropdownVisible--)| boolean | Indicates whether the AutoFilter button for this column is visible. |
| [filter](#filter--)| Object | Gets and sets the condition of filtering data. |
| [filterType](#filterType--)| FilterType | Gets and sets the type fo filtering data. |
| [filterValues](#filterValues--)| FilterValueCollection | Readonly. Gets [Aspose.Cells.FilterValueCollection](../aspose.cells.filtervaluecollection/) for filtering data by labels or date time. |
| [multipleFilters](#multipleFilters--)| MultipleFilterCollection | Gets [MultipleFilterCollection](../multiplefiltercollection/) for filtering data by labels or date time. |
| [customFilters](#customFilters--)| CustomFilterCollection | Gets [CustomFilterCollection](../customfiltercollection/) for filtering data by custom criteria. |
| [colorFilter](#colorFilter--)| ColorFilter | Readonly. Gets [Aspose.Cells.ColorFilter](../aspose.cells.colorfilter/) for filtering data by color. |
| [dynamicFilter](#dynamicFilter--)| DynamicFilter | Readonly. Gets [DynamicFilter](../dynamicfilter/) for filtering with dynamic criteria. |
| [iconFilter](#iconFilter--)| IconFilter | Readonly. Gets [IconFilter](../iconfilter/) for filtering data by icon. |
| [top10Filter](#top10Filter--)| Top10Filter | Readonly. Gets [Top10Filter](../top10filter/) for filtering data by rank of data. |
| [fieldIndex](#fieldIndex--)| number | Gets and sets the column offset in the range. |

## Methods

| Method | Description |
| --- | --- |
| [isDropdownVisible()](#isDropdownVisible--)| <b>@deprecated.</b> Please use the 'isDropdownVisible' property instead. Indicates whether the AutoFilter button for this column is visible. |
| [setIsDropdownVisible(boolean)](#setIsDropdownVisible-boolean-)| <b>@deprecated.</b> Please use the 'isDropdownVisible' property instead. Indicates whether the AutoFilter button for this column is visible. |
| [getFilter()](#getFilter--)| <b>@deprecated.</b> Please use the 'filter' property instead. Gets and sets the condition of filtering data. |
| [setFilter(Object)](#setFilter-object-)| <b>@deprecated.</b> Please use the 'filter' property instead. Gets and sets the condition of filtering data. |
| [getFilterType()](#getFilterType--)| <b>@deprecated.</b> Please use the 'filterType' property instead. Gets and sets the type fo filtering data. |
| [setFilterType(FilterType)](#setFilterType-filtertype-)| <b>@deprecated.</b> Please use the 'filterType' property instead. Gets and sets the type fo filtering data. |
| [getFilterValues()](#getFilterValues--)| <b>@deprecated.</b> Please use the 'filterValues' property instead. Gets [Aspose.Cells.FilterValueCollection](../aspose.cells.filtervaluecollection/) for filtering data by labels or date time. |
| [getMultipleFilters()](#getMultipleFilters--)| <b>@deprecated.</b> Please use the 'multipleFilters' property instead. Gets [MultipleFilterCollection](../multiplefiltercollection/) for filtering data by labels or date time. |
| [setMultipleFilters(MultipleFilterCollection)](#setMultipleFilters-multiplefiltercollection-)| <b>@deprecated.</b> Please use the 'multipleFilters' property instead. Gets [MultipleFilterCollection](../multiplefiltercollection/) for filtering data by labels or date time. |
| [getCustomFilters()](#getCustomFilters--)| <b>@deprecated.</b> Please use the 'customFilters' property instead. Gets [CustomFilterCollection](../customfiltercollection/) for filtering data by custom criteria. |
| [setCustomFilters(CustomFilterCollection)](#setCustomFilters-customfiltercollection-)| <b>@deprecated.</b> Please use the 'customFilters' property instead. Gets [CustomFilterCollection](../customfiltercollection/) for filtering data by custom criteria. |
| [getColorFilter()](#getColorFilter--)| <b>@deprecated.</b> Please use the 'colorFilter' property instead. Gets [Aspose.Cells.ColorFilter](../aspose.cells.colorfilter/) for filtering data by color. |
| [getDynamicFilter()](#getDynamicFilter--)| <b>@deprecated.</b> Please use the 'dynamicFilter' property instead. Gets [DynamicFilter](../dynamicfilter/) for filtering with dynamic criteria. |
| [getIconFilter()](#getIconFilter--)| <b>@deprecated.</b> Please use the 'iconFilter' property instead. Gets [IconFilter](../iconfilter/) for filtering data by icon. |
| [getTop10Filter()](#getTop10Filter--)| <b>@deprecated.</b> Please use the 'top10Filter' property instead. Gets [Top10Filter](../top10filter/) for filtering data by rank of data. |
| [getFieldIndex()](#getFieldIndex--)| <b>@deprecated.</b> Please use the 'fieldIndex' property instead. Gets and sets the column offset in the range. |
| [setFieldIndex(number)](#setFieldIndex-number-)| <b>@deprecated.</b> Please use the 'fieldIndex' property instead. Gets and sets the column offset in the range. |
| [selectAll()](#selectAll--)| Selects all. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### isDropdownVisible {#isDropdownVisible--}

Indicates whether the AutoFilter button for this column is visible.

```javascript
isDropdownVisible : boolean;
```


### filter {#filter--}

Gets and sets the condition of filtering data.

```javascript
filter : Object;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please use corresponding property according to [FilterColumn.FilterType](../filtercolumn.filtertype/). And for filter type [FilterType.MultipleFilters](../filtertype.multiplefilters/), the returned object is [FilterValueCollection](../filtervaluecollection/) now instead of [MultipleFilterCollection](../multiplefiltercollection/). This property will be removed 12 months later since October 2025. Aspose apologizes for any inconvenience you may have experienced.

### filterType {#filterType--}

Gets and sets the type fo filtering data.

```javascript
filterType : FilterType;
```


**Remarks**

The corresponding filter object will be created when this property is set and corresponding property should be used to get the filter object accordingly: <list type="table"> <listheader> <description>FilterType</description> <description>Property</description> </listheader> <item> <description>MultipleFilters</description> <description>[FilterColumn.FilterValues](../filtercolumn.filtervalues/)</description> </item> <item> <description>CustomFilters</description> <description>[FilterColumn.CustomFilters](../filtercolumn.customfilters/)</description> </item> <item> <description>ColorFilter</description> <description>[FilterColumn.ColorFilter](../filtercolumn.colorfilter/)</description> </item> <item> <description>DynamicFilter</description> <description>[FilterColumn.DynamicFilter](../filtercolumn.dynamicfilter/)</description> </item> <item> <description>IconFilter</description> <description>[FilterColumn.IconFilter](../filtercolumn.iconfilter/)</description> </item> <item> <description>Top10</description> <description>[FilterColumn.Top10Filter](../filtercolumn.top10filter/)</description> </item> </list

### filterValues {#filterValues--}

Readonly. Gets [Aspose.Cells.FilterValueCollection](../aspose.cells.filtervaluecollection/) for filtering data by labels or date time.

```javascript
filterValues : FilterValueCollection;
```


**Remarks**

Sets [FilterColumn.FilterType](../filtercolumn.filtertype/) as [FilterType.MultipleFilters](../filtertype.multiplefilters/) first,otherwise Null will be returned.

### multipleFilters {#multipleFilters--}

Gets [MultipleFilterCollection](../multiplefiltercollection/) for filtering data by labels or date time.

```javascript
multipleFilters : MultipleFilterCollection;
```


**Remarks**

NOTE: This member is now obsolete. Instead,please use FilterColumn.FilterValues property . This property will be removed 12 months later since June 2026. Aspose apologizes for any inconvenience you may have experienced.

### customFilters {#customFilters--}

Gets [CustomFilterCollection](../customfiltercollection/) for filtering data by custom criteria.

```javascript
customFilters : CustomFilterCollection;
```


**Remarks**

NOTE: This setter of this propery is now obsolete. Instead,please use property [FilterColumn.FilterType](../filtercolumn.filtertype/) by setting it as [FilterType.CustomFilters](../filtertype.customfilters/). This property will be removed 12 months later since June 2026. Aspose apologizes for any inconvenience you may have experienced.

### colorFilter {#colorFilter--}

Readonly. Gets [Aspose.Cells.ColorFilter](../aspose.cells.colorfilter/) for filtering data by color.

```javascript
colorFilter : ColorFilter;
```


**Remarks**

Sets [FilterType](../filtertype/) as [FilterType.ColorFilter](../filtertype.colorfilter/) first,otherwise Null will be returned.

### dynamicFilter {#dynamicFilter--}

Readonly. Gets [DynamicFilter](../dynamicfilter/) for filtering with dynamic criteria.

```javascript
dynamicFilter : DynamicFilter;
```


**Remarks**

Before using this property, please make sure [FilterColumn.FilterType](../filtercolumn.filtertype/) is [FilterType.DynamicFilter](../filtertype.dynamicfilter/), otherwise null will be returned.

### iconFilter {#iconFilter--}

Readonly. Gets [IconFilter](../iconfilter/) for filtering data by icon.

```javascript
iconFilter : IconFilter;
```


**Remarks**

Before using this property, please make sure [FilterColumn.FilterType](../filtercolumn.filtertype/) is [FilterType.IconFilter](../filtertype.iconfilter/), otherwise null will be returned.

### top10Filter {#top10Filter--}

Readonly. Gets [Top10Filter](../top10filter/) for filtering data by rank of data.

```javascript
top10Filter : Top10Filter;
```


**Remarks**

Before using this property, please make sure [FilterColumn.FilterType](../filtercolumn.filtertype/) is [FilterType.Top10](../filtertype.top10/), otherwise null will be returned.

### fieldIndex {#fieldIndex--}

Gets and sets the column offset in the range.

```javascript
fieldIndex : number;
```


### isDropdownVisible() {#isDropdownVisible--}

<b>@deprecated.</b> Please use the 'isDropdownVisible' property instead. Indicates whether the AutoFilter button for this column is visible.

```javascript
isDropdownVisible() : boolean;
```


### setIsDropdownVisible(boolean) {#setIsDropdownVisible-boolean-}

<b>@deprecated.</b> Please use the 'isDropdownVisible' property instead. Indicates whether the AutoFilter button for this column is visible.

```javascript
setIsDropdownVisible(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getFilter() {#getFilter--}

<b>@deprecated.</b> Please use the 'filter' property instead. Gets and sets the condition of filtering data.

```javascript
getFilter() : Object;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please use corresponding property according to [FilterColumn.FilterType](../filtercolumn.filtertype/). And for filter type [FilterType.MultipleFilters](../filtertype.multiplefilters/), the returned object is [FilterValueCollection](../filtervaluecollection/) now instead of [MultipleFilterCollection](../multiplefiltercollection/). This property will be removed 12 months later since October 2025. Aspose apologizes for any inconvenience you may have experienced.

### setFilter(Object) {#setFilter-object-}

<b>@deprecated.</b> Please use the 'filter' property instead. Gets and sets the condition of filtering data.

```javascript
setFilter(value: Object) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Object | The value to set. |

**Remarks**

NOTE: This member is now obsolete. Instead, please use corresponding property according to [FilterColumn.FilterType](../filtercolumn.filtertype/). And for filter type [FilterType.MultipleFilters](../filtertype.multiplefilters/), the returned object is [FilterValueCollection](../filtervaluecollection/) now instead of [MultipleFilterCollection](../multiplefiltercollection/). This property will be removed 12 months later since October 2025. Aspose apologizes for any inconvenience you may have experienced.

### getFilterType() {#getFilterType--}

<b>@deprecated.</b> Please use the 'filterType' property instead. Gets and sets the type fo filtering data.

```javascript
getFilterType() : FilterType;
```


**Returns**

[FilterType](../filtertype/)

**Remarks**

The corresponding filter object will be created when this property is set and corresponding property should be used to get the filter object accordingly: <list type="table"> <listheader> <description>FilterType</description> <description>Property</description> </listheader> <item> <description>MultipleFilters</description> <description>[FilterColumn.FilterValues](../filtercolumn.filtervalues/)</description> </item> <item> <description>CustomFilters</description> <description>[FilterColumn.CustomFilters](../filtercolumn.customfilters/)</description> </item> <item> <description>ColorFilter</description> <description>[FilterColumn.ColorFilter](../filtercolumn.colorfilter/)</description> </item> <item> <description>DynamicFilter</description> <description>[FilterColumn.DynamicFilter](../filtercolumn.dynamicfilter/)</description> </item> <item> <description>IconFilter</description> <description>[FilterColumn.IconFilter](../filtercolumn.iconfilter/)</description> </item> <item> <description>Top10</description> <description>[FilterColumn.Top10Filter](../filtercolumn.top10filter/)</description> </item> </list

### setFilterType(FilterType) {#setFilterType-filtertype-}

<b>@deprecated.</b> Please use the 'filterType' property instead. Gets and sets the type fo filtering data.

```javascript
setFilterType(value: FilterType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FilterType](../filtertype/) | The value to set. |

**Remarks**

The corresponding filter object will be created when this property is set and corresponding property should be used to get the filter object accordingly: <list type="table"> <listheader> <description>FilterType</description> <description>Property</description> </listheader> <item> <description>MultipleFilters</description> <description>[FilterColumn.FilterValues](../filtercolumn.filtervalues/)</description> </item> <item> <description>CustomFilters</description> <description>[FilterColumn.CustomFilters](../filtercolumn.customfilters/)</description> </item> <item> <description>ColorFilter</description> <description>[FilterColumn.ColorFilter](../filtercolumn.colorfilter/)</description> </item> <item> <description>DynamicFilter</description> <description>[FilterColumn.DynamicFilter](../filtercolumn.dynamicfilter/)</description> </item> <item> <description>IconFilter</description> <description>[FilterColumn.IconFilter](../filtercolumn.iconfilter/)</description> </item> <item> <description>Top10</description> <description>[FilterColumn.Top10Filter](../filtercolumn.top10filter/)</description> </item> </list

### getFilterValues() {#getFilterValues--}

<b>@deprecated.</b> Please use the 'filterValues' property instead. Gets [Aspose.Cells.FilterValueCollection](../aspose.cells.filtervaluecollection/) for filtering data by labels or date time.

```javascript
getFilterValues() : FilterValueCollection;
```


**Returns**

[FilterValueCollection](../filtervaluecollection/)

**Remarks**

Sets [FilterColumn.FilterType](../filtercolumn.filtertype/) as [FilterType.MultipleFilters](../filtertype.multiplefilters/) first,otherwise Null will be returned.

### getMultipleFilters() {#getMultipleFilters--}

<b>@deprecated.</b> Please use the 'multipleFilters' property instead. Gets [MultipleFilterCollection](../multiplefiltercollection/) for filtering data by labels or date time.

```javascript
getMultipleFilters() : MultipleFilterCollection;
```


**Returns**

[MultipleFilterCollection](../multiplefiltercollection/)

**Remarks**

NOTE: This member is now obsolete. Instead,please use FilterColumn.FilterValues property . This property will be removed 12 months later since June 2026. Aspose apologizes for any inconvenience you may have experienced.

### setMultipleFilters(MultipleFilterCollection) {#setMultipleFilters-multiplefiltercollection-}

<b>@deprecated.</b> Please use the 'multipleFilters' property instead. Gets [MultipleFilterCollection](../multiplefiltercollection/) for filtering data by labels or date time.

```javascript
setMultipleFilters(value: MultipleFilterCollection) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MultipleFilterCollection](../multiplefiltercollection/) | The value to set. |

**Remarks**

NOTE: This member is now obsolete. Instead,please use FilterColumn.FilterValues property . This property will be removed 12 months later since June 2026. Aspose apologizes for any inconvenience you may have experienced.

### getCustomFilters() {#getCustomFilters--}

<b>@deprecated.</b> Please use the 'customFilters' property instead. Gets [CustomFilterCollection](../customfiltercollection/) for filtering data by custom criteria.

```javascript
getCustomFilters() : CustomFilterCollection;
```


**Returns**

[CustomFilterCollection](../customfiltercollection/)

**Remarks**

NOTE: This setter of this propery is now obsolete. Instead,please use property [FilterColumn.FilterType](../filtercolumn.filtertype/) by setting it as [FilterType.CustomFilters](../filtertype.customfilters/). This property will be removed 12 months later since June 2026. Aspose apologizes for any inconvenience you may have experienced.

### setCustomFilters(CustomFilterCollection) {#setCustomFilters-customfiltercollection-}

<b>@deprecated.</b> Please use the 'customFilters' property instead. Gets [CustomFilterCollection](../customfiltercollection/) for filtering data by custom criteria.

```javascript
setCustomFilters(value: CustomFilterCollection) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CustomFilterCollection](../customfiltercollection/) | The value to set. |

**Remarks**

NOTE: This setter of this propery is now obsolete. Instead,please use property [FilterColumn.FilterType](../filtercolumn.filtertype/) by setting it as [FilterType.CustomFilters](../filtertype.customfilters/). This property will be removed 12 months later since June 2026. Aspose apologizes for any inconvenience you may have experienced.

### getColorFilter() {#getColorFilter--}

<b>@deprecated.</b> Please use the 'colorFilter' property instead. Gets [Aspose.Cells.ColorFilter](../aspose.cells.colorfilter/) for filtering data by color.

```javascript
getColorFilter() : ColorFilter;
```


**Returns**

[ColorFilter](../colorfilter/)

**Remarks**

Sets [FilterType](../filtertype/) as [FilterType.ColorFilter](../filtertype.colorfilter/) first,otherwise Null will be returned.

### getDynamicFilter() {#getDynamicFilter--}

<b>@deprecated.</b> Please use the 'dynamicFilter' property instead. Gets [DynamicFilter](../dynamicfilter/) for filtering with dynamic criteria.

```javascript
getDynamicFilter() : DynamicFilter;
```


**Returns**

[DynamicFilter](../dynamicfilter/)

**Remarks**

Before using this property, please make sure [FilterColumn.FilterType](../filtercolumn.filtertype/) is [FilterType.DynamicFilter](../filtertype.dynamicfilter/), otherwise null will be returned.

### getIconFilter() {#getIconFilter--}

<b>@deprecated.</b> Please use the 'iconFilter' property instead. Gets [IconFilter](../iconfilter/) for filtering data by icon.

```javascript
getIconFilter() : IconFilter;
```


**Returns**

[IconFilter](../iconfilter/)

**Remarks**

Before using this property, please make sure [FilterColumn.FilterType](../filtercolumn.filtertype/) is [FilterType.IconFilter](../filtertype.iconfilter/), otherwise null will be returned.

### getTop10Filter() {#getTop10Filter--}

<b>@deprecated.</b> Please use the 'top10Filter' property instead. Gets [Top10Filter](../top10filter/) for filtering data by rank of data.

```javascript
getTop10Filter() : Top10Filter;
```


**Returns**

[Top10Filter](../top10filter/)

**Remarks**

Before using this property, please make sure [FilterColumn.FilterType](../filtercolumn.filtertype/) is [FilterType.Top10](../filtertype.top10/), otherwise null will be returned.

### getFieldIndex() {#getFieldIndex--}

<b>@deprecated.</b> Please use the 'fieldIndex' property instead. Gets and sets the column offset in the range.

```javascript
getFieldIndex() : number;
```


### setFieldIndex(number) {#setFieldIndex-number-}

<b>@deprecated.</b> Please use the 'fieldIndex' property instead. Gets and sets the column offset in the range.

```javascript
setFieldIndex(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### selectAll() {#selectAll--}

Selects all.

```javascript
selectAll() : void;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



