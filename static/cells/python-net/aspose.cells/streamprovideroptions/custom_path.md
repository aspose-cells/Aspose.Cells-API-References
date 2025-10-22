##custom_path property
## custom_path property
The user custom path(URL) saved in generated html file for the referred source. If not defined by user, DefaultPath will be used.
For example, the sheet data will be saved by user to d:/sheet001.htm, the url used in the main html file should be "d:/sheet001.htm" or other valid relative path that can be accessed by the main html file.
### Definition:
```python
@property
def custom_path(self):
...
@custom_path.setter
def custom_path(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`StreamProviderOptions`](/cells/python-net/aspose.cells/streamprovideroptions)
