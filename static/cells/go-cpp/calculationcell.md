##CalculationCell Class
'CalculationCell class. Encapsulates the object that represents calculationcell in Go.'
## CalculationCell class
Represents the calculation relevant data about one cell which is being calculated.
```go
type CalculationCell struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[SetCalculatedValue](./setcalculatedvalue/) | Sets the calculated value for the cell. |
|[GetWorkbook](./getworkbook/) | Gets the Workbook object. |
|[GetWorksheet](./getworksheet/) | Gets the Worksheet object where the cell is in. |
|[GetCellRow](./getcellrow/) | Gets the row index of the cell. |
|[GetCellColumn](./getcellcolumn/) | Gets the column index of the cell. |
|[GetCell](./getcell/) | Gets the Cell object which is being calculated. |
