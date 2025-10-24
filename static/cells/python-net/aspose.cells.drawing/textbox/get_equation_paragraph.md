##get_equation_paragraph method
## get_equation_paragraph(self) {#}
Gets the first math paragraph from the TextBody property of the TextBox object.
### Returns
If there has math paragraph, returns the first one, otherwise returns null.
```python
def get_equation_paragraph(self):
...
```
## get_equation_paragraph(self, index) {#int}
Get the specified math paragraph from the TextBody property of the TextBox object.
Notice:
(1) Returns NULL when the index is out of bounds or not found.
(2) Also returns NULL if the specified index position is not a math paragraph.
### Returns
Returns the math paragraph specified by index.
```python
def get_equation_paragraph(self, index):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| index | int | The position index of the math paragraph, starting from 0. |
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`TextBox`](/cells/python-net/aspose.cells.drawing/textbox)
