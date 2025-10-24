##get_picture method
## get_picture(self, is_header, section) {#bool-int}
Gets the [`Picture`](/cells/python-net/aspose.cells.drawing/picture) object of the header / footer.
### Returns
Returns [`Picture`](/cells/python-net/aspose.cells.drawing/picture) object.
Returns null if there is no picture.
```python
def get_picture(self, is_header, section):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| is_header | bool | Indicates whether it is in the header or footer. |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |
## get_picture(self, is_first, is_even, is_header, section) {#bool-bool-bool-int}
Gets the [`Picture`](/cells/python-net/aspose.cells.drawing/picture) object of the header / footer.
### Returns
Returns [`Picture`](/cells/python-net/aspose.cells.drawing/picture) object.
```python
def get_picture(self, is_first, is_even, is_header, section):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| is_first | bool | Indicates whether getting the picture of first page header/footer. |
| is_even | bool | Indicates whether getting the picture of even page header/footer. |
| is_header | bool | Indicates whether getting the picture of header/footer. |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |
### See Also
* module [`aspose.cells`](../../)
* class [`PageSetup`](/cells/python-net/aspose.cells/pagesetup)
* class [`Picture`](/cells/python-net/aspose.cells.drawing/picture)
