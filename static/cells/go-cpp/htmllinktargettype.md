##HtmlLinkTargetType Enum
'HtmlLinkTargetType enum. Encapsulates the object that represents htmllinktargettype in Go.'
## HtmlLinkTargetType Enum
Represents the type of target attribute in HTML <a/> tag.
```go
type HtmlLinkTargetType int32
```
## Fields
| Field | Description |
| --- | --- |
|[Blank](./blank/) | Opens the linked document in a new window or tab |
|[Parent](./parent/) | Opens the linked document in the parent frame |
|[Self](./self/) | Opens the linked document in the same frame as it was clicked (this is default) |
|[Top](./top/) | Opens the linked document in the full body of the window |
