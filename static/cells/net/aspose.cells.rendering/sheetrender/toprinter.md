##SheetRender.ToPrinter
SheetRender method. Render worksheet to Printer
## ToPrinter(string) {#toprinter_2}
Render worksheet to Printer
```csharp
public void ToPrinter(string printerName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| printerName | String | the name of the printer , for example: "Microsoft Office Document Image Writer" |
### See Also
* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
## ToPrinter(string, string) {#toprinter_4}
Render worksheet to Printer
```csharp
public void ToPrinter(string printerName, string jobName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| printerName | String | the name of the printer , for example: "Microsoft Office Document Image Writer" |
| jobName | String | set the print job name |
### See Also
* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
## ToPrinter(PrinterSettings) {#toprinter}
Render worksheet to Printer
```csharp
public void ToPrinter(PrinterSettings printerSettings)
```
| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | PrinterSettings | the settings of printer, e.g. PrinterName, Duplex |
### See Also
* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
## ToPrinter(PrinterSettings, string) {#toprinter_1}
Render worksheet to Printer
```csharp
public void ToPrinter(PrinterSettings printerSettings, string jobName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | PrinterSettings | the settings of printer, e.g. PrinterName, Duplex |
| jobName | String | set the print job name |
### See Also
* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
## ToPrinter(string, int, int) {#toprinter_3}
Render worksheet to Printer
```csharp
[Obsolete("Use ToPrinter(string PrinterName) and ImageOrPrintOptions.PageIndex, PageCount instead.")]
public void ToPrinter(string printerName, int printPageIndex, int printPageCount)
```
| Parameter | Type | Description |
| --- | --- | --- |
| printerName | String | the name of the printer , for example: "Microsoft Office Document Image Writer" |
| printPageIndex | Int32 | the 0-based index of the first page to print, it must be in Range [0, SheetRender.PageCount-1] |
| printPageCount | Int32 | the number of pages to print, it must be greater than zero |
### Remarks
NOTE: This method is now obsolete. Instead, please use ToPrinter(string PrinterName) and ImageOrPrintOptions.PageIndex, PageCount to set the first page and the number of pages to print. This property will be removed 12 months later since December 2021. Aspose apologizes for any inconvenience you may have experienced.
### See Also
* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
