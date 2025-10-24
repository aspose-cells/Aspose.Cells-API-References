##max_data_column property
## max_data_column property
Maximum column index of cell which contains data.
### Remarks
-1 will be returned if there is no cell which contains data.
This property needs to iterate and check all cells in a worksheet dynamically,
so it is a time-consumed progress and should not be invoked repeatedly,
such as using it directly as condition in a loop.
### Definition:
```python
@property
def max_data_column(self):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`Cells`](/cells/python-net/aspose.cells/cells)
