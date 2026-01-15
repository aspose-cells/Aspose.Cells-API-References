---
title: AccessCacheOptions
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Caching options for data access. Multiple options can be combined using the  operator.
type: docs
url: /javascript-cpp/accesscacheoptions/
---

## AccessCacheOptions enumeration
Caching options for data access. Multiple options can be combined using the "|" operator.
### Remarks
For some features, accessing large dataset requires a lot of repeated and complicated operations such as search, calculation, ...etc and those operations will take a lot of extra time. For common situations, all dependent data remains unchanged during the access, so some caches can be built and used to improve the access performance. For this purpose, we provide this API so that user can specify which kind of data access needs to be optimized by possible caching mechanism. <br></br> Please note, for different options, different data set may be required to be "read-only". And performance of accessing data depends on many aspects, the use of caching mechanism does not guarantee that performance will be improved. For some situations, such as the dataset to be accessed is small, using cache may cause even more time because caching itself also needs certain extra time.
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | No cache for any data access. |
| All | `-1` | Apply all possible optimizations for all kinds of data access in the workbook. All settings and data should not be changed during the optimized access. |
| PositionAndSize | `3` | Apply possible optimization for getting object(such as Shape)'s position and size. Row height and column width settings should not be changed during the optimized access. |
| CellsData | `9` | Apply possible optimization for getting cells' values. Cells data(data and settings of Cell, Row) should not be changed during the optimized access, no new Cell/Row objects should be created either(such as by [Cells.this[int, int]](../cells.this[int, int]/)). |
| CellDisplay | `1048710` | Apply possible optimization for getting display-related results of cells([Cell.DisplayStringValue](../cell.displaystringvalue/), [Cell.GetStyle()](../cell.getstyle()/), [Cell.GetDisplayStyle()](../cell.getdisplaystyle()/), etc.). Cells data and style-related objects(Cell/Row/Column styles, column width, etc.) should not be changed during the optimized access. |
| GetFormula | `2097152` | Apply possible optimization for getting formulas. All data and settings which may affect the formula expression(Worksheet's name, Name's text, table's column, etc.) should not be changed during the optimized access. |
| SetFormula | `4194304` | Apply possible optimization for setting formulas. All data and settings which may affect the formula expression(Worksheet's name, Name's text, table's column, etc.) should not be changed during the optimized access. |
| CalculateFormula | `8388617` | Apply possible optimization for calculating formulas. Cells data should not be changed during the optimized access, none new objects(Cell, Row, etc.) should be created either(such as by [Cells.this[int, int]](../cells.this[int, int]/)). |
| ConditionalFormatting | `16777225` | Apply possible optimization for getting formatting result of conditional formattings. All data and settings which may affect the result of conditional formattings(settings of conditional formattings, dependent cell values, etc.) should not be changed during the optimized access. |
| Validation | `33554441` | Apply possible optimization for getting validation result. All data and settings which may affect the result of validation(settings of the validation, dependent cell values, etc.) should not be changed during the optimized access. |

