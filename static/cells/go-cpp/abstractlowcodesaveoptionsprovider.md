##AbstractLowCodeSaveOptionsProvider Class
'AbstractLowCodeSaveOptionsProvider class. Encapsulates the object that represents abstractlowcodesaveoptionsprovider in Go.'
## AbstractLowCodeSaveOptionsProvider class
Implementation to provide multiple save options for processesthat require multiple outputs. For example,<see cref="SpreadsheetSplitter"/> feature requires multiple destinationsto save the split files.
```go
type AbstractLowCodeSaveOptionsProvider struct  {
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
|[GetSaveOptions](./getsaveoptions/) | Gets the save options from which to get the output settings for currently split part.Returning null denotes to skip given part. |
|[Finish](./finish/) | Releases resources after processing currently split part. |
