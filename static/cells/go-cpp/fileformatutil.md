##FileFormatUtil Class
'FileFormatUtil class. Encapsulates the object that represents fileformatutil in Go.'
## FileFormatUtil class
Provides utility methods for converting file format enums to strings or file extensions and back.
```go
type FileFormatUtil struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[FileFormatUtil_DetectFileFormat_Stream](./fileformatutil_detectfileformat_stream/) | Detects and returns the information about a format of an excel stored in a stream. |
|[FileFormatUtil_DetectFileFormat_Stream_String](./fileformatutil_detectfileformat_stream_string/) | Detects and returns the information about a format of an excel stored in a stream. |
|[FileFormatUtil_VerifyPassword](./fileformatutil_verifypassword/) | Detects and returns the information about a format of an excel stored in a stream. |
|[FileFormatUtil_DetectFileFormat_String](./fileformatutil_detectfileformat_string/) | Detects and returns the information about a format of an excel stored in a file. |
|[FileFormatUtil_DetectFileFormat_String_String](./fileformatutil_detectfileformat_string_string/) | Detects and returns the information about a format of an excel stored in a file. |
|[FileFormatUtil_FileFormatToSaveFormat](./fileformatutil_fileformattosaveformat/) | Converting file format to save format. |
|[FileFormatUtil_ExtensionToSaveFormat](./fileformatutil_extensiontosaveformat/) | Converts a file name extension into a SaveFormat value. |
|[FileFormatUtil_IsTemplateFormat](./fileformatutil_istemplateformat/) | Returns true if the extension is .xlt, .xltX, .xltm,.ots. |
|[FileFormatUtil_LoadFormatToExtension](./fileformatutil_loadformattoextension/) | Converts a load format enumerated value into a file extension. |
|[FileFormatUtil_LoadFormatToSaveFormat](./fileformatutil_loadformattosaveformat/) | Converts a LoadFormat value to a SaveFormat value if possible. |
|[FileFormatUtil_SaveFormatToExtension](./fileformatutil_saveformattoextension/) | Converts a save format enumerated value into a file extension. |
|[FileFormatUtil_SaveFormatToLoadFormat](./fileformatutil_saveformattoloadformat/) | Converts a SaveFormat value to a LoadFormat value if possible. |
