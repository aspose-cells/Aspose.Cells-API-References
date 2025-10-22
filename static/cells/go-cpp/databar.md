##DataBar Class
'DataBar class. Encapsulates the object that represents databar in Go.'
## DataBar class
Describe the DataBar conditional formatting rule.This conditional formatting rule displays a gradateddata bar in the range of cells.
```go
type DataBar struct  {
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
|[GetAxisColor](./getaxiscolor/) | Gets the color of the axis for cells with conditional formatting as data bars. |
|[SetAxisColor](./setaxiscolor/) | Gets the color of the axis for cells with conditional formatting as data bars. |
|[GetAxisPosition](./getaxisposition/) | Gets or sets the position of the axis of the data bars specified by a conditional formatting rule. |
|[SetAxisPosition](./setaxisposition/) | Gets or sets the position of the axis of the data bars specified by a conditional formatting rule. |
|[GetBarFillType](./getbarfilltype/) | Gets or sets how a data bar is filled with color. |
|[SetBarFillType](./setbarfilltype/) | Gets or sets how a data bar is filled with color. |
|[GetDirection](./getdirection/) | Gets or sets the direction the databar is displayed. |
|[SetDirection](./setdirection/) | Gets or sets the direction the databar is displayed. |
|[GetBarBorder](./getbarborder/) | Gets an object that specifies the border of a data bar. |
|[GetNegativeBarFormat](./getnegativebarformat/) | Gets the NegativeBarFormat object associated with a data bar conditional formatting rule. |
|[GetMinCfvo](./getmincfvo/) | Get or set this DataBar's min value object.Cannot set null or CFValueObject with type FormatConditionValueType.Max to it. |
|[GetMaxCfvo](./getmaxcfvo/) | Get or set this DataBar's max value object.Cannot set null or CFValueObject with type FormatConditionValueType.Min to it. |
|[GetColor](./getcolor/) | Get or set this DataBar's Color. |
|[SetColor](./setcolor/) | Get or set this DataBar's Color. |
|[GetMinLength](./getminlength/) | Represents the min length of data bar . |
|[SetMinLength](./setminlength/) | Represents the min length of data bar . |
|[GetMaxLength](./getmaxlength/) | Represents the max length of data bar . |
|[SetMaxLength](./setmaxlength/) | Represents the max length of data bar . |
|[GetShowValue](./getshowvalue/) | Get or set the flag indicating whether to show the values of the cells on which this data bar is applied.Default value is true. |
|[SetShowValue](./setshowvalue/) | Get or set the flag indicating whether to show the values of the cells on which this data bar is applied.Default value is true. |
|[ToImage](./toimage/) | Render data bar in cell to image byte array. |
