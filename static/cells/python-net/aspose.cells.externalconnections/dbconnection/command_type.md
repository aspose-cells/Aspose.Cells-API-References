##command_type property
## command_type property
Specifies the OLE DB command type.
1. Query specifies a cube name
2. Query specifies a SQL statement
3. Query specifies a table name
4. Query specifies that default information has been given, and it is up to the provider how to interpret.
5. Query is against a web based List Data Provider.
### Definition:
```python
@property
def command_type(self):
...
@command_type.setter
def command_type(self, value):
...
```
### See Also
* module [`aspose.cells.externalconnections`](../../)
* class [`DBConnection`](/cells/python-net/aspose.cells.externalconnections/dbconnection)
* class [`OLEDBCommandType`](/cells/python-net/aspose.cells.externalconnections/oledbcommandtype)
