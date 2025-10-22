##AccessCacheOptions Enum
'AccessCacheOptions enum. Encapsulates the object that represents accesscacheoptions in Go.'
## AccessCacheOptions Enum
Cache options for data access. Can be combined with | operator for multiple options together.
```go
type AccessCacheOptions int32
```
## Fields
| Field | Description |
| --- | --- |
|[None](./none/) | No cache for any data access. |
|[All](./all/) | Apply all possible optimizations for all kinds of data access in the workbook.All settings and data should not be changed during the optimized access. |
|[PositionAndSize](./positionandsize/) | Apply possible optimization for getting object(such as Shape)'s position and size.Row height and column width settings should not be changed during the optimized access. |
|[CellsData](./cellsdata/) | Apply possible optimization for getting cells' values.Cells data(data and settings of Cell, Row) should not be changed duringthe optimized access, no new Cell/Row objects should be created either(such asby <see cref="Cells.this[int, int]"/>). |
|[CellDisplay](./celldisplay/) | Apply possible optimization for getting display-related results ofcells(<see cref="Cell.DisplayStringValue"/>, <see cref="Cell.GetStyle()"/>, <see cref="Cell.GetDisplayStyle()"/>, etc.).Cells data and style-related objects(Cell/Row/Column styles, column width, etc.) should not be changedduring the optimized access. |
|[GetFormula](./getformula/) | Apply possible optimization for getting formulas.All data and settings which may affect the formula expression(Worksheet's name, Name's text,table's column, etc.) should not be changed during the optimized access. |
|[SetFormula](./setformula/) | Apply possible optimization for setting formulas.All data and settings which may affect the formula expression(Worksheet's name, Name's text,table's column, etc.) should not be changed during the optimized access. |
|[CalculateFormula](./calculateformula/) | Apply possible optimization for calculating formulas.Cells data should not be changed during the optimized access, none new objects(Cell, Row, etc.)should be created either(such as by <see cref="Cells.this[int, int]"/>). |
|[ConditionalFormatting](./conditionalformatting/) | Apply possible optimization for getting formatting result of conditional formattings.All data and settings which may affect the result of conditional formattings(settings ofconditional formattings, dependent cell values, etc.) should not be changed during the optimized access. |
|[Validation](./validation/) | Apply possible optimization for getting validation result.All data and settings which may affect the result of validation(settings of the validation,dependent cell values, etc.) should not be changed during the optimized access. |
