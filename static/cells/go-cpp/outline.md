##Outline Class
'Outline class. Encapsulates the object that represents outline in Go.'
## Outline class
Represents an outline on a worksheet.
```go
type Outline struct  {
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
|[GetSummaryRowBelow](./getsummaryrowbelow/) | Indicates if the summary row will be positioned below the detail rows in the outline. |
|[SetSummaryRowBelow](./setsummaryrowbelow/) | Indicates if the summary row will be positioned below the detail rows in the outline. |
|[GetSummaryColumnRight](./getsummarycolumnright/) | Indicates if the summary column will be positioned to the right of the detail columns in the outline. |
|[SetSummaryColumnRight](./setsummarycolumnright/) | Indicates if the summary column will be positioned to the right of the detail columns in the outline. |
