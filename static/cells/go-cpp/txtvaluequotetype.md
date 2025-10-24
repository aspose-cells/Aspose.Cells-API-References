##TxtValueQuoteType Enum
'TxtValueQuoteType enum. Encapsulates the object that represents txtvaluequotetype in Go.'
## TxtValueQuoteType Enum
Specifies the type of using quotation marks for values in text format files.
```go
type TxtValueQuoteType int32
```
## Fields
| Field | Description |
| --- | --- |
|[Normal](./normal/) | All values that contain special characters such as quotation mark, separator character will be quoted.Same with the behavior of ms excel for exporting text file. |
|[Always](./always/) | All values will be quoted always. |
|[Minimum](./minimum/) | Only quote values when needed. Such as, if one value contains quotation mark but the quotation mark is not at the begin of this value, this value will not be quoted. |
|[Never](./never/) | All values will not be quoted. The exported text file with this type may not be read back correctly because the needed quotation marks being absent. |
