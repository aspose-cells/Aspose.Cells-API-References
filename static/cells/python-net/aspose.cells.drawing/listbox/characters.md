##characters method
## characters(self, start_index, length) {#int-int}
Returns a Characters object that represents a range of characters within the text.
### Returns
Characters object.
```python
def characters(self, start_index, length):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| start_index | int | The index of the start of the character. |
| length | int | The number of characters. |
### Remarks
This method only works on shape with title.
### Example
```python
fontSetting = shape.characters(0, 4)
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`FontSetting`](/cells/python-net/aspose.cells/fontsetting)
* class [`ListBox`](/cells/python-net/aspose.cells.drawing/listbox)
