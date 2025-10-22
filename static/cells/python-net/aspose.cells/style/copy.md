##copy method
## copy(self, style) {#aspose.cells.Style}
Copies data from another style object
```python
def copy(self, style):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| style | aspose.cells.Style | Source Style object |
### Remarks
This method does not copy the name of the style.
If you want to copy the name, please call the following codes after copying style:
destStyle.Name = style.Name.
### See Also
* module [`aspose.cells`](../../)
* class [`Style`](/cells/python-net/aspose.cells/style)
