##Column Class
'Column class. Encapsulates the object that represents column in Go.'
## Column class
Represents a single column in a worksheet.
```go
type Column struct  {
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
|[GetIndex](./getindex/) | Gets the index of this column. |
|[GetWidth](./getwidth/) | Gets and sets the column width in unit of characters. |
|[SetWidth](./setwidth/) | Gets and sets the column width in unit of characters. |
|[GetGroupLevel](./getgrouplevel/) | Gets the group level of the column. |
|[SetGroupLevel](./setgrouplevel/) | Gets the group level of the column. |
|[IsHidden](./ishidden/) | Indicates whether the column is hidden. |
|[SetIsHidden](./setishidden/) | Indicates whether the column is hidden. |
|[GetHasCustomStyle](./gethascustomstyle/) | Indicates whether this column has custom style settings(different from the default one inherited from workbook). |
|[ApplyStyle](./applystyle/) | Applies formats for a whole column. |
|[GetStyle](./getstyle/) | Gets the style of this column. |
|[SetStyle](./setstyle/) | Sets the style of this column. |
|[IsCollapsed](./iscollapsed/) | whether the column is collapsed |
|[SetIsCollapsed](./setiscollapsed/) | whether the column is collapsed |
