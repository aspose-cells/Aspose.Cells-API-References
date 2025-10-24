##HtmlFormatHandlingType Enum
'HtmlFormatHandlingType enum. Encapsulates the object that represents htmlformathandlingtype in Go.'
## HtmlFormatHandlingType Enum
Specifies how to handle formatting from the HTML source
```go
type HtmlFormatHandlingType int32
```
## Fields
| Field | Description |
| --- | --- |
|[All](./all/) | Transfer all HTML formatting into the worksheet along with data. |
|[None](./none/) | Bring data in as unformatted text (setting data types still occurs). |
|[Rtf](./rtf/) | Translate HTML formatting to rich text formatting on the data brought into the worksheet. |
