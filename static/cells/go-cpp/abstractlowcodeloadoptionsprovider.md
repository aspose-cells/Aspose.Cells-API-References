##AbstractLowCodeLoadOptionsProvider Class
'AbstractLowCodeLoadOptionsProvider class. Encapsulates the object that represents abstractlowcodeloadoptionsprovider in Go.'
## AbstractLowCodeLoadOptionsProvider class
Implementation to provide multiple load options for processesthat use multiple inputs(such as template files).
```go
type AbstractLowCodeLoadOptionsProvider struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[MoveNext](./movenext/) | Checks whether there is more input. |
|[GetCurrent](./getcurrent/) | Gets the load options from which to load data of currently processed part. |
|[Finish](./finish/) | Releases resources after processing currently part of input. |
