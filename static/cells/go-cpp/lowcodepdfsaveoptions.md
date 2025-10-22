##LowCodePdfSaveOptions Class
'LowCodePdfSaveOptions class. Encapsulates the object that represents lowcodepdfsaveoptions in Go.'
## LowCodePdfSaveOptions class
Options for saving pdf in low code way.
```go
type LowCodePdfSaveOptions struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewLowCodePdfSaveOptions](./newlowcodepdfsaveoptions/) | Default constructor. |
|[NewLowCodePdfSaveOptions_LowCodeSaveOptions](./newlowcodepdfsaveoptions_lowcodesaveoptions/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetSaveFormat](./getsaveformat/) | The save format for the output.For converting to pdf, it can only be SaveFormat.Pdf. |
|[SetSaveFormat](./setsaveformat/) | The save format for the output.For converting to pdf, it can only be SaveFormat.Pdf. |
|[GetPdfOptions](./getpdfoptions/) | The options for saving Pdf file. |
|[SetPdfOptions](./setpdfoptions/) | The options for saving Pdf file. |
|[GetOutputFile](./getoutputfile/) | Gets and sets the file(with path if needed) for saving the generated data.When setting this property with value other than null or empty string, OutputStream will be ignored. |
|[SetOutputFile](./setoutputfile/) | Gets and sets the file(with path if needed) for saving the generated data.When setting this property with value other than null or empty string, OutputStream will be ignored. |
|[GetOutputStream](./getoutputstream/) | Gets and sets the Stream for writing the generated data to.When setting this property with value other than null, OutputFile will be ignored. |
|[SetOutputStream](./setoutputstream/) | Gets and sets the Stream for writing the generated data to.When setting this property with value other than null, OutputFile will be ignored. |
