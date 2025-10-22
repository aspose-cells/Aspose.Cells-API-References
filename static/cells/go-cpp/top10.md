##Top10 Class
'Top10 class. Encapsulates the object that represents top10 in Go.'
## Top10 class
Describe the Top10 conditional formatting rule.This conditional formatting rule highlights cells whosevalues fall in the top N or bottom N bracket, as specified.
```go
type Top10 struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewTop10](./newtop10/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[IsPercent](./ispercent/) | Get or set whether a "top/bottom n" rule is a "top/bottom n percent" rule.Default value is false. |
|[SetIsPercent](./setispercent/) | Get or set whether a "top/bottom n" rule is a "top/bottom n percent" rule.Default value is false. |
|[IsBottom](./isbottom/) | Get or set whether a "top/bottom n" rule is a "bottom n" rule.Default value is false. |
|[SetIsBottom](./setisbottom/) | Get or set whether a "top/bottom n" rule is a "bottom n" rule.Default value is false. |
|[GetRank](./getrank/) | Get or set the value of "n" in a "top/bottom n" conditional formatting rule.If IsPercent is true, the value must between 0 and 100.Otherwise it must between 0 and 1000.Default value is 10. |
|[SetRank](./setrank/) | Get or set the value of "n" in a "top/bottom n" conditional formatting rule.If IsPercent is true, the value must between 0 and 100.Otherwise it must between 0 and 1000.Default value is 10. |
