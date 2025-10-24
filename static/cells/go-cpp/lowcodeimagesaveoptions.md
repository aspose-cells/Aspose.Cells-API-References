##LowCodeImageSaveOptions Class
'LowCodeImageSaveOptions class. Encapsulates the object that represents lowcodeimagesaveoptions in Go.'
## LowCodeImageSaveOptions class
Options for saving image in low code way.
```go
type LowCodeImageSaveOptions struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewLowCodeImageSaveOptions](./newlowcodeimagesaveoptions/) | Default constructor. |
|[NewLowCodeImageSaveOptions_LowCodeSaveOptions](./newlowcodeimagesaveoptions_lowcodesaveoptions/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetSaveFormat](./getsaveformat/) | Gets or sets the save format. |
|[SetSaveFormat](./setsaveformat/) | Gets or sets the save format. |
|[GetImageOptions](./getimageoptions/) | The options for rendering images. |
|[SetImageOptions](./setimageoptions/) | The options for rendering images. |
|[GetSaveOptionsProvider](./getsaveoptionsprovider/) | Provider of save options for saving generated images. |
|[SetSaveOptionsProvider](./setsaveoptionsprovider/) | Provider of save options for saving generated images. |
|[GetOutputFile](./getoutputfile/) | Gets and sets the file(with path if needed) for saving the generated data.When setting this property with value other than null or empty string, OutputStream will be ignored. |
|[SetOutputFile](./setoutputfile/) | Gets and sets the file(with path if needed) for saving the generated data.When setting this property with value other than null or empty string, OutputStream will be ignored. |
|[GetOutputStream](./getoutputstream/) | Gets and sets the Stream for writing the generated data to.When setting this property with value other than null, OutputFile will be ignored. |
|[SetOutputStream](./setoutputstream/) | Gets and sets the Stream for writing the generated data to.When setting this property with value other than null, OutputFile will be ignored. |
