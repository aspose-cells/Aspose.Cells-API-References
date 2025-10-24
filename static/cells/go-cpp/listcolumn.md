##ListColumn Class
'ListColumn class. Encapsulates the object that represents listcolumn in Go.'
## ListColumn class
Represents a column in a Table.
```go
type ListColumn struct  {
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
|[GetName](./getname/) | Gets and sets the name of the column. |
|[SetName](./setname/) | Gets and sets the name of the column. |
|[GetTotalsCalculation](./gettotalscalculation/) | Gets and sets the type of calculation in the Totals row of the list column. |
|[SetTotalsCalculation](./settotalscalculation/) | Gets and sets the type of calculation in the Totals row of the list column. |
|[GetRange](./getrange/) | Gets the range of this list column. |
|[GetCustomTotalsRowFormula](./getcustomtotalsrowformula/) | Gets the formula of totals row of this list column. |
|[SetCustomTotalsRowFormula](./setcustomtotalsrowformula/) | Gets the formula of totals row of this list column. |
|[IsArrayFormula](./isarrayformula/) | Indicates whether the fomula is array formula. |
|[GetFormula](./getformula/) | Gets and sets the formula of the list column. |
|[SetFormula](./setformula/) | Gets and sets the formula of the list column. |
|[GetCustomCalculatedFormula](./getcustomcalculatedformula/) | Gets the formula of this list column. |
|[SetCustomCalculatedFormula](./setcustomcalculatedformula/) | Sets the formula for this list column. |
|[GetTotalsRowLabel](./gettotalsrowlabel/) | Gets and sets the display labels of total row. |
|[SetTotalsRowLabel](./settotalsrowlabel/) | Gets and sets the display labels of total row. |
|[GetDataStyle](./getdatastyle/) | Gets the style of the data in this column of the table. |
|[SetDataStyle](./setdatastyle/) | Sets the style of the data in this column of the table. |
