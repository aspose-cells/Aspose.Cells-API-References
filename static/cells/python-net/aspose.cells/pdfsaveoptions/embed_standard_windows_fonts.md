##embed_standard_windows_fonts property
## embed_standard_windows_fonts property
True to embed true type fonts.
Affects only ASCII characters 32-127.
Fonts for character codes greater than 127 are always embedded.
Fonts are always embedded for PDF/A-1a, PDF/A-1b standard.
Default is true.
### Definition:
```python
@property
def embed_standard_windows_fonts(self):
...
@embed_standard_windows_fonts.setter
def embed_standard_windows_fonts(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`PdfSaveOptions`](/cells/python-net/aspose.cells/pdfsaveoptions)
