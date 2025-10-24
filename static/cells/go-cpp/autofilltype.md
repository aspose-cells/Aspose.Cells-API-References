##AutoFillType Enum
'AutoFillType enum. Encapsulates the object that represents autofilltype in Go.'
## AutoFillType Enum
Represents the auto fill type.
```go
type AutoFillType int32
```
## Fields
| Field | Description |
| --- | --- |
|[Copy](./copy/) | Copies the value and format of the source area to the target area |
|[Default](./default/) | Automatically fills the target area with the value and format. |
|[Formats](./formats/) | Copies only the format of the source area to the target area, |
|[Series](./series/) | Extend the value in the source area to the target area in the form of a series and copy format to the target area. |
|[Values](./values/) | Copies only the value of the source area to the target area, |
