##Sparkline Class
'Sparkline class. Encapsulates the object that represents sparkline in Go.'
## Sparkline class
A sparkline represents a tiny chart or graphic in a worksheet cell that provides a visual representation of data.
```go
type Sparkline struct  {
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
|[GetDataRange](./getdatarange/) | Represents the data range of the sparkline. |
|[SetDataRange](./setdatarange/) | Represents the data range of the sparkline. |
|[GetRow](./getrow/) | Gets the row index of the sparkline. |
|[GetColumn](./getcolumn/) | Gets the column index of the sparkline. |
|[ToImage_String_ImageOrPrintOptions](./toimage_string_imageorprintoptions/) | Converts a sparkline to an image. |
|[ToImage_ImageOrPrintOptions](./toimage_imageorprintoptions/) | Converts a sparkline to an image. |
