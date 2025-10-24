##TextConverter Class
'TextConverter class. Encapsulates the object that represents textconverter in Go.'
## TextConverter class
Converter for conversion between text based formats(csv, tsv, dif...) and other spreadsheet file formats.
```go
type TextConverter struct  {
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
|[TextConverter_Process_String_String](./textconverter_process_string_string/) | Converts given template file between text based files and other formats. |
|[TextConverter_Process_LowCodeLoadOptions_LowCodeSaveOptions](./textconverter_process_lowcodeloadoptions_lowcodesaveoptions/) | Converts file format between text based formats and other spreadsheet file formats |
