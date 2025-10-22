##QuartileCalculationType Enum
'QuartileCalculationType enum. Encapsulates the object that represents quartilecalculationtype in Go.'
## QuartileCalculationType Enum
Represents quartile calculation methods.
```go
type QuartileCalculationType int32
```
## Fields
| Field | Description |
| --- | --- |
|[Exclusive](./exclusive/) | The quartile calculation includes the median when splitting the dataset into quartiles. |
|[Inclusive](./inclusive/) | The quartile calculation excludes the median when splitting the dataset into quartiles. |
