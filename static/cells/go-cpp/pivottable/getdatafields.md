##GetDataFields Method
'GetDataFields method. Encapsulates the function that represents getdatafields in Go.'
## GetDataFields function
Gets a PivotField object that represents all the data fields in a PivotTable.Read-only.It would be init only when there are two or more data fields in the DataPiovtFiels.It only use to add DataPivotField to the PivotTable row/column area . Default is in row area.
```go
func (instance *PivotTable) GetDataFields()  (*PivotFieldCollection,  error)
```
## Remarks
## See Also
* Class [PivotTable](../)
* Library [Aspose.Cells for Go](../../)
