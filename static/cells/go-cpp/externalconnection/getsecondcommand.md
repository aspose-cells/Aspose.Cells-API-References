##GetSecondCommand Method
'GetSecondCommand method. Encapsulates the function that represents getsecondcommand in Go.'
## GetSecondCommand function
Specifies a second command text string that is persisted when PivotTable server-basedpage fields are in use.For ODBC connections, serverCommand is usually a broader query than command (noWHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand),parameter UI can be populated and parameterized queries can be constructed
```go
func (instance *ExternalConnection) GetSecondCommand()  (string,  error)
```
## Remarks
## See Also
* Class [ExternalConnection](../)
* Library [Aspose.Cells for Go](../../)
