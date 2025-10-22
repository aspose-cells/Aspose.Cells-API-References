##save_options_provider property
## save_options_provider property
Provider of save options for saving generated images.
### Remarks
The output([`LowCodeSaveOptions.output_file`](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptions#output_file) or [`LowCodeSaveOptions.output_stream`](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptions#output_stream))
specified by this instance will take no effect when this property is specified.
Instead the output of every generated image will be specified by the provider.
### Definition:
```python
@property
def save_options_provider(self):
...
@save_options_provider.setter
def save_options_provider(self, value):
...
```
### See Also
* module [`aspose.cells.lowcode`](../../)
* class [`LowCodeImageSaveOptions`](/cells/python-net/aspose.cells.lowcode/lowcodeimagesaveoptions)
