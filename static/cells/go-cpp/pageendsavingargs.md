##PageEndSavingArgs Class
'PageEndSavingArgs class. Encapsulates the object that represents pageendsavingargs in Go.'
## PageEndSavingArgs class
Info for a page ends saving process.
```go
type PageEndSavingArgs struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewPageEndSavingArgs](./newpageendsavingargs/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetHasMorePages](./gethasmorepages/) | Gets or sets a value indicating whether having more pages to be output.The default value is true. |
|[SetHasMorePages](./sethasmorepages/) | Gets or sets a value indicating whether having more pages to be output.The default value is true. |
|[GetPageIndex](./getpageindex/) | Current page index, zero based. |
|[GetPageCount](./getpagecount/) | Total page count. |
