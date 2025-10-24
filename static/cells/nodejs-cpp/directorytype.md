##DirectoryType
Represents the directory  type of the file name.
## DirectoryType enumeration
Represents the directory  type of the file name.
### Values
| Name | Value | Description |
| --- | --- | --- |
| Volume | `0` | Represents an MS-DOS drive letter. It is followed by the drive letter. Or UNC file names, such as \\server\share\myfile.xls |
| SameVolume | `1` | Indicates that the source workbook is on the same drive as the dependent workbook (the drive letter is omitted) |
| DownDirectory | `2` | Indicates that the source workbook is in a subdirectory of the current directory. |
| UpDirectory | `3` | Indicates that the source workbook is in the parent directory of the current directory. |
