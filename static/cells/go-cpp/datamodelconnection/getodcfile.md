##GetOdcFile Method
'GetOdcFile method. Encapsulates the function that represents getodcfile in Go.'
## GetOdcFile function
Specifies the full path to external connection file from which this connection wascreated. If a connection fails during an attempt to refresh data, and reconnectionMethod=1,then the spreadsheet application will try again using information from the external connection fileinstead of the connection object embedded within the workbook.
```go
func (instance *DataModelConnection) GetOdcFile()  (string,  error)
```
## Remarks
## See Also
* Class [DataModelConnection](../)
* Library [Aspose.Cells for Go](../../)
