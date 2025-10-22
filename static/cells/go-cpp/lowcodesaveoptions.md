##LowCodeSaveOptions Class
'LowCodeSaveOptions class. Encapsulates the object that represents lowcodesaveoptions in Go.'
## LowCodeSaveOptions class
Options for saving generated results in low code way.
```go
type LowCodeSaveOptions struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewLowCodeSaveOptions](./newlowcodesaveoptions/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetOutputFile](./getoutputfile/) | Gets and sets the file(with path if needed) for saving the generated data.When setting this property with value other than null or empty string, OutputStream will be ignored. |
|[SetOutputFile](./setoutputfile/) | Gets and sets the file(with path if needed) for saving the generated data.When setting this property with value other than null or empty string, OutputStream will be ignored. |
|[GetOutputStream](./getoutputstream/) | Gets and sets the Stream for writing the generated data to.When setting this property with value other than null, OutputFile will be ignored. |
|[SetOutputStream](./setoutputstream/) | Gets and sets the Stream for writing the generated data to.When setting this property with value other than null, OutputFile will be ignored. |
|[GetSaveFormat](./getsaveformat/) | Gets and sets the save format for the output.Generally, for specific process in low code way, only some specific formats are allowed.Please specify the correct format for corresponding process, otherwise unexpected resultor even exception may be caused. |
|[SetSaveFormat](./setsaveformat/) | Gets and sets the save format for the output.Generally, for specific process in low code way, only some specific formats are allowed.Please specify the correct format for corresponding process, otherwise unexpected resultor even exception may be caused. |
