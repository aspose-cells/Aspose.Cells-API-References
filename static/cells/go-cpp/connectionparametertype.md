##ConnectionParameterType Enum
'ConnectionParameterType enum. Encapsulates the object that represents connectionparametertype in Go.'
## ConnectionParameterType Enum
Specifies the parameter type of external connection
```go
type ConnectionParameterType int32
```
## Fields
| Field | Description |
| --- | --- |
|[Cell](./cell/) | Get the parameter value from a cell on each refresh. |
|[Prompt](./prompt/) | Prompt the user on each refresh for a parameter value. |
|[Value](./value/) | Use a constant value on each refresh for the parameter value. |
