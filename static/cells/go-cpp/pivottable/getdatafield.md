##GetDataField Method
'GetDataField method. Encapsulates the function that represents getdatafield in Go.'
## GetDataField function
Gets a PivotField object that represents all the data fields in a PivotTable.Read-only.It would only be created when there are two or more data fields in the Data region.Defaultly it is in row region. You can drag it to the row/column region with PivotTable.AddFieldToArea() method .
```go
func (instance *PivotTable) GetDataField()  (*PivotField,  error)
```
## Remarks
## See Also
* Class [PivotTable](../)
* Library [Aspose.Cells for Go](../../)
