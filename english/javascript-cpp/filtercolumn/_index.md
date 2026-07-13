---
title: FilterColumn
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents a filter for a single column or a column in the table.
type: docs
url: /javascript-cpp/filtercolumn/
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
| [filter](#filter--)| VObject | Gets and sets the condition of filtering data. |
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
| [selectAll()](#selectAll--)| Selects all. |


### isDropdownVisible {#isDropdownVisible--}

Indicates whether the AutoFilter button for this column is visible.

```javascript
isDropdownVisible : boolean;
```


### filter {#filter--}

Gets and sets the condition of filtering data.

```javascript
filter : VObject;
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


### selectAll() {#selectAll--}

Selects all.

```javascript
selectAll() : void;
```



