﻿---
title: AutoFilter
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents autofiltering for the specified worksheet.
type: docs
url: /nodejs-cpp/autofilter/
---

## AutoFilter class

Represents autofiltering for the specified worksheet.

```javascript
class AutoFilter;
```


## Methods

| Method | Description |
| --- | --- |
| [getSorter()](#getSorter--)| Gets the data sorter. |
| [getRange()](#getRange--)| Represents the range to which the specified AutoFilter applies. |
| [getShowFilterButton()](#getShowFilterButton--)| Indicates whether the AutoFilter button for this column is visible. |
| [setShowFilterButton(boolean)](#setShowFilterButton-boolean-)| Indicates whether the AutoFilter button for this column is visible. |
| [getFilterColumns()](#getFilterColumns--)| Gets the collection of the filter columns. |
| [setRange(number, number, number)](#setRange-number-number-number-)| Sets the range to which the specified AutoFilter applies. |
| [getCellArea()](#getCellArea--)| Gets the [CellArea](../cellarea/) where the specified AutoFilter applies to. |
| [addFilter(number, string)](#addFilter-number-string-)| Adds a filter for a filter column. |
| [addDateFilter(number, DateTimeGroupingType, number, number, number, number, number, number)](#addDateFilter-number-datetimegroupingtype-number-number-number-number-number-number-)| Adds a date filter. |
| [removeDateFilter(number, DateTimeGroupingType, number, number, number, number, number, number)](#removeDateFilter-number-datetimegroupingtype-number-number-number-number-number-number-)| Removes a date filter. |
| [removeFilter(number, string)](#removeFilter-number-string-)| Removes a filter for a filter column. |
| [removeFilter(number)](#removeFilter-number-)| Remove the specific filter. |
| [filter(number, string)](#filter-number-string-)| Filters a list with specified criteria. |
| [filterTop10(number, boolean, boolean, number)](#filterTop10-number-boolean-boolean-number-)| Filter the top 10 item in the list |
| [dynamic_Filter(number, DynamicFilterType)](#dynamic_Filter-number-dynamicfiltertype-)| Adds a dynamic filter. |
| [addFontColorFilter(number, CellsColor)](#addFontColorFilter-number-cellscolor-)| Adds a font color filter. |
| [addFillColorFilter(number, BackgroundType, CellsColor, CellsColor)](#addFillColorFilter-number-backgroundtype-cellscolor-cellscolor-)| Adds a fill color filter. |
| [addIconFilter(number, IconSetType, number)](#addIconFilter-number-iconsettype-number-)| Adds an icon filter. |
| [matchBlanks(number)](#matchBlanks-number-)| Match all blank cell in the list. |
| [matchNonBlanks(number)](#matchNonBlanks-number-)| Match all not blank cell in the list. |
| [custom(number, FilterOperatorType, object)](#custom-number-filteroperatortype-object-)| Filters a list with a custom criteria. |
| [custom(number, FilterOperatorType, object, boolean, FilterOperatorType, object)](#custom-number-filteroperatortype-object-boolean-filteroperatortype-object-)| Filters a list with custom criteria. |
| [showAll()](#showAll--)| Unhide all rows. |
| [refresh()](#refresh--)| Refresh auto filters to hide or unhide the rows. |
| [refresh(boolean)](#refresh-boolean-)| Gets all hidden rows' indexes. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### getSorter() {#getSorter--}

Gets the data sorter.

```javascript
getSorter() : DataSorter;
```


**Returns**

[DataSorter](../datasorter/)

### getRange() {#getRange--}

Represents the range to which the specified AutoFilter applies.

```javascript
getRange() : string;
```


### getShowFilterButton() {#getShowFilterButton--}

Indicates whether the AutoFilter button for this column is visible.

```javascript
getShowFilterButton() : boolean;
```


### setShowFilterButton(boolean) {#setShowFilterButton-boolean-}

Indicates whether the AutoFilter button for this column is visible.

```javascript
setShowFilterButton(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getFilterColumns() {#getFilterColumns--}

Gets the collection of the filter columns.

```javascript
getFilterColumns() : FilterColumnCollection;
```


**Returns**

[FilterColumnCollection](../filtercolumncollection/)

### setRange(number, number, number) {#setRange-number-number-number-}

Sets the range to which the specified AutoFilter applies.

```javascript
setRange(row: number, startColumn: number, endColumn: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | Row index. |
| startColumn | number | Start column index. |
| endColumn | number | End column Index. |

### getCellArea() {#getCellArea--}

Gets the [CellArea](../cellarea/) where the specified AutoFilter applies to.

```javascript
getCellArea() : CellArea;
```


**Returns**

[CellArea](../cellarea/)

### addFilter(number, string) {#addFilter-number-string-}

Adds a filter for a filter column.

```javascript
addFilter(fieldIndex: number, criteria: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | number | The integer offset of the field on which you want to base the filter          /// (from the left of the list; the leftmost field is field 0). |
| criteria | string | The specified criteria (a string; for example, "101").          /// It only can be null or be one of the cells' value in this column. |

**Remarks**

MS Excel 2007 supports multiple selection in a filter column.

### addDateFilter(number, DateTimeGroupingType, number, number, number, number, number, number) {#addDateFilter-number-datetimegroupingtype-number-number-number-number-number-number-}

Adds a date filter.

```javascript
addDateFilter(fieldIndex: number, dateTimeGroupingType: DateTimeGroupingType, year: number, month: number, day: number, hour: number, minute: number, second: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | number | The integer offset of the field on which you want to base the filter          /// (from the left of the list; the leftmost field is field 0). |
| dateTimeGroupingType | [DateTimeGroupingType](../datetimegroupingtype/) | The grouping type |
| year | number | The year. |
| month | number | The month. |
| day | number | The day. |
| hour | number | The hour. |
| minute | number | The minute. |
| second | number | The second. |

**Remarks**

If DateTimeGroupingType is Year, only the param year effects. If DateTiemGroupingType is Month, only the param year and month effect.

### removeDateFilter(number, DateTimeGroupingType, number, number, number, number, number, number) {#removeDateFilter-number-datetimegroupingtype-number-number-number-number-number-number-}

Removes a date filter.

```javascript
removeDateFilter(fieldIndex: number, dateTimeGroupingType: DateTimeGroupingType, year: number, month: number, day: number, hour: number, minute: number, second: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | number | The integer offset of the field on which you want to base the filter          /// (from the left of the list; the leftmost field is field 0). |
| dateTimeGroupingType | [DateTimeGroupingType](../datetimegroupingtype/) | The grouping type |
| year | number | The year. |
| month | number | The month. |
| day | number | The day. |
| hour | number | The hour. |
| minute | number | The minute. |
| second | number | The second. |

**Remarks**

If DateTimeGroupingType is Year, only the param year effects. If DateTiemGroupingType is Month, only the param year and month effect.

### removeFilter(number, string) {#removeFilter-number-string-}

Removes a filter for a filter column.

```javascript
removeFilter(fieldIndex: number, criteria: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | number | The integer offset of the field on which you want to base the filter          /// (from the left of the list; the leftmost field is field 0). |
| criteria | string | The specified criteria (a string; for example, "101").          /// It only can be null or be one of the cells' value in this column. |

### removeFilter(number) {#removeFilter-number-}

Remove the specific filter.

```javascript
removeFilter(fieldIndex: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | number | The specific filter index |

### filter(number, string) {#filter-number-string-}

Filters a list with specified criteria.

```javascript
filter(fieldIndex: number, criteria: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | number | The integer offset of the field on which you want to base the filter  		/// (from the left of the list; the leftmost field is field 0). 		 |
| criteria | string | The specified criteria (a string; for example, "101"). |

**Remarks**

Aspose.Cells will remove all other filter setting on this field as Ms Excel 97-2003.

### filterTop10(number, boolean, boolean, number) {#filterTop10-number-boolean-boolean-number-}

Filter the top 10 item in the list

```javascript
filterTop10(fieldIndex: number, isTop: boolean, isPercent: boolean, itemCount: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | number | The integer offset of the field on which you want to base the filter          /// (from the left of the list; the leftmost field is field 0). |
| isTop | boolean | Indicates whether filter from top or bottom |
| isPercent | boolean | Indicates whether the items is percent or count |
| itemCount | number | The item count |

### dynamic_Filter(number, DynamicFilterType) {#dynamic_Filter-number-dynamicfiltertype-}

Adds a dynamic filter.

```javascript
dynamic_Filter(fieldIndex: number, dynamicFilterType: DynamicFilterType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | number | The integer offset of the field on which you want to base the filter          /// (from the left of the list; the leftmost field is field 0). |
| dynamicFilterType | [DynamicFilterType](../dynamicfiltertype/) | Dynamic filter type. |

### addFontColorFilter(number, CellsColor) {#addFontColorFilter-number-cellscolor-}

Adds a font color filter.

```javascript
addFontColorFilter(fieldIndex: number, color: CellsColor) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | number | The integer offset of the field on which you want to base the filter          /// (from the left of the list; the leftmost field is field 0). |
| color | [CellsColor](../cellscolor/) | The [CellsColor](../cellscolor/) object. |

### addFillColorFilter(number, BackgroundType, CellsColor, CellsColor) {#addFillColorFilter-number-backgroundtype-cellscolor-cellscolor-}

Adds a fill color filter.

```javascript
addFillColorFilter(fieldIndex: number, pattern: BackgroundType, foregroundColor: CellsColor, backgroundColor: CellsColor) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | number | The integer offset of the field on which you want to base the filter          /// (from the left of the list; the leftmost field is field 0). |
| pattern | [BackgroundType](../backgroundtype/) | The background pattern type. |
| foregroundColor | [CellsColor](../cellscolor/) | The foreground color. |
| backgroundColor | [CellsColor](../cellscolor/) | The background color. |

### addIconFilter(number, IconSetType, number) {#addIconFilter-number-iconsettype-number-}

Adds an icon filter.

```javascript
addIconFilter(fieldIndex: number, iconSetType: IconSetType, iconId: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | number | The integer offset of the field on which you want to base the filter          /// (from the left of the list; the leftmost field is field 0). |
| iconSetType | [IconSetType](../iconsettype/) | The icon set type. |
| iconId | number | The icon id. |

**Remarks**

Only supports to add the icon filter. Not supports checking which row is visible if the filter is icon filter.

### matchBlanks(number) {#matchBlanks-number-}

Match all blank cell in the list.

```javascript
matchBlanks(fieldIndex: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | number | The integer offset of the field on which you want to base the filter          /// (from the left of the list; the leftmost field is field 0). |

### matchNonBlanks(number) {#matchNonBlanks-number-}

Match all not blank cell in the list.

```javascript
matchNonBlanks(fieldIndex: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | number | The integer offset of the field on which you want to base the filter          /// (from the left of the list; the leftmost field is field 0). |

### custom(number, FilterOperatorType, object) {#custom-number-filteroperatortype-object-}

Filters a list with a custom criteria.

```javascript
custom(fieldIndex: number, operatorType1: FilterOperatorType, criteria1: object) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | number | The integer offset of the field on which you want to base the filter          /// (from the left of the list; the leftmost field is field 0). |
| operatorType1 | [FilterOperatorType](../filteroperatortype/) | The filter operator type |
| criteria1 | object | The custom criteria |

### custom(number, FilterOperatorType, object, boolean, FilterOperatorType, object) {#custom-number-filteroperatortype-object-boolean-filteroperatortype-object-}

Filters a list with custom criteria.

```javascript
custom(fieldIndex: number, operatorType1: FilterOperatorType, criteria1: object, isAnd: boolean, operatorType2: FilterOperatorType, criteria2: object) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | number | The integer offset of the field on which you want to base the filter          /// (from the left of the list; the leftmost field is field 0). |
| operatorType1 | [FilterOperatorType](../filteroperatortype/) | The filter operator type |
| criteria1 | object | The custom criteria |
| isAnd | boolean |  |
| operatorType2 | [FilterOperatorType](../filteroperatortype/) | The filter operator type |
| criteria2 | object | The custom criteria |

### showAll() {#showAll--}

Unhide all rows.

```javascript
showAll() : void;
```


### refresh() {#refresh--}

Refresh auto filters to hide or unhide the rows.

```javascript
refresh() : number[];
```


**Returns**

Returns all hidden rows' indexes.

### refresh(boolean) {#refresh-boolean-}

Gets all hidden rows' indexes.

```javascript
refresh(hideRows: boolean) : number[];
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| hideRows | boolean | If true, hide the filtered rows. |

**Returns**

Returns all hidden rows indexes.

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



