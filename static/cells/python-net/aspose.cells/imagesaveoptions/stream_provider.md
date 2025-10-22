##stream_provider property
## stream_provider property
Gets or sets the IStreamProvider for exporting objects.
### Remarks
If saving as Tiff, this property is ignored.
Otherwise, if more than one image should be saving, we will write other images by this.
For advanced usage, please use [`WorkbookRender`](/cells/python-net/aspose.cells.rendering/workbookrender) or [`SheetRender`](/cells/python-net/aspose.cells.rendering/sheetrender).
### Definition:
```python
@property
def stream_provider(self):
...
@stream_provider.setter
def stream_provider(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`IStreamProvider`](/cells/python-net/aspose.cells/istreamprovider)
* class [`ImageSaveOptions`](/cells/python-net/aspose.cells/imagesaveoptions)
* class [`SheetRender`](/cells/python-net/aspose.cells.rendering/sheetrender)
* class [`WorkbookRender`](/cells/python-net/aspose.cells.rendering/workbookrender)
