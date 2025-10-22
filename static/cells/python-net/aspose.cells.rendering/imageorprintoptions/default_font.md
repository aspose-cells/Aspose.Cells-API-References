##default_font property
## default_font property
When characters in the Excel are Unicode and not be set with correct font in cell style,
They may appear as block in pdf,image.
Set the DefaultFont such as MingLiu or MS Gothic to show these characters.
If this property is not set, Aspose.Cells will use system default font to show these unicode characters.
### Definition:
```python
@property
def default_font(self):
...
@default_font.setter
def default_font(self, value):
...
```
### See Also
* module [`aspose.cells.rendering`](../../)
* class [`ImageOrPrintOptions`](/cells/python-net/aspose.cells.rendering/imageorprintoptions)
