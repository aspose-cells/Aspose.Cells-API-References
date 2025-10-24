##process method
## process(, options) {#aspose.cells.lowcode.LowCodeSplitOptions}
Splits spreadsheet file into multiple parts.
```python
@staticmethod
def process(options):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| options | aspose.cells.lowcode.LowCodeSplitOptions | Options for splitting spreadsheet |
## process(, template_file, result_file) {#System.String-System.String}
Splits given template file into multiple parts.
```python
@staticmethod
def process(template_file, result_file):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| template_file | System.String | The template file to be split |
| result_file | System.String | The resultant file(name pattern) |
### Remarks
The output files will be build from the specified resultant file by
appending sequence number of the sheet and split part.
For example, if the specified output file is Split.xlsx, then the generated
files will be Split_0_0.xlsx, Split_0_1.xlsx, ..., Split_1_0.xlsx, ...
### See Also
* module [`aspose.cells.lowcode`](../../)
* class [`SpreadsheetSplitter`](/cells/python-net/aspose.cells.lowcode/spreadsheetsplitter)
