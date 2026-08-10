---
title: "CellValueFormatStrategy Enum"
linktitle: "CellValueFormatStrategy"
articleTitle: "CellValueFormatStrategy"
second_title: "Aspose.Cells for Python via Java"
description: "Utility class containing constants."
type: docs
weight: 580
url: /python-java/asposecells.api/cellvalueformatstrategy/
---

## CellValueFormatStrategy enumeration

Utility class containing constants. Specifies how to apply style for the value of the cell.

## Values

| Name | Description |
| --- | --- |
| NONE | Not formatted. |
| CELL_STYLE | Only formatted with the cell's original style. |
| DISPLAY_STYLE | Formatted with the cell's displayed style. |
| DISPLAY_STRING | Gets the displayed string shown in ms excel. The main difference from DISPLAY_STYLE is this option also considers the effect of column width. If the column width is too small to show the formatted string completely, "#" may be shown, just like what ms excel does. |
