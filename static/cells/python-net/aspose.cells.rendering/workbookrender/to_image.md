##to_image method
## to_image(self, stream) {#io.RawIOBase}
Render whole workbook as Tiff Image to stream.
```python
def to_image(self, stream):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| stream | io.RawIOBase | the stream of the output image |
## to_image(self, filename) {#System.String}
Render whole workbook as Tiff Image to a file.
```python
def to_image(self, filename):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| filename | System.String | the filename of the output image |
## to_image(self, page_index, file_name) {#int-System.String}
Render certain page to a file.
```python
def to_image(self, page_index, file_name):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| page_index | int | indicate which page is to be converted |
| file_name | System.String | filename of the output image |
## to_image(self, page_index, stream) {#int-io.RawIOBase}
Render certain page to a stream.
```python
def to_image(self, page_index, stream):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| page_index | int | indicate which page is to be converted |
| stream | io.RawIOBase | the stream of the output image |
### See Also
* module [`aspose.cells.rendering`](../../)
* class [`WorkbookRender`](/cells/python-net/aspose.cells.rendering/workbookrender)
