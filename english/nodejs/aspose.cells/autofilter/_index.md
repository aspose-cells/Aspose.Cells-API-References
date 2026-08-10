---
title: "AutoFilter"
linktitle: "AutoFilter"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents autofiltering for the specified worksheet."
type: docs
weight: 140
url: /nodejs/aspose.cells/autofilter/
---

## AutoFilter class

Represents autofiltering for the specified worksheet.

## Methods

| Name | Description |
| --- | --- |
| [addDateFilter(fieldIndex, dateTimeGroupingType, year, month, day, hour, minute, second)](#adddatefilter) | Adds a date filter. If DateTimeGroupingType is Year, only the param year effects. If DateTiemGroupingType is Month, only |
| [addFillColorFilter(fieldIndex, pattern, foregroundColor, backgroundColor)](#addfillcolorfilter) | Adds a fill color filter. |
| [addFilter(fieldIndex, criteria)](#addfilter) | Adds a filter for a filter column. MS Excel 2007 supports multiple selection in a filter column. |
| [addFontColorFilter(fieldIndex, color)](#addfontcolorfilter) | Adds a font color filter. |
| [addIconFilter(fieldIndex, iconSetType, iconId)](#addiconfilter) | Adds an icon filter. Only supports to add the icon filter. Not supports checking which row is visible if the filter is i |
| [custom(fieldIndex, operatorType1, criteria1)](#custom) | Filters a list with a custom criteria. |
| [custom(fieldIndex, operatorType1, criteria1, isAnd, operatorType2, criteria2)](#custom-1) | Filters a list with custom criteria. |
| [dynamicFilter(fieldIndex, dynamicFilterType)](#dynamicfilter) | Adds a dynamic filter. |
| [filter(fieldIndex, criteria)](#filter) | Filters a list with specified criteria. Aspose.Cells will remove all other filter setting on this field as Ms Excel 97-2 |
| [filterTop10(fieldIndex, isTop, isPercent, itemCount)](#filtertop10) | Filter the top 10 item in the list |
| [getCellArea()](#getcellarea) | Gets the CellArea where the specified AutoFilter applies to. |
| [getCellArea()](#getcellarea-1) |  |
| [getFilterColumns()](#getfiltercolumns) | Gets the collection of the filter columns. |
| [getRange()](#getrange) | Represents the range to which the specified AutoFilter applies. |
| [getShowFilterButton()](#getshowfilterbutton) | Indicates whether the AutoFilter button for this column is visible. |
| [getSorter()](#getsorter) | Gets the data sorter. |
| [matchBlanks(fieldIndex)](#matchblanks) | Match all blank cell in the list. |
| [matchNonBlanks(fieldIndex)](#matchnonblanks) | Match all not blank cell in the list. |
| [refresh()](#refresh) | Refresh auto filters to hide or unhide the rows. |
| [refresh(hideRows)](#refresh-1) | Gets all hidden rows' indexes. |
| [removeDateFilter(fieldIndex, dateTimeGroupingType, year, month, day, hour, minute, second)](#removedatefilter) | Removes a date filter. If DateTimeGroupingType is Year, only the param year effects. If DateTiemGroupingType is Month, o |
| [removeFilter(fieldIndex, criteria)](#removefilter) | Removes a filter for a filter column. |
| [removeFilter(fieldIndex)](#removefilter-1) | Remove the specific filter. |
| [setRange()](#setrange) | Represents the range to which the specified AutoFilter applies. |
| [setRange(row, startColumn, endColumn)](#setrange-1) | Sets the range to which the specified AutoFilter applies. |
| [setShowFilterButton()](#setshowfilterbutton) | Indicates whether the AutoFilter button for this column is visible. |
| [showAll()](#showall) | Unhide all rows. |

### addDateFilter(fieldIndex, dateTimeGroupingType, year, month, day, hour, minute, second) {#adddatefilter}

Adds a date filter. If DateTimeGroupingType is Year, only the param year effects. If DateTiemGroupingType is Month, only the param year and month effect.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Number | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| dateTimeGroupingType | Number | DateTimeGroupingType |
| year | Number | The year. |
| month | Number | The month. |
| day | Number | The day. |
| hour | Number | The hour. |
| minute | Number | The minute. |
| second | Number | The second. |

### addFillColorFilter(fieldIndex, pattern, foregroundColor, backgroundColor) {#addfillcolorfilter}

Adds a fill color filter.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Number | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| pattern | Number | BackgroundType |
| foregroundColor | CellsColor | The foreground color. |
| backgroundColor | CellsColor | The background color. |

### addFilter(fieldIndex, criteria) {#addfilter}

Adds a filter for a filter column. MS Excel 2007 supports multiple selection in a filter column.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Number | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| criteria | String | The specified criteria (a string; for example, "101"). It only can be null or be one of the cells' value in this column. |

### addFontColorFilter(fieldIndex, color) {#addfontcolorfilter}

Adds a font color filter.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Number | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| color | CellsColor | The |

### addIconFilter(fieldIndex, iconSetType, iconId) {#addiconfilter}

Adds an icon filter. Only supports to add the icon filter. Not supports checking which row is visible if the filter is icon filter.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Number | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| iconSetType | Number | IconSetType |
| iconId | Number | The icon id. |

### custom(fieldIndex, operatorType1, criteria1) {#custom}

Filters a list with a custom criteria.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Number | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| operatorType1 | Number | FilterOperatorType |
| criteria1 | Object | The custom criteria |

### custom(fieldIndex, operatorType1, criteria1, isAnd, operatorType2, criteria2) {#custom-1}

Filters a list with custom criteria.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Number | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| operatorType1 | Number | FilterOperatorType |
| criteria1 | Object | The custom criteria |
| isAnd | boolean |  |
| operatorType2 | Number | FilterOperatorType |
| criteria2 | Object | The custom criteria |

### dynamicFilter(fieldIndex, dynamicFilterType) {#dynamicfilter}

Adds a dynamic filter.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Number | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| dynamicFilterType | Number | DynamicFilterType |

### filter(fieldIndex, criteria) {#filter}

Filters a list with specified criteria. Aspose.Cells will remove all other filter setting on this field as Ms Excel 97-2003.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Number | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| criteria | String | The specified criteria (a string; for example, "101"). |

### filterTop10(fieldIndex, isTop, isPercent, itemCount) {#filtertop10}

Filter the top 10 item in the list

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Number | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| isTop | boolean | Indicates whether filter from top or bottom |
| isPercent | boolean | Indicates whether the items is percent or count |
| itemCount | Number | The item count |

### getCellArea() {#getcellarea}

Gets the CellArea where the specified AutoFilter applies to.

**Returns:** CellArea — `CellArea`

### getCellArea() {#getcellarea-1}

### getFilterColumns() {#getfiltercolumns}

Gets the collection of the filter columns.

### getRange() {#getrange}

Represents the range to which the specified AutoFilter applies.

### getShowFilterButton() {#getshowfilterbutton}

Indicates whether the AutoFilter button for this column is visible.

### getSorter() {#getsorter}

Gets the data sorter.

### matchBlanks(fieldIndex) {#matchblanks}

Match all blank cell in the list.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Number | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |

### matchNonBlanks(fieldIndex) {#matchnonblanks}

Match all not blank cell in the list.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Number | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |

### refresh() {#refresh}

Refresh auto filters to hide or unhide the rows.

**Returns:** Array of Number — `Array of Number` Returns all hidden rows' indexes.

### refresh(hideRows) {#refresh-1}

Gets all hidden rows' indexes.

| Parameter | Type | Description |
| --- | --- | --- |
| hideRows | boolean | If true, hide the filtered rows. |

**Returns:** Array of Number — `Array of Number` Returns all hidden rows indexes.

### removeDateFilter(fieldIndex, dateTimeGroupingType, year, month, day, hour, minute, second) {#removedatefilter}

Removes a date filter. If DateTimeGroupingType is Year, only the param year effects. If DateTiemGroupingType is Month, only the param year and month effect.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Number | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| dateTimeGroupingType | Number | DateTimeGroupingType |
| year | Number | The year. |
| month | Number | The month. |
| day | Number | The day. |
| hour | Number | The hour. |
| minute | Number | The minute. |
| second | Number | The second. |

### removeFilter(fieldIndex, criteria) {#removefilter}

Removes a filter for a filter column.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Number | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| criteria | String | The specified criteria (a string; for example, "101"). It only can be null or be one of the cells' value in this column. |

### removeFilter(fieldIndex) {#removefilter-1}

Remove the specific filter.

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Number | The specific filter index |

### setRange() {#setrange}

Represents the range to which the specified AutoFilter applies.

### setRange(row, startColumn, endColumn) {#setrange-1}

Sets the range to which the specified AutoFilter applies.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index. |
| startColumn | Number | Start column index. |
| endColumn | Number | End column Index. |

### setShowFilterButton() {#setshowfilterbutton}

Indicates whether the AutoFilter button for this column is visible.

### showAll() {#showall}

Unhide all rows.
