##AboveAverage Class
'AboveAverage class. Encapsulates the object that represents aboveaverage in Go.'
## AboveAverage class
Describe the AboveAverage conditional formatting rule.This conditional formatting rule highlights cells thatare above or below the average for all values in the range.
```go
type AboveAverage struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewAboveAverage](./newaboveaverage/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[IsAboveAverage](./isaboveaverage/) | Get or set the flag indicating whether the rule is an "above average" rule.'true' indicates 'above average'.Default value is true. |
|[SetIsAboveAverage](./setisaboveaverage/) | Get or set the flag indicating whether the rule is an "above average" rule.'true' indicates 'above average'.Default value is true. |
|[IsEqualAverage](./isequalaverage/) | Get or set the flag indicating whether the 'aboveAverage' and 'belowAverage' criteriais inclusive of the average itself, or exclusive of that value.'true' indicates to include the average value in the criteria.Default value is false. |
|[SetIsEqualAverage](./setisequalaverage/) | Get or set the flag indicating whether the 'aboveAverage' and 'belowAverage' criteriais inclusive of the average itself, or exclusive of that value.'true' indicates to include the average value in the criteria.Default value is false. |
|[GetStdDev](./getstddev/) | Get or set the number of standard deviations to include above or below the average in theconditional formatting rule.The input value must between 0 and 3 (include 0 and 3).Setting this value to 0 means stdDev is not set.The default value is 0. |
|[SetStdDev](./setstddev/) | Get or set the number of standard deviations to include above or below the average in theconditional formatting rule.The input value must between 0 and 3 (include 0 and 3).Setting this value to 0 means stdDev is not set.The default value is 0. |
