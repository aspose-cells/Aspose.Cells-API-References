##merge_empty_td_forcely property
## merge_empty_td_forcely property
Indicates whether merging empty TD element forcedly when exporting file to html.
The size of html file will be reduced significantly after setting value to true. The default value is false.
If you want to import the html file to excel or export perfect grid lines when saving file to html,
please keep the default value.
### Definition:
```python
@property
def merge_empty_td_forcely(self):
...
@merge_empty_td_forcely.setter
def merge_empty_td_forcely(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`HtmlSaveOptions`](/cells/python-net/aspose.cells/htmlsaveoptions)
