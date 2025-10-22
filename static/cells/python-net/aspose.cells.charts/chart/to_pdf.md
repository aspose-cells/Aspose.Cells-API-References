##to_pdf method
## to_pdf(self, file_name) {#System.String}
Saves the chart to a pdf file.
```python
def to_pdf(self, file_name):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| file_name | System.String | the pdf file name with full path |
## to_pdf(self, stream) {#io.RawIOBase}
Creates the chart pdf and saves it to a stream.
```python
def to_pdf(self, stream):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| stream | io.RawIOBase | The output stream. |
## to_pdf(self, file_name, desired_page_width, desired_page_height, h_alignment_type, v_alignment_type) {#System.String-float-float-aspose.cells.PageLayoutAlignmentType-aspose.cells.PageLayoutAlignmentType}
Saves the chart to a pdf file.
```python
def to_pdf(self, file_name, desired_page_width, desired_page_height, h_alignment_type, v_alignment_type):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| file_name | System.String | the pdf file name with full path |
| desired_page_width | float | The desired page width in inches. |
| desired_page_height | float | The desired page height in inches. |
| h_alignment_type | aspose.cells.PageLayoutAlignmentType | The chart horizontal alignment type in the output page. |
| v_alignment_type | aspose.cells.PageLayoutAlignmentType | The chart vertical alignment type in the output page. |
## to_pdf(self, stream, desired_page_width, desired_page_height, h_alignment_type, v_alignment_type) {#io.RawIOBase-float-float-aspose.cells.PageLayoutAlignmentType-aspose.cells.PageLayoutAlignmentType}
Creates the chart pdf and saves it to a stream.
```python
def to_pdf(self, stream, desired_page_width, desired_page_height, h_alignment_type, v_alignment_type):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| stream | io.RawIOBase | The output stream. |
| desired_page_width | float | The desired page width in inches. |
| desired_page_height | float | The desired page height in inches. |
| h_alignment_type | aspose.cells.PageLayoutAlignmentType | The chart horizontal alignment type in the output page. |
| v_alignment_type | aspose.cells.PageLayoutAlignmentType | The chart vertical alignment type in the output page. |
### See Also
* module [`aspose.cells.charts`](../../)
* class [`Chart`](/cells/python-net/aspose.cells.charts/chart)
