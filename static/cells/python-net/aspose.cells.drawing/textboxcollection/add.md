##add method
## add(self, upper_left_row, upper_left_column, height, width) {#int-int-int-int}
Adds a textbox to the collection.
### Returns
[`TextBox`](/cells/python-net/aspose.cells.drawing/textbox) object index.
```python
def add(self, upper_left_row, upper_left_column, height, width):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| upper_left_row | int | Upper left row index. |
| upper_left_column | int | Upper left column index. |
| height | int | Height of textbox, in unit of pixel. |
| width | int | Width of textbox, in unit of pixel. |
### Example
```python
# add a TextBox
index2 = textBoxCollection.add(1, 1, 50, 100)
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`TextBox`](/cells/python-net/aspose.cells.drawing/textbox)
* class [`TextBoxCollection`](/cells/python-net/aspose.cells.drawing/textboxcollection)
