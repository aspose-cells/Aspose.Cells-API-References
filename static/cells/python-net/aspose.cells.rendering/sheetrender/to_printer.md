##to_printer method
## to_printer(self, printer_name) {#System.String}
Render worksheet to Printer
```python
def to_printer(self, printer_name):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| printer_name | System.String | the name of the printer , for example: "Microsoft Office Document Image Writer" |
## to_printer(self, printer_settings) {#aspose.pydrawing.printing.PrinterSettings}
Render worksheet to Printer
```python
def to_printer(self, printer_settings):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| printer_settings | aspose.pydrawing.printing.PrinterSettings | the settings of printer, e.g. PrinterName, Duplex |
## to_printer(self, printer_name, job_name) {#System.String-System.String}
Render worksheet to Printer
```python
def to_printer(self, printer_name, job_name):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| printer_name | System.String | the name of the printer , for example: "Microsoft Office Document Image Writer" |
| job_name | System.String | set the print job name |
## to_printer(self, printer_settings, job_name) {#aspose.pydrawing.printing.PrinterSettings-System.String}
Render worksheet to Printer
```python
def to_printer(self, printer_settings, job_name):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| printer_settings | aspose.pydrawing.printing.PrinterSettings | the settings of printer, e.g. PrinterName, Duplex |
| job_name | System.String | set the print job name |
## to_printer(self, printer_name, print_page_index, print_page_count) {#System.String-int-int}
Render worksheet to Printer
```python
def to_printer(self, printer_name, print_page_index, print_page_count):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| printer_name | System.String | the name of the printer , for example: "Microsoft Office Document Image Writer" |
| print_page_index | int | the 0-based index of the first page to print, it must be in Range [0, SheetRender.PageCount-1] |
| print_page_count | int | the number of pages to print, it must be greater than zero |
### Remarks
NOTE: This method is now obsolete.
Instead, please use ToPrinter(string PrinterName) and ImageOrPrintOptions.PageIndex, PageCount to set the first page and the number of pages to print.
This property will be removed 12 months later since December 2021.
Aspose apologizes for any inconvenience you may have experienced.
### See Also
* module [`aspose.cells.rendering`](../../)
* class [`SheetRender`](/cells/python-net/aspose.cells.rendering/sheetrender)
