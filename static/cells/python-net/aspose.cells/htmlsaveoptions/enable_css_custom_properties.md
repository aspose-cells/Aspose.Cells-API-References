##enable_css_custom_properties property
## enable_css_custom_properties property
Optimize the output of html by using CSS custom properties. For example, for the scenario that there are multiple occurences for one base64 image, with custom property the image data only needs to be saved once so the performance of the resultant html can be improved.
The default value is false.
### Definition:
```python
@property
def enable_css_custom_properties(self):
...
@enable_css_custom_properties.setter
def enable_css_custom_properties(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`HtmlSaveOptions`](/cells/python-net/aspose.cells/htmlsaveoptions)
