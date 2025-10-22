##is_same_setting method
## is_same_setting(self, obj) {#System.Object}
Returns whether the shape is same.
### Returns
```python
def is_same_setting(self, obj):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| obj | System.Object |  |
### Example
```python
from aspose.cells import Workbook
# Instantiating a Workbook object
workbook = Workbook()
worksheet = workbook.worksheets[0]
# insert first picture
imgIndex1 = worksheet.pictures.add(1, 1, "1.png")
# Get the inserted picture object
pic1 = worksheet.pictures[imgIndex1]
# insert second picture
imgIndex2 = worksheet.pictures.add(1, 9, "2.jpeg")
# Get the inserted picture object
pic2 = worksheet.pictures[imgIndex2]
if pic1.is_same_setting(pic1):
pass
if notpic1.is_same_setting(pic2):
pass
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`Picture`](/cells/python-net/aspose.cells.drawing/picture)
