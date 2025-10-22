##AxisBins Class
'AxisBins class. Encapsulates the object that represents axisbins in Go.'
## AxisBins class
Represents axis bins
```go
type AxisBins struct  {
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
|[IsByCategory](./isbycategory/) | Indicates whether grouping data by category |
|[SetIsByCategory](./setisbycategory/) | Indicates whether grouping data by category |
|[IsAutomatic](./isautomatic/) | Indicates whether the axis bins are automatic. |
|[SetIsAutomatic](./setisautomatic/) | Indicates whether the axis bins are automatic. |
|[GetWidth](./getwidth/) | Gets or sets the width of axis bin |
|[SetWidth](./setwidth/) | Gets or sets the width of axis bin |
|[GetCount](./getcount/) | Gets or set the count of axis bins |
|[SetCount](./setcount/) | Gets or set the count of axis bins |
|[GetOverflow](./getoverflow/) | Gets or set the overflow of axis bins |
|[SetOverflow](./setoverflow/) | Gets or set the overflow of axis bins |
|[GetUnderflow](./getunderflow/) | Gets or set the underflow of axis bins |
|[SetUnderflow](./setunderflow/) | Gets or set the underflow of axis bins |
