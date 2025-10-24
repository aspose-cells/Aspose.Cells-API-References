##SetCommandType Method
'SetCommandType method. Encapsulates the function that represents setcommandtype in Go.'
## SetCommandType function
Specifies the OLE DB command type.1. Query specifies a cube name2. Query specifies a SQL statement3. Query specifies a table name4. Query specifies that default information has been given, and it is up to the provider how to interpret.5. Query is against a web based List Data Provider.
```go
func (instance *ExternalConnection) SetCommandType(value OLEDBCommandType)  error
```
## Remarks
## See Also
* Class [ExternalConnection](../)
* Library [Aspose.Cells for Go](../../)
