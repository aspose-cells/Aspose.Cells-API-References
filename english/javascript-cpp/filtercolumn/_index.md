---
title: FilterColumn
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents a filter for a single column.
type: docs
url: /javascript-cpp/filtercolumn/
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
| [filter](#filter--)| VObject | Gets and sets the condition of filtering data. |
| [filterType](#filterType--)| FilterType | Gets and sets the type fo filtering data. |
| [multipleFilters](#multipleFilters--)| MultipleFilterCollection | Gets [Aspose.Cells.MultipleFilterCollection](../aspose.cells.multiplefiltercollection/) for filtering data by labels or date time. |
| [customFilters](#customFilters--)| CustomFilterCollection | Gets [Aspose.Cells.CustomFilterCollection](../aspose.cells.customfiltercollection/) for filtering data by custom criteria. |
| [colorFilter](#colorFilter--)| ColorFilter | Readonly. Gets [Aspose.Cells.ColorFilter](../aspose.cells.colorfilter/) for filtering data by color. |
| [dynamicFilter](#dynamicFilter--)| DynamicFilter | Readonly. Gets [Aspose.Cells.DynamicFilter](../aspose.cells.dynamicfilter/) for filtering with dynamic criteria. |
| [iconFilter](#iconFilter--)| IconFilter | Readonly. Gets [Aspose.Cells.IconFilter](../aspose.cells.iconfilter/) for filtering data by icon. |
| [top10Filter](#top10Filter--)| Top10Filter | Readonly. Gets [Aspose.Cells.Top10Filter](../aspose.cells.top10filter/) for filtering data by rank of data. |
| [fieldIndex](#fieldIndex--)| number | Gets and sets the column offset in the range. |


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



