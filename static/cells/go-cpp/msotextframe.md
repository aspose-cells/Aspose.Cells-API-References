##MsoTextFrame Class
'MsoTextFrame class. Encapsulates the object that represents msotextframe in Go.'
## MsoTextFrame class
Represents the text frame in a Shape object.
```go
type MsoTextFrame struct  {
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
|[GetAutoSize](./getautosize/) | Indicates if size of shape is adjusted automatically according to its content. |
|[SetAutoSize](./setautosize/) | Indicates if size of shape is adjusted automatically according to its content. |
|[IsAutoMargin](./isautomargin/) | Indicates whether the margin is auto calculated. |
|[SetIsAutoMargin](./setisautomargin/) | Indicates whether the margin is auto calculated. |
|[GetRotateTextWithShape](./getrotatetextwithshape/) | Indicates whether rotating text with shape. |
|[SetRotateTextWithShape](./setrotatetextwithshape/) | Indicates whether rotating text with shape. |
|[GetLeftMarginPt](./getleftmarginpt/) | Returns the left margin in unit of Points |
|[SetLeftMarginPt](./setleftmarginpt/) | Returns the left margin in unit of Points |
|[GetRightMarginPt](./getrightmarginpt/) | Returns the right margin in unit of Points |
|[SetRightMarginPt](./setrightmarginpt/) | Returns the right margin in unit of Points |
|[GetTopMarginPt](./gettopmarginpt/) | Returns the top margin in unit of Points |
|[SetTopMarginPt](./settopmarginpt/) | Returns the top margin in unit of Points |
|[GetBottomMarginPt](./getbottommarginpt/) | Returns the bottom margin in unit of Points |
|[SetBottomMarginPt](./setbottommarginpt/) | Returns the bottom margin in unit of Points |
