##PasteType Enum
'PasteType enum. Encapsulates the object that represents pastetype in Go.'
## PasteType Enum
Represents the paste special type.
```go
type PasteType int32
```
## Fields
| Field | Description |
| --- | --- |
|[All](./all/) | Copies all data of the range. |
|[Default](./default/) | It works as "All" behavior of MS Excel. |
|[AllExceptBorders](./allexceptborders/) | Copies all data of the range without the range. |
|[DefaultExceptBorders](./defaultexceptborders/) | It works as "All except borders" behavior of MS Excel. |
|[ColumnWidths](./columnwidths/) | Only copies the widths of the range. |
|[RowHeights](./rowheights/) | Only copies the heights of the range. |
|[Comments](./comments/) | Only copies comments in the range. |
|[Formats](./formats/) | Only copies formats in the range. |
|[Formulas](./formulas/) | Only copies formulas in the range. |
|[FormulasAndNumberFormats](./formulasandnumberformats/) | Only copies formulas and number formats in the range. |
|[Validation](./validation/) | Only copies validations in the range. |
|[Values](./values/) | Only copies values in the range. |
|[ValuesAndFormats](./valuesandformats/) | Only copies values and formats in the range. |
|[ValuesAndNumberFormats](./valuesandnumberformats/) | Only copies values and number formats in the range. |
