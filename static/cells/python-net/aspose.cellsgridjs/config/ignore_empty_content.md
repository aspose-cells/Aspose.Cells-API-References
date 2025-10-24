##ignore_empty_content property
## ignore_empty_content property
Sets/Gets whether to show  the max range which includes data ,style, merged cells and shapes.
if the last row or column contains cells with  no value and formula but has custom style
then we will not show this row/column when this vlaue is true。
the default value is true .
### Definition:
```python
@property
def ignore_empty_content(self):
...
@ignore_empty_content.setter
def ignore_empty_content(self, value):
...
```
### See Also
* module [`aspose.cellsgridjs`](../../)
* class [`Config`](/cells/python-net/aspose.cellsgridjs/config)
