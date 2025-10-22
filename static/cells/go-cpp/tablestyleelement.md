##TableStyleElement Class
'TableStyleElement class. Encapsulates the object that represents tablestyleelement in Go.'
## TableStyleElement class
Represents the element of the table style.
```go
type TableStyleElement struct  {
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
|[GetSize](./getsize/) | Number of rows or columns in a single band of striping.Applies only when type is firstRowStripe, secondRowStripe, firstColumnStripe, or secondColumnStripe. |
|[SetSize](./setsize/) | Number of rows or columns in a single band of striping.Applies only when type is firstRowStripe, secondRowStripe, firstColumnStripe, or secondColumnStripe. |
|[GetType](./gettype/) | Gets the element type. |
|[GetElementStyle](./getelementstyle/) | Gets the element style. |
|[SetElementStyle](./setelementstyle/) | Sets the element style. |
