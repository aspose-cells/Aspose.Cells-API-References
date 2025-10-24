##GetExportCellName Method
'GetExportCellName method. Encapsulates the function that represents getexportcellname in Go.'
## GetExportCellName function
Indicates if export cell name to Excel2007 .xlsx (.xlsm, .xltx, .xltm) file.If the output file may be accessed by SQL Server DTS, this value must be true.Setting the value to false will highly increase the performance and reduce the file size when creating large file.Default value is true.
```go
func (instance *OoxmlSaveOptions) GetExportCellName()  (bool,  error)
```
## Remarks
## See Also
* Class [OoxmlSaveOptions](../)
* Library [Aspose.Cells for Go](../../)
