##max_data_row property
## max_data_row property
Maximum row index of cell which contains data.
### Remarks
Return -1 if there is no cell which contains data.
This property needs to iterate and check cells and rows dynamically,
so it is a time-consumed progress and should not be invoked repeatedly,
such as using it directly as condition in a loop.
### Definition:
```python
@property
def max_data_row(self):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`Cells`](/cells/python-net/aspose.cells/cells)
