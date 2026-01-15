---
title: AutoFilter
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents autofiltering for the specified worksheet.
type: docs
url: /javascript-cpp/autofilter/
---

## AutoFilter class

Represents autofiltering for the specified worksheet.

```javascript
class AutoFilter;
```


### Example
```javascript
const { Workbook, SaveFormat } = AsposeCells;

//Instantiating a Workbook object
var workbook = new Workbook(data);
//Accessing the first worksheet in the Excel file
var worksheet = workbook.worksheets.get(0);
//Creating AutoFilter by giving the cells range of the heading row
worksheet.autoFilter.range = "A1:C1";
//Filtering columns with specified values
worksheet.autoFilter.filter(2, "present");
// Refreshing auto filters to hide or unhide the rows.
worksheet.autoFilter.refresh();
//Saving the modified Excel file.
var uint8Array = workbook.save(SaveFormat.Xlsx);
```
## Properties

| Property | Type | Description |
| --- | --- | --- |
| [sorter](#sorter--)| DataSorter | Readonly. Gets the data sorter. |
| [range](#range--)| string | Represents the range to which the specified AutoFilter applies. |
| [showFilterButton](#showFilterButton--)| boolean | Indicates whether the AutoFilter button for this column is visible. |
| [filterColumns](#filterColumns--)| FilterColumnCollection | Readonly. Gets the collection of the filter columns. |

## Methods

| Method | Description |
| --- | --- |
| [setRange(number, number, number)](#setRange-number-number-number-)| Sets the range to which the specified AutoFilter applies. |
| [getCellArea()](#getCellArea--)| Gets the [CellArea](../cellarea/) where the this AutoFilter applies to. |
| [getCellArea(boolean)](#getCellArea-boolean-)| Gets the [Aspose.Cells.CellArea](../aspose.cells.cellarea/) where the specified AutoFilter applies. |
| [addFilter(number, string)](#addFilter-number-string-)| Adds a filter for a filter column. |
| [addDateFilter(number, DateTimeGroupingType, number, number, number, number, number, number)](#addDateFilter-number-datetimegroupingtype-number-number-number-number-number-number-)| Adds a date filter. |
| [removeDateFilter(number, DateTimeGroupingType, number, number, number, number, number, number)](#removeDateFilter-number-datetimegroupingtype-number-number-number-number-number-number-)| Removes a date filter. |
| [removeFilter(number, string)](#removeFilter-number-string-)| Removes a filter for a filter column. |
| [removeFilter(number)](#removeFilter-number-)| Remove the specific filter. |
| [filter(number, string)](#filter-number-string-)| Filters a list with specified criteria. |
| [filterTop10(number, boolean, boolean, number)](#filterTop10-number-boolean-boolean-number-)| Filter the top 10 items in the list |
| [dynamic_Filter(number, DynamicFilterType)](#dynamic_Filter-number-dynamicfiltertype-)| Adds a dynamic filter. |
| [addFontColorFilter(number, CellsColor)](#addFontColorFilter-number-cellscolor-)| Adds a font color filter. |
| [addFillColorFilter(number, BackgroundType, CellsColor, CellsColor)](#addFillColorFilter-number-backgroundtype-cellscolor-cellscolor-)| Adds a fill color filter. |
| [addIconFilter(number, IconSetType, number)](#addIconFilter-number-iconsettype-number-)| Adds an icon filter. |
| [matchBlanks(number)](#matchBlanks-number-)| Match all blank cells in the list. |
| [matchNonBlanks(number)](#matchNonBlanks-number-)| Match all not-blank cells in the list. |
| [custom(number, FilterOperatorType, VObject)](#custom-number-filteroperatortype-vobject-)| Filters a list with a custom criterion. |
| [custom(number, FilterOperatorType, VObject, boolean, FilterOperatorType, VObject)](#custom-number-filteroperatortype-vobject-boolean-filteroperatortype-vobject-)| Filters a list with custom criteria. |
| [showAll()](#showAll--)| Unhide all rows. |
| [refresh()](#refresh--)| Refresh auto filters to hide or unhide the rows. |
| [refresh(boolean)](#refresh-boolean-)| Gets all hidden rows' indexes. |


### sorter {#sorter--}

Readonly. Gets the data sorter.

```javascript
sorter : DataSorter;
```


### range {#range--}

Represents the range to which the specified AutoFilter applies.

```javascript
range : string;
```


### showFilterButton {#showFilterButton--}

Indicates whether the AutoFilter button for this column is visible.

```javascript
showFilterButton : boolean;
```


### filterColumns {#filterColumns--}

Readonly. Gets the collection of the filter columns.

```javascript
filterColumns : FilterColumnCollection;
```


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

Gets the [CellArea](../cellarea/) where the this AutoFilter applies to.

```javascript
getCellArea() : CellArea;
```


**Returns**

the area this filter applies to

### getCellArea(boolean) {#getCellArea-boolean-}

Gets the [Aspose.Cells.CellArea](../aspose.cells.cellarea/) where the specified AutoFilter applies.

```javascript
getCellArea(refreshAppliedRange: boolean) : CellArea;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| refreshAppliedRange | boolean | Whether refresh the applied range.         /// For the applied range of auto filter, the last row may change when cells data changes.         /// If this flag is true, then the last row of the range will be re-calculated according to current cells data. |

**Returns**

the area this filter applies to

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

Filter the top 10 items in the list

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

Match all blank cells in the list.

```javascript
matchBlanks(fieldIndex: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | number | The integer offset of the field on which you want to base the filter          /// (from the left of the list; the leftmost field is field 0). |

### matchNonBlanks(number) {#matchNonBlanks-number-}

Match all not-blank cells in the list.

```javascript
matchNonBlanks(fieldIndex: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | number | The integer offset of the field on which you want to base the filter          /// (from the left of the list; the leftmost field is field 0). |

### custom(number, FilterOperatorType, VObject) {#custom-number-filteroperatortype-vobject-}

Filters a list with a custom criterion.

```javascript
custom(fieldIndex: number, operatorType1: FilterOperatorType, criteria1: VObject) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | number | The integer offset of the field on which you want to base the filter          /// (from the left of the list; the leftmost field is field 0). |
| operatorType1 | [FilterOperatorType](../filteroperatortype/) | The filter operator type |
| criteria1 | VObject | The custom criteria |

### custom(number, FilterOperatorType, VObject, boolean, FilterOperatorType, VObject) {#custom-number-filteroperatortype-vobject-boolean-filteroperatortype-vobject-}

Filters a list with custom criteria.

```javascript
custom(fieldIndex: number, operatorType1: FilterOperatorType, criteria1: VObject, isAnd: boolean, operatorType2: FilterOperatorType, criteria2: VObject) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | number | The integer offset of the field on which you want to base the filter          /// (from the left of the list; the leftmost field is field 0). |
| operatorType1 | [FilterOperatorType](../filteroperatortype/) | The filter operator type |
| criteria1 | VObject | The custom criteria |
| isAnd | boolean |  |
| operatorType2 | [FilterOperatorType](../filteroperatortype/) | The filter operator type |
| criteria2 | VObject | The custom criteria |

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


