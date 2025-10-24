##edit_page property
## edit_page property
The URL of the user-facing web page showing the web query data. This URL is persisted
in the case that sourceData="true" and url has been redirected to reference an XML file.
Then the user-facing page can be shown in the UI, and the XML data can be retrieved
behind the scenes.
### Remarks
NOTE: This property is now obsolete. Instead,
please use WebQueryConnection.EditWebPage property.
This property will be removed 12 months later since October 2017.
Aspose apologizes for any inconvenience you may have experienced.
### Definition:
```python
@property
def edit_page(self):
...
@edit_page.setter
def edit_page(self, value):
...
```
### See Also
* module [`aspose.cells.externalconnections`](../../)
* class [`WebQueryConnection`](/cells/python-net/aspose.cells.externalconnections/webqueryconnection)
