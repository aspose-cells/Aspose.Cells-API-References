##LowCodeHtmlSaveOptions Class
'LowCodeHtmlSaveOptions class. Encapsulates the object that represents lowcodehtmlsaveoptions in Go.'
## LowCodeHtmlSaveOptions class
Options for saving html in low code way.
```go
type LowCodeHtmlSaveOptions struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewLowCodeHtmlSaveOptions](./newlowcodehtmlsaveoptions/) | Default constructor. |
|[NewLowCodeHtmlSaveOptions_LowCodeSaveOptions](./newlowcodehtmlsaveoptions_lowcodesaveoptions/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetSaveFormat](./getsaveformat/) | Gets and sets the format of spreadsheet. |
|[SetSaveFormat](./setsaveformat/) | Gets and sets the format of spreadsheet. |
|[GetHtmlOptions](./gethtmloptions/) | The general options for saving html. |
|[SetHtmlOptions](./sethtmloptions/) | The general options for saving html. |
|[GetOutputFile](./getoutputfile/) | Gets and sets the file(with path if needed) for saving the generated data.When setting this property with value other than null or empty string, OutputStream will be ignored. |
|[SetOutputFile](./setoutputfile/) | Gets and sets the file(with path if needed) for saving the generated data.When setting this property with value other than null or empty string, OutputStream will be ignored. |
|[GetOutputStream](./getoutputstream/) | Gets and sets the Stream for writing the generated data to.When setting this property with value other than null, OutputFile will be ignored. |
|[SetOutputStream](./setoutputstream/) | Gets and sets the Stream for writing the generated data to.When setting this property with value other than null, OutputFile will be ignored. |
