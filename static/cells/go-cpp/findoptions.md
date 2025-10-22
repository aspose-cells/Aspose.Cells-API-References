##FindOptions Class
'FindOptions class. Encapsulates the object that represents findoptions in Go.'
## FindOptions class
Represents find options.
```go
type FindOptions struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewFindOptions](./newfindoptions/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetCaseSensitive](./getcasesensitive/) | Indicates if the searched string is case sensitive. |
|[SetCaseSensitive](./setcasesensitive/) | Indicates if the searched string is case sensitive. |
|[GetLookAtType](./getlookattype/) | Look at type. |
|[SetLookAtType](./setlookattype/) | Look at type. |
|[GetRange](./getrange/) | Gets and sets the searched range. |
|[SetRange](./setrange/) | Sets the searched range. |
|[IsRangeSet](./israngeset/) | Indicates whether the searched range is set. |
|[GetSearchBackward](./getsearchbackward/) | Whether search backward for cells. |
|[SetSearchBackward](./setsearchbackward/) | Whether search backward for cells. |
|[GetSearchOrderByRows](./getsearchorderbyrows/) | Indicates whether search order by rows or columns. |
|[SetSearchOrderByRows](./setsearchorderbyrows/) | Indicates whether search order by rows or columns. |
|[GetLookInType](./getlookintype/) | Look in type. |
|[SetLookInType](./setlookintype/) | Look in type. |
|[GetRegexKey](./getregexkey/) | Indicates whether the searched key is regex.If true the searched key will be taken as regex and parsed.Otherwise the key will be parsed according to the rules in ms excel. |
|[SetRegexKey](./setregexkey/) | Indicates whether the searched key is regex.If true the searched key will be taken as regex and parsed.Otherwise the key will be parsed according to the rules in ms excel. |
|[GetValueTypeSensitive](./getvaluetypesensitive/) | Indicates whether searched cell value type should be same with the searched key. |
|[SetValueTypeSensitive](./setvaluetypesensitive/) | Indicates whether searched cell value type should be same with the searched key. |
|[GetStyle](./getstyle/) | The format to search for. |
|[SetStyle](./setstyle/) | The format to search for. |
|[GetConvertNumericData](./getconvertnumericdata/) | Gets or sets a value that indicates whether converting the searched string value to numeric data. |
|[SetConvertNumericData](./setconvertnumericdata/) | Gets or sets a value that indicates whether converting the searched string value to numeric data. |
