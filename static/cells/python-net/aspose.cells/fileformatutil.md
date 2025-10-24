##FileFormatUtil class
## FileFormatUtil class
Provides utility methods for converting file format enums to strings or file extensions and back.
The FileFormatUtil type exposes the following members:
### Methods
| Method | Description |
| :- | :- |
| [`detect_file_format(, stream)`](/cells/python-net/aspose.cells/fileformatutil/detect_file_format/#io.rawiobase) | Detects and returns the information about a format of an excel stored in a stream. |
| [`detect_file_format(, stream, password)`](/cells/python-net/aspose.cells/fileformatutil/detect_file_format/#io.rawiobase-system.string) | Detects and returns the information about a format of an excel stored in a stream. |
| [`detect_file_format(, file_path)`](/cells/python-net/aspose.cells/fileformatutil/detect_file_format/#system.string) | Detects and returns the information about a format of an excel stored in a file. |
| [`detect_file_format(, file_path, password)`](/cells/python-net/aspose.cells/fileformatutil/detect_file_format/#system.string-system.string) | Detects and returns the information about a format of an excel stored in a file. |
| [`verify_password(, stream, password)`](/cells/python-net/aspose.cells/fileformatutil/verify_password/#io.rawiobase-system.string) | Detects and returns the information about a format of an excel stored in a stream. |
| [`file_format_to_save_format(, format)`](/cells/python-net/aspose.cells/fileformatutil/file_format_to_save_format/#aspose.cells.fileformattype) | Converting file format to save format. |
| [`extension_to_save_format(, extension)`](/cells/python-net/aspose.cells/fileformatutil/extension_to_save_format/#system.string) | Converts a file name extension into a SaveFormat value. |
| [`is_template_format(, extension)`](/cells/python-net/aspose.cells/fileformatutil/is_template_format/#system.string) | Returns true if the extension is .xlt, .xltX, .xltm,.ots. |
| [`load_format_to_extension(, load_format)`](/cells/python-net/aspose.cells/fileformatutil/load_format_to_extension/#aspose.cells.loadformat) | Converts a load format enumerated value into a file extension. |
| [`load_format_to_save_format(, load_format)`](/cells/python-net/aspose.cells/fileformatutil/load_format_to_save_format/#aspose.cells.loadformat) | Converts a LoadFormat value to a SaveFormat value if possible. |
| [`save_format_to_extension(, format)`](/cells/python-net/aspose.cells/fileformatutil/save_format_to_extension/#aspose.cells.saveformat) | Converts a save format enumerated value into a file extension. |
| [`save_format_to_load_format(, save_format)`](/cells/python-net/aspose.cells/fileformatutil/save_format_to_load_format/#aspose.cells.saveformat) | Converts a SaveFormat value to a LoadFormat value if possible. |
### See Also
* module [`aspose.cells`](..)
