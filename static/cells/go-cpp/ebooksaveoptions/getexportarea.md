##GetExportArea Method
'GetExportArea method. Encapsulates the function that represents getexportarea in Go.'
## GetExportArea function
Gets or Sets the exporting CellArea of current active Worksheet.If you set this attribute, the print area of current active Worksheet will be omitted.Only the specified area will be exported when saving the file to html.
```go
func (instance *EbookSaveOptions) GetExportArea()  (*CellArea,  error)
```
## Remarks
## See Also
* Class [EbookSaveOptions](../)
* Library [Aspose.Cells for Go](../../)
