##second_command property
## second_command property
Specifies a second command text string that is persisted when PivotTable server-based
page fields are in use.
For ODBC connections, serverCommand is usually a broader query than command (no
WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand),
parameter UI can be populated and parameterized queries can be constructed
### Definition:
```python
@property
def second_command(self):
...
@second_command.setter
def second_command(self, value):
...
```
### See Also
* module [`aspose.cells.externalconnections`](../../)
* class [`DBConnection`](/cells/python-net/aspose.cells.externalconnections/dbconnection)
