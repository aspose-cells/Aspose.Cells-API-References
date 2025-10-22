##Aspose::Cells::LowCode::LowCodeSaveOptions class
'Aspose::Cells::LowCode::LowCodeSaveOptions class. Options for saving generated results in low code way in C++.'
## LowCodeSaveOptions class
Options for saving generated results in low code way.
```cpp
class LowCodeSaveOptions
```
## Methods
| Method | Description |
| --- | --- |
| [GetOutputFile()](./getoutputfile/) | Gets and sets the file(with path if needed) for saving the generated data. When setting this property with value other than null or empty string, OutputStream will be ignored. |
| [GetOutputStream()](./getoutputstream/) | Gets and sets the Stream for writing the generated data to. When setting this property with value other than null, OutputFile will be ignored. |
| [GetSaveFormat()](./getsaveformat/) | Gets and sets the save format for the output. Generally, for specific process in low code way, only some specific formats are allowed. Please specify the correct format for corresponding process, otherwise unexpected result or even exception may be caused. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [LowCodeSaveOptions()](./lowcodesaveoptions/) | Default constructor. |
| [LowCodeSaveOptions(LowCodeSaveOptions_Impl* impl)](./lowcodesaveoptions/) | Constructs from an implementation object. |
| [LowCodeSaveOptions(const LowCodeSaveOptions\& src)](./lowcodesaveoptions/) | Copy constructor. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const LowCodeSaveOptions\& src)](./operator_asm/) | operator= |
| [SetOutputFile(const U16String\& value)](./setoutputfile/) | Gets and sets the file(with path if needed) for saving the generated data. When setting this property with value other than null or empty string, OutputStream will be ignored. |
| [SetOutputFile(const char16_t* value)](./setoutputfile/) | Gets and sets the file(with path if needed) for saving the generated data. When setting this property with value other than null or empty string, OutputStream will be ignored. |
| [SetOutputStream(const Vector \<uint8_t\>\& value)](./setoutputstream/) | Gets and sets the Stream for writing the generated data to. When setting this property with value other than null, OutputFile will be ignored. |
| [SetSaveFormat(SaveFormat value)](./setsaveformat/) | Gets and sets the save format for the output. Generally, for specific process in low code way, only some specific formats are allowed. Please specify the correct format for corresponding process, otherwise unexpected result or even exception may be caused. |
| [~LowCodeSaveOptions()](./~lowcodesaveoptions/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells::LowCode](../)
* Library [Aspose.Cells for C++](../../)
