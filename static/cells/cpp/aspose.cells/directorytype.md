##Aspose::Cells::DirectoryType enum
'Aspose::Cells::DirectoryType enum. Represents the directory type of the file name in C++.'
## DirectoryType enum
Represents the directory type of the file name.
```cpp
enum class DirectoryType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Volume | 0 | <br>Represents an MS-DOS drive letter. It is followed by the drive letter. Or UNC file names, such as \server\share\myfile.xls. |
| SameVolume | 1 | <br>Indicates that the source workbook is on the same drive as the dependent workbook (the drive letter is omitted) |
| DownDirectory | 2 | <br>Indicates that the source workbook is in a subdirectory of the current directory. |
| UpDirectory | 3 | <br>Indicates that the source workbook is in the parent directory of the current directory. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
