---
title: "AutoFilter Class"
linktitle: "AutoFilter"
articleTitle: "AutoFilter"
second_title: "Aspose.Cells for Python via Java"
description: "Represents autofiltering for the specified worksheet."
type: docs
weight: 170
url: /python-java/asposecells.api/autofilter/
---

## AutoFilter class

Represents autofiltering for the specified worksheet.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Sorter](#sorter) | DataSorter | Gets the data sorter. |
| [Range](#range) | String | Represents the range to which the specified AutoFilter applies. |
| [ShowFilterButton](#showfilterbutton) | boolean | Indicates whether the AutoFilter button for this column is visible. |
| [FilterColumns](#filtercolumns) | FilterColumnCollection | Gets the collection of the filter columns. |

## Methods

| Name | Description |
| --- | --- |
| [setRange](#setrange) | Sets the range to which the specified AutoFilter applies. |
| [getCellArea](#getcellarea) | Gets the CellArea where the specified AutoFilter applies to. |
| [addFilter](#addfilter) | Adds a filter for a filter column.

MS Excel 2007 supports multiple selection in a filter column. |
| [addDateFilter](#adddatefilter) | Adds a date filter.

If DateTimeGroupingType is Year, only the param year effects. If DateTiemGroupingType is Month, onl |
| [removeDateFilter](#removedatefilter) | Removes a date filter.

If DateTimeGroupingType is Year, only the param year effects. If DateTiemGroupingType is Month,  |
| [removeFilter](#removefilter) | Removes a filter for a filter column. |
| [filter](#filter) | Filters a list with specified criteria.

Aspose.Cells will remove all other filter setting on this field as Ms Excel 97- |
| [filterTop10](#filtertop10) | Filter the top 10 item in the list |
| [dynamicFilter](#dynamicfilter) | Adds a dynamic filter. |
| [addFontColorFilter](#addfontcolorfilter) | Adds a font color filter. |
| [addFillColorFilter](#addfillcolorfilter) | Adds a fill color filter. |
| [addIconFilter](#addiconfilter) | Adds an icon filter.

Only supports to add the icon filter. Not supports checking which row is visible if the filter is  |
| [matchBlanks](#matchblanks) | Match all blank cell in the list. |
| [matchNonBlanks](#matchnonblanks) | Match all not blank cell in the list. |
| [custom](#custom) | Filters a list with a custom criteria. |
| [showAll](#showall) | Unhide all rows. |
| [refresh](#refresh) | Refresh auto filters to hide or unhide the rows. |

### AutoFilter.Sorter property {#sorter}

Gets the data sorter.

**Type:** DataSorter

### AutoFilter.Range property {#range}

Represents the range to which the specified AutoFilter applies.

**Type:** String

### AutoFilter.ShowFilterButton property {#showfilterbutton}

Indicates whether the AutoFilter button for this column is visible.

**Type:** boolean

### AutoFilter.FilterColumns property {#filtercolumns}

Gets the collection of the filter columns.

**Type:** FilterColumnCollection

### setRange(row, startColumn, endColumn) {#setrange}

Sets the range to which the specified AutoFilter applies.

| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index. |
| startColumn | int | Start column index. |
| endColumn | int | End column Index. |

### getCellArea() (1 of 2) {#getcellarea}

Gets the CellArea where the specified AutoFilter applies to.

---

### getCellArea(refreshAppliedRange) (2 of 2) {#getcellarea-1}

### addFilter(fieldIndex, criteria) {#addfilter}

Adds a filter for a filter column.

MS Excel 2007 supports multiple selection in a filter column.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| criteria | String | The specified criteria (a string; for example, "101"). It only can be null or be one of the cells' value in this column. |

### addDateFilter(fieldIndex, dateTimeGroupingType, year, month, day, hour, minute, second) {#adddatefilter}

Adds a date filter.

If DateTimeGroupingType is Year, only the param year effects. If DateTiemGroupingType is Month, only the param year and month effect.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| dateTimeGroupingType | int | A DateTimeGroupingType value. The grouping type |
| year | int | The year. |
| month | int | The month. |
| day | int | The day. |
| hour | int | The hour. |
| minute | int | The minute. |
| second | int | The second. |

### removeDateFilter(fieldIndex, dateTimeGroupingType, year, month, day, hour, minute, second) {#removedatefilter}

Removes a date filter.

If DateTimeGroupingType is Year, only the param year effects. If DateTiemGroupingType is Month, only the param year and month effect.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| dateTimeGroupingType | int | A DateTimeGroupingType value. The grouping type |
| year | int | The year. |
| month | int | The month. |
| day | int | The day. |
| hour | int | The hour. |
| minute | int | The minute. |
| second | int | The second. |

### removeFilter(fieldIndex, criteria) (1 of 2) {#removefilter}

Removes a filter for a filter column.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| criteria | String | The specified criteria (a string; for example, "101"). It only can be null or be one of the cells' value in this column. |

---

### removeFilter(fieldIndex) (2 of 2) {#removefilter-1}

Remove the specific filter.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | The specific filter index |

### filter(fieldIndex, criteria) {#filter}

Filters a list with specified criteria.

Aspose.Cells will remove all other filter setting on this field as Ms Excel 97-2003.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| criteria | String | The specified criteria (a string; for example, "101"). |

### filterTop10(fieldIndex, isTop, isPercent, itemCount) {#filtertop10}

Filter the top 10 item in the list

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| isTop | boolean | Indicates whether filter from top or bottom |
| isPercent | boolean | Indicates whether the items is percent or count |
| itemCount | int | The item count |

### dynamicFilter(fieldIndex, dynamicFilterType) {#dynamicfilter}

Adds a dynamic filter.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| dynamicFilterType | int | A DynamicFilterType value. Dynamic filter type. |

### addFontColorFilter(fieldIndex, color) {#addfontcolorfilter}

Adds a font color filter.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| color | CellsColor | The CellsColor object. |

### addFillColorFilter(fieldIndex, pattern, foregroundColor, backgroundColor) {#addfillcolorfilter}

Adds a fill color filter.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| pattern | int | A BackgroundType value. The background pattern type. |
| foregroundColor | CellsColor | The foreground color. |
| backgroundColor | CellsColor | The background color. |

### addIconFilter(fieldIndex, iconSetType, iconId) {#addiconfilter}

Adds an icon filter.

Only supports to add the icon filter. Not supports checking which row is visible if the filter is icon filter.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| iconSetType | int | A IconSetType value. The icon set type. |
| iconId | int | The icon id. |

### matchBlanks(fieldIndex) {#matchblanks}

Match all blank cell in the list.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |

### matchNonBlanks(fieldIndex) {#matchnonblanks}

Match all not blank cell in the list.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |

### custom(fieldIndex, operatorType1, criteria1) (1 of 2) {#custom}

Filters a list with a custom criteria.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| operatorType1 | int | A FilterOperatorType value. The filter operator type |
| criteria1 | Object | The custom criteria |

---

### custom(fieldIndex, operatorType1, criteria1, isAnd, operatorType2, criteria2) (2 of 2) {#custom-1}

Filters a list with custom criteria.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| operatorType1 | int | A FilterOperatorType value. The filter operator type |
| criteria1 | Object | The custom criteria |
| isAnd | boolean |  |
| operatorType2 | int | A FilterOperatorType value. The filter operator type |
| criteria2 | Object | The custom criteria |

### showAll() {#showall}

Unhide all rows.

### refresh() (1 of 2) {#refresh}

Refresh auto filters to hide or unhide the rows.

**Returns:** Returns all hidden rows' indexes.

---

### refresh(hideRows) (2 of 2) {#refresh-1}

Gets all hidden rows' indexes.

| Parameter | Type | Description |
| --- | --- | --- |
| hideRows | boolean | If true, hide the filtered rows. |

**Returns:** Returns all hidden rows indexes.
