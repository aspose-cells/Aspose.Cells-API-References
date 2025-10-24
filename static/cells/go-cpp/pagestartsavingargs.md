##PageStartSavingArgs Class
'PageStartSavingArgs class. Encapsulates the object that represents pagestartsavingargs in Go.'
## PageStartSavingArgs class
Info for a page starts saving process.
```go
type PageStartSavingArgs struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewPageStartSavingArgs](./newpagestartsavingargs/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[IsToOutput](./istooutput/) | Gets or sets a value indicating whether the page should be output.The default value is true. |
|[SetIsToOutput](./setistooutput/) | Gets or sets a value indicating whether the page should be output.The default value is true. |
|[GetPageIndex](./getpageindex/) | Current page index, zero based. |
|[GetPageCount](./getpagecount/) | Total page count. |
