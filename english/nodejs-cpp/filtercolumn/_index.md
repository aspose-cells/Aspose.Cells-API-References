---
title: FilterColumn
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a filter for a single column.
type: docs
url: /nodejs-cpp/filtercolumn/
---

## FilterColumn class

Represents a filter for a single column.

```javascript
class FilterColumn;
```


## Properties

| Property | Type | Description |
| --- | --- | --- |
| [isDropdownVisible](#isDropdownVisible--)| boolean | Indicates whether the AutoFilter button for this column is visible. |
| [filter](#filter--)| Object | Gets and sets the condition of filtering data. |
| [filterType](#filterType--)| FilterType | Gets and sets the type fo filtering data. |
| [multipleFilters](#multipleFilters--)| MultipleFilterCollection | Gets [Aspose.Cells.MultipleFilterCollection](../aspose.cells.multiplefiltercollection/) for filtering data by labels or date time. |
| [customFilters](#customFilters--)| CustomFilterCollection | Gets [Aspose.Cells.CustomFilterCollection](../aspose.cells.customfiltercollection/) for filtering data by custom criteria. |
| [colorFilter](#colorFilter--)| ColorFilter | Readonly. Gets [Aspose.Cells.ColorFilter](../aspose.cells.colorfilter/) for filtering data by color. |
| [dynamicFilter](#dynamicFilter--)| DynamicFilter | Readonly. Gets [Aspose.Cells.DynamicFilter](../aspose.cells.dynamicfilter/) for filtering with dynamic criteria. |
| [iconFilter](#iconFilter--)| IconFilter | Readonly. Gets [Aspose.Cells.IconFilter](../aspose.cells.iconfilter/) for filtering data by icon. |
| [top10Filter](#top10Filter--)| Top10Filter | Readonly. Gets [Aspose.Cells.Top10Filter](../aspose.cells.top10filter/) for filtering data by rank of data. |
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
| [getMultipleFilters()](#getMultipleFilters--)| <b>@deprecated.</b> Please use the 'multipleFilters' property instead. Gets [Aspose.Cells.MultipleFilterCollection](../aspose.cells.multiplefiltercollection/) for filtering data by labels or date time. |
| [setMultipleFilters(MultipleFilterCollection)](#setMultipleFilters-multiplefiltercollection-)| <b>@deprecated.</b> Please use the 'multipleFilters' property instead. Gets [Aspose.Cells.MultipleFilterCollection](../aspose.cells.multiplefiltercollection/) for filtering data by labels or date time. |
| [getCustomFilters()](#getCustomFilters--)| <b>@deprecated.</b> Please use the 'customFilters' property instead. Gets [Aspose.Cells.CustomFilterCollection](../aspose.cells.customfiltercollection/) for filtering data by custom criteria. |
| [setCustomFilters(CustomFilterCollection)](#setCustomFilters-customfiltercollection-)| <b>@deprecated.</b> Please use the 'customFilters' property instead. Gets [Aspose.Cells.CustomFilterCollection](../aspose.cells.customfiltercollection/) for filtering data by custom criteria. |
| [getColorFilter()](#getColorFilter--)| <b>@deprecated.</b> Please use the 'colorFilter' property instead. Gets [Aspose.Cells.ColorFilter](../aspose.cells.colorfilter/) for filtering data by color. |
| [getDynamicFilter()](#getDynamicFilter--)| <b>@deprecated.</b> Please use the 'dynamicFilter' property instead. Gets [Aspose.Cells.DynamicFilter](../aspose.cells.dynamicfilter/) for filtering with dynamic criteria. |
| [getIconFilter()](#getIconFilter--)| <b>@deprecated.</b> Please use the 'iconFilter' property instead. Gets [Aspose.Cells.IconFilter](../aspose.cells.iconfilter/) for filtering data by icon. |
| [getTop10Filter()](#getTop10Filter--)| <b>@deprecated.</b> Please use the 'top10Filter' property instead. Gets [Aspose.Cells.Top10Filter](../aspose.cells.top10filter/) for filtering data by rank of data. |
| [getFieldIndex()](#getFieldIndex--)| <b>@deprecated.</b> Please use the 'fieldIndex' property instead. Gets and sets the column offset in the range. |
| [setFieldIndex(number)](#setFieldIndex-number-)| <b>@deprecated.</b> Please use the 'fieldIndex' property instead. Gets and sets the column offset in the range. |
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

NOTE: This member is now obsolete. Instead,please use FilterColumn.MultipleFilters,CustomFilters and so on... property according to differnt type of filter This property will be removed 12 months later since October 2025. Aspose apologizes for any inconvenience you may have experienced.

### filterType {#filterType--}

Gets and sets the type fo filtering data.

```javascript
filterType : FilterType;
```


### multipleFilters {#multipleFilters--}

Gets [Aspose.Cells.MultipleFilterCollection](../aspose.cells.multiplefiltercollection/) for filtering data by labels or date time.

```javascript
multipleFilters : MultipleFilterCollection;
```


### customFilters {#customFilters--}

Gets [Aspose.Cells.CustomFilterCollection](../aspose.cells.customfiltercollection/) for filtering data by custom criteria.

```javascript
customFilters : CustomFilterCollection;
```


### colorFilter {#colorFilter--}

Readonly. Gets [Aspose.Cells.ColorFilter](../aspose.cells.colorfilter/) for filtering data by color.

```javascript
colorFilter : ColorFilter;
```


### dynamicFilter {#dynamicFilter--}

Readonly. Gets [Aspose.Cells.DynamicFilter](../aspose.cells.dynamicfilter/) for filtering with dynamic criteria.

```javascript
dynamicFilter : DynamicFilter;
```


### iconFilter {#iconFilter--}

Readonly. Gets [Aspose.Cells.IconFilter](../aspose.cells.iconfilter/) for filtering data by icon.

```javascript
iconFilter : IconFilter;
```


### top10Filter {#top10Filter--}

Readonly. Gets [Aspose.Cells.Top10Filter](../aspose.cells.top10filter/) for filtering data by rank of data.

```javascript
top10Filter : Top10Filter;
```


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

NOTE: This member is now obsolete. Instead,please use FilterColumn.MultipleFilters,CustomFilters and so on... property according to differnt type of filter This property will be removed 12 months later since October 2025. Aspose apologizes for any inconvenience you may have experienced.

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

NOTE: This member is now obsolete. Instead,please use FilterColumn.MultipleFilters,CustomFilters and so on... property according to differnt type of filter This property will be removed 12 months later since October 2025. Aspose apologizes for any inconvenience you may have experienced.

### getFilterType() {#getFilterType--}

<b>@deprecated.</b> Please use the 'filterType' property instead. Gets and sets the type fo filtering data.

```javascript
getFilterType() : FilterType;
```


**Returns**

[FilterType](../filtertype/)

### setFilterType(FilterType) {#setFilterType-filtertype-}

<b>@deprecated.</b> Please use the 'filterType' property instead. Gets and sets the type fo filtering data.

```javascript
setFilterType(value: FilterType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FilterType](../filtertype/) | The value to set. |

### getMultipleFilters() {#getMultipleFilters--}

<b>@deprecated.</b> Please use the 'multipleFilters' property instead. Gets [Aspose.Cells.MultipleFilterCollection](../aspose.cells.multiplefiltercollection/) for filtering data by labels or date time.

```javascript
getMultipleFilters() : MultipleFilterCollection;
```


**Returns**

[MultipleFilterCollection](../multiplefiltercollection/)

### setMultipleFilters(MultipleFilterCollection) {#setMultipleFilters-multiplefiltercollection-}

<b>@deprecated.</b> Please use the 'multipleFilters' property instead. Gets [Aspose.Cells.MultipleFilterCollection](../aspose.cells.multiplefiltercollection/) for filtering data by labels or date time.

```javascript
setMultipleFilters(value: MultipleFilterCollection) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MultipleFilterCollection](../multiplefiltercollection/) | The value to set. |

### getCustomFilters() {#getCustomFilters--}

<b>@deprecated.</b> Please use the 'customFilters' property instead. Gets [Aspose.Cells.CustomFilterCollection](../aspose.cells.customfiltercollection/) for filtering data by custom criteria.

```javascript
getCustomFilters() : CustomFilterCollection;
```


**Returns**

[CustomFilterCollection](../customfiltercollection/)

### setCustomFilters(CustomFilterCollection) {#setCustomFilters-customfiltercollection-}

<b>@deprecated.</b> Please use the 'customFilters' property instead. Gets [Aspose.Cells.CustomFilterCollection](../aspose.cells.customfiltercollection/) for filtering data by custom criteria.

```javascript
setCustomFilters(value: CustomFilterCollection) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CustomFilterCollection](../customfiltercollection/) | The value to set. |

### getColorFilter() {#getColorFilter--}

<b>@deprecated.</b> Please use the 'colorFilter' property instead. Gets [Aspose.Cells.ColorFilter](../aspose.cells.colorfilter/) for filtering data by color.

```javascript
getColorFilter() : ColorFilter;
```


**Returns**

[ColorFilter](../colorfilter/)

### getDynamicFilter() {#getDynamicFilter--}

<b>@deprecated.</b> Please use the 'dynamicFilter' property instead. Gets [Aspose.Cells.DynamicFilter](../aspose.cells.dynamicfilter/) for filtering with dynamic criteria.

```javascript
getDynamicFilter() : DynamicFilter;
```


**Returns**

[DynamicFilter](../dynamicfilter/)

### getIconFilter() {#getIconFilter--}

<b>@deprecated.</b> Please use the 'iconFilter' property instead. Gets [Aspose.Cells.IconFilter](../aspose.cells.iconfilter/) for filtering data by icon.

```javascript
getIconFilter() : IconFilter;
```


**Returns**

[IconFilter](../iconfilter/)

### getTop10Filter() {#getTop10Filter--}

<b>@deprecated.</b> Please use the 'top10Filter' property instead. Gets [Aspose.Cells.Top10Filter](../aspose.cells.top10filter/) for filtering data by rank of data.

```javascript
getTop10Filter() : Top10Filter;
```


**Returns**

[Top10Filter](../top10filter/)

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

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



