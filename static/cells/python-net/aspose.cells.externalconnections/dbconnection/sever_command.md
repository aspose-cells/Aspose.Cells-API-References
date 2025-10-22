##sever_command property
## sever_command property
Specifies a second command text string that is persisted when PivotTable server-based
page fields are in use.
For ODBC connections, serverCommand is usually a broader query than command (no
WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand),
parameter UI can be populated and parameterized queries can be constructed
### Remarks
NOTE: This property is now obsolete. Instead,
please use ExternalConnection.SecondCommand property.
This method will be removed 12 months later since October 2024.
Aspose apologizes for any inconvenience you may have experienced.
### Definition:
```python
@property
def sever_command(self):
...
@sever_command.setter
def sever_command(self, value):
...
```
### See Also
* module [`aspose.cells.externalconnections`](../../)
* class [`DBConnection`](/cells/python-net/aspose.cells.externalconnections/dbconnection)
