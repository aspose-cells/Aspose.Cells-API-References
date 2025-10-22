##characters method
## characters(self, start_index, length) {#int-int}
Returns a Characters object that represents a range of characters within the comment text.
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
### Example
```python
fontSetting = comment1.characters(0, 4)
```
### See Also
* module [`aspose.cells`](../../)
* class [`Comment`](/cells/python-net/aspose.cells/comment)
* class [`FontSetting`](/cells/python-net/aspose.cells/fontsetting)
