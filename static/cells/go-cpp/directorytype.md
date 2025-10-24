##DirectoryType Enum
'DirectoryType enum. Encapsulates the object that represents directorytype in Go.'
## DirectoryType Enum
Represents the directory  type of the file name.
```go
type DirectoryType int32
```
## Fields
| Field | Description |
| --- | --- |
|[Volume](./volume/) | Represents an MS-DOS drive letter. It is followed by the drive letter.Or UNC file names, such as \\server\share\myfile.xls |
|[SameVolume](./samevolume/) | Indicates that the source workbook is on the same drive as the dependent workbook (the drive letter is omitted) |
|[DownDirectory](./downdirectory/) | Indicates that the source workbook is in a subdirectory of the current directory. |
|[UpDirectory](./updirectory/) | Indicates that the source workbook is in the parent directory of the current directory. |
