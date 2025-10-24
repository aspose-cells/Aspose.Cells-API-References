##TextOverflowType Enum
'TextOverflowType enum. Encapsulates the object that represents textoverflowtype in Go.'
## TextOverflowType Enum
Represents the way the text vertical or horizontal overflow.
```go
type TextOverflowType int32
```
## Fields
| Field | Description |
| --- | --- |
|[Clip](./clip/) | Pay attention to top and bottom barriers.Provide no indication that there is text which is not visible. |
|[Ellipsis](./ellipsis/) | Pay attention to top and bottom barriers.Use an ellipsis to denote that there is text which is not visible.Only for vertical overflow. |
|[Overflow](./overflow/) | Overflow the text and pay no attention to top and bottom barriers. |
