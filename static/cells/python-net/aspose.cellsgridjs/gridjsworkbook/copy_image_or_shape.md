##copy_image_or_shape method
## copy_image_or_shape {#str-str}
Copys image or shape.
### Returns
The JSON format string of the new copied image
```python
def copy_image_or_shape(self, uid, p):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| uid | str | The unique id for the file cache. |
| p | str | The JSON format string for the operation which specify the cell location ,it contains the worksheet name,upper left row,upper left column for the image or shape，etc  {name:'sheet1',ri:1,ci:1,srcid:2,srcname:'sheet2',isshape:true} |
### See Also
* module [`aspose.cellsgridjs`](../../)
* class [`GridJsWorkbook`](/cells/python-net/aspose.cellsgridjs/gridjsworkbook)
