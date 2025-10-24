##max_row property
## max_row property
Maximum row index of cell which contains data or style.
### Remarks
Return -1 if there is no cell which contains data or style in the worksheet.
This property needs to iterate and check cells and rows dynamically,
so it is a time-consumed progress and should not be invoked repeatedly,
such as using it directly as condition in a loop.
### Definition:
```python
@property
def max_row(self):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`Cells`](/cells/python-net/aspose.cells/cells)
