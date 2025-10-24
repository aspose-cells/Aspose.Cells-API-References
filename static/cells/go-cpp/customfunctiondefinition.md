##CustomFunctionDefinition Class
'CustomFunctionDefinition class. Encapsulates the object that represents customfunctiondefinition in Go.'
## CustomFunctionDefinition class
Definition of custom function for calculating with user's custom engine.
```go
type CustomFunctionDefinition struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewCustomFunctionDefinition](./newcustomfunctiondefinition/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetArrayModeParameters](./getarraymodeparameters/) | Gets the indices of given custom function's parameters that need to be calculated in array mode. |
