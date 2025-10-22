##Hyperlink Class
'Hyperlink class. Encapsulates the object that represents hyperlink in Go.'
## Hyperlink class
Encapsulates the object that represents a hyperlink.
```go
type Hyperlink struct  {
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
|[GetAddress](./getaddress/) | Represents the address of a hyperlink. |
|[SetAddress](./setaddress/) | Represents the address of a hyperlink. |
|[GetTextToDisplay](./gettexttodisplay/) | Represents the text to be displayed for the specified hyperlink. The default value is the address of the hyperlink. |
|[SetTextToDisplay](./settexttodisplay/) | Represents the text to be displayed for the specified hyperlink. The default value is the address of the hyperlink. |
|[GetArea](./getarea/) | Gets the range of hyperlink. |
|[GetScreenTip](./getscreentip/) | Returns or sets the ScreenTip text for the specified hyperlink. |
|[SetScreenTip](./setscreentip/) | Returns or sets the ScreenTip text for the specified hyperlink. |
|[GetLinkType](./getlinktype/) | Gets the link type. |
|[Delete](./delete/) | Deletes this hyperlink |
