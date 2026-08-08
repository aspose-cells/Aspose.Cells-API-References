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
| [addDateFilter(fieldIndex, dateTimeGroupingType, year, month, day, hour, minute, second)](./adddatefilter/) | Adds a date filter. If DateTimeGroupingType is Year, only the param year effects. If DateTiemGroupingType is Month, only |
| [addFillColorFilter(fieldIndex, pattern, foregroundColor, backgroundColor)](./addfillcolorfilter/) | Adds a fill color filter. |
| [addFilter(fieldIndex, criteria)](./addfilter/) | Adds a filter for a filter column. MS Excel 2007 supports multiple selection in a filter column. |
| [addFontColorFilter(fieldIndex, color)](./addfontcolorfilter/) | Adds a font color filter. |
| [addIconFilter(fieldIndex, iconSetType, iconId)](./addiconfilter/) | Adds an icon filter. Only supports to add the icon filter. Not supports checking which row is visible if the filter is i |
| [custom(fieldIndex, operatorType1, criteria1)](./custom/) | Filters a list with a custom criteria. |
| [custom(fieldIndex, operatorType1, criteria1, isAnd, operatorType2, criteria2)](./custom-1/) | Filters a list with custom criteria. |
| [dynamicFilter(fieldIndex, dynamicFilterType)](./dynamicfilter/) | Adds a dynamic filter. |
| [filter(fieldIndex, criteria)](./filter/) | Filters a list with specified criteria. Aspose.Cells will remove all other filter setting on this field as Ms Excel 97-2 |
| [filterTop10(fieldIndex, isTop, isPercent, itemCount)](./filtertop10/) | Filter the top 10 item in the list |
| [getCellArea()](./getcellarea/) | Gets the CellArea where the specified AutoFilter applies to. |
| [getCellArea()](./getcellarea-1/) |  |
| [getFilterColumns()](./getfiltercolumns/) | Gets the collection of the filter columns. |
| [getRange()](./getrange/) | Represents the range to which the specified AutoFilter applies. |
| [getShowFilterButton()](./getshowfilterbutton/) | Indicates whether the AutoFilter button for this column is visible. |
| [getSorter()](./getsorter/) | Gets the data sorter. |
| [matchBlanks(fieldIndex)](./matchblanks/) | Match all blank cell in the list. |
| [matchNonBlanks(fieldIndex)](./matchnonblanks/) | Match all not blank cell in the list. |
| [refresh()](./refresh/) | Refresh auto filters to hide or unhide the rows. |
| [refresh(hideRows)](./refresh-1/) | Gets all hidden rows' indexes. |
| [removeDateFilter(fieldIndex, dateTimeGroupingType, year, month, day, hour, minute, second)](./removedatefilter/) | Removes a date filter. If DateTimeGroupingType is Year, only the param year effects. If DateTiemGroupingType is Month, o |
| [removeFilter(fieldIndex, criteria)](./removefilter/) | Removes a filter for a filter column. |
| [removeFilter(fieldIndex)](./removefilter-1/) | Remove the specific filter. |
| [setRange()](./setrange/) | Represents the range to which the specified AutoFilter applies. |
| [setRange(row, startColumn, endColumn)](./setrange-1/) | Sets the range to which the specified AutoFilter applies. |
| [setShowFilterButton()](./setshowfilterbutton/) | Indicates whether the AutoFilter button for this column is visible. |
| [showAll()](./showall/) | Unhide all rows. |
