##name property
## name property
Gets or sets the name of the data series.
### Example
```python
# Reference name to a cell
chart.n_series[0].name = "=A1"
# Set a string to name
chart.n_series[0].name = "First Series"
```
### Definition:
```python
@property
def name(self):
...
@name.setter
def name(self, value):
...
```
### See Also
* module [`aspose.cells.charts`](../../)
* class [`Series`](/cells/python-net/aspose.cells.charts/series)
