---
title: "AccessCacheOptions"
linktitle: "AccessCacheOptions"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Utility class containing constants."
type: docs
weight: 10
url: /nodejs/global/accesscacheoptions/
---

## AccessCacheOptions

Utility class containing constants. Cache options for data access. Can be combined with | operator for multiple options together. For some features, accessing large dataset requires a lot of repeated and complicated operations such as search, calculation, ...etc and those operations will take a lot of extra time. For common situations, all dependent data remains unchanged during the access, so some caches can be built and used to improve the access performance. For this purpose, we provide this API so that user can specify which kind of data access needs to be optimized by possible caching mechanism. Please note, for different options, different data set may be required to be "read-only". And performance of accessing data depends on many aspects, the use of caching mechanism does not guarantee that performance will be improved. For some situations, such as the dataset to be accessed is small, using cache may cause even more time because caching itself also needs certain extra time.

## Values

| Name | Description |
| --- | --- |
| NONE | No cache for any data access. |
| ALL | Apply all possible optimizations for all kinds of data access in the workbook. All settings and data should not be changed during the optimized access. |
| POSITION_AND_SIZE | Apply possible optimization for getting object(such as Shape)'s position and size. Row height and column width settings should not be changed during the optimized access. |
| CELLS_DATA | Apply possible optimization for getting cells' values. Cells data(data and settings of Cell, Row) should not be changed during the optimized access, no new Cell/Row objects should be created either(such as by #Error Cref: P:Aspose.Cells.Cells.Item(System.Int32,System.Int32)). |
| CELL_DISPLAY | Apply possible optimization for getting display-related results of cells(Cell.DisplayStringValue, Cell.getStyle(), Cell.getDisplayStyle(), etc.). Cells data and style-related objects(Cell/Row/Column styles, column width, etc.) should not be changed during the optimized access. |
| GET_FORMULA | Apply possible optimization for getting formulas. All data and settings which may affect the formula expression(Worksheet's name, Name's text, table's column, etc.) should not be changed during the optimized access. |
| SET_FORMULA | Apply possible optimization for setting formulas. All data and settings which may affect the formula expression(Worksheet's name, Name's text, table's column, etc.) should not be changed during the optimized access. |
| CALCULATE_FORMULA | Apply possible optimization for calculating formulas. Cells data should not be changed during the optimized access, none new objects(Cell, Row, etc.) should be created either(such as by #Error Cref: P:Aspose.Cells.Cells.Item(System.Int32,System.Int32)). |
| CONDITIONAL_FORMATTING | Apply possible optimization for getting formatting result of conditional formattings. All data and settings which may affect the result of conditional formattings(settings of conditional formattings, dependent cell values, etc.) should not be changed during the optimized access. |
| VALIDATION | Apply possible optimization for getting validation result. All data and settings which may affect the result of validation(settings of the validation, dependent cell values, etc.) should not be changed during the optimized access. |
