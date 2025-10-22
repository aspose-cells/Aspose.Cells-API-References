##TextFontAlignType Enum
'TextFontAlignType enum. Encapsulates the object that represents textfontaligntype in Go.'
## TextFontAlignType Enum
Represents the different types of font alignment.
```go
type TextFontAlignType int32
```
## Fields
| Field | Description |
| --- | --- |
|[Automatic](./automatic/) | When the text flow is horizontal or simple vertical same as fontBaselinebut for other vertical modes same as fontCenter. |
|[Bottom](./bottom/) | The letters are anchored to the very bottom of a single line. |
|[Baseline](./baseline/) | The letters are anchored to the bottom baseline of a single line. |
|[Center](./center/) | The letters are anchored between the two baselines of a single line. |
|[Top](./top/) | The letters are anchored to the top baseline of a single line. |
