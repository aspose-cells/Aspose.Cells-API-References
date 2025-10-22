##PdfBookmarkEntry Class
'PdfBookmarkEntry class. Encapsulates the object that represents pdfbookmarkentry in Go.'
## PdfBookmarkEntry class
PdfBookmarkEntry is an entry in pdf bookmark.if Text property of current instance is null or "",current instance will be hidden and children will be inserted on current level.
```go
type PdfBookmarkEntry struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewPdfBookmarkEntry](./newpdfbookmarkentry/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetText](./gettext/) | Title of a bookmark. |
|[SetText](./settext/) | Title of a bookmark. |
|[GetDestination](./getdestination/) | The cell to which the bookmark link. |
|[SetDestination](./setdestination/) | The cell to which the bookmark link. |
|[GetDestinationName](./getdestinationname/) | Gets or sets name of destination. |
|[SetDestinationName](./setdestinationname/) | Gets or sets name of destination. |
|[IsOpen](./isopen/) | When this property is true, the bookmarkentry will expand, otherwise it will collapse. |
|[SetIsOpen](./setisopen/) | When this property is true, the bookmarkentry will expand, otherwise it will collapse. |
|[IsCollapse](./iscollapse/) | When this property is true, the bookmarkentry will collapse, otherwise it will expand. |
|[SetIsCollapse](./setiscollapse/) | When this property is true, the bookmarkentry will collapse, otherwise it will expand. |
