##edit_web_page property
## edit_web_page property
The URL of the user-facing web page showing the web query data. This URL is persisted
in the case that sourceData="true" and url has been redirected to reference an XML file.
Then the user-facing page can be shown in the UI, and the XML data can be retrieved
behind the scenes.
### Definition:
```python
@property
def edit_web_page(self):
...
@edit_web_page.setter
def edit_web_page(self, value):
...
```
### See Also
* module [`aspose.cells.externalconnections`](../../)
* class [`WebQueryConnection`](/cells/python-net/aspose.cells.externalconnections/webqueryconnection)
