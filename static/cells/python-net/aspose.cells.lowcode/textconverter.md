##TextConverter class
## TextConverter class
Converter for conversion between text based formats(csv, tsv, dif...) and other spreadsheet file formats.
The TextConverter type exposes the following members:
### Methods
| Method | Description |
| :- | :- |
| [`process(, template_file, result_file)`](/cells/python-net/aspose.cells.lowcode/textconverter/process/#system.string-system.string) | Converts given template file between text based files and other formats. |
| [`process(, load_options, save_options)`](/cells/python-net/aspose.cells.lowcode/textconverter/process/#aspose.cells.lowcode.lowcodeloadoptions-aspose.cells.lowcode.lowcodesaveoptions) | Converts file format between text based formats and other spreadsheet file formats |
### Example
```python
from aspose.cells.lowcode import TextConverter
TextConverter.process("template.csv", "res.xlsx")
```
### See Also
* module [`aspose.cells.lowcode`](..)
