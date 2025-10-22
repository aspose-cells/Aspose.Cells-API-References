##refresh_on_change property
## refresh_on_change property
Flag indicating whether the query should automatically refresh when the contents of a
cell that provides the parameter value changes. If true, then external data is refreshed
using the new parameter value every time there's a change. If false, then external data
is only refreshed when requested by the user, or some other event triggers refresh (e.g., workbook opened).
### Definition:
```python
@property
def refresh_on_change(self):
...
@refresh_on_change.setter
def refresh_on_change(self, value):
...
```
### See Also
* module [`aspose.cells.externalconnections`](../../)
* class [`ConnectionParameter`](/cells/python-net/aspose.cells.externalconnections/connectionparameter)
