##Enum TxtValueQuoteType
Aspose.Cells.TxtValueQuoteType enum. Specifies the type of using quotation marks for values in text format files
## TxtValueQuoteType enumeration
Specifies the type of using quotation marks for values in text format files.
```csharp
public enum TxtValueQuoteType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Normal | `0` | All values that contain special characters such as quotation mark, separator character will be quoted. Same with the behavior of ms excel for exporting text file. |
| Always | `1` | All values will be quoted always. |
| Minimum | `2` | Only quote values when needed. Such as, if one value contains quotation mark but the quotation mark is not at the begin of this value, this value will not be quoted. |
| Never | `3` | All values will not be quoted. The exported text file with this type may not be read back correctly because the needed quotation marks being absent. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class TxtValueQuoteTypeDemo
{
public static void TxtValueQuoteTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to the worksheet
worksheet.Cells[0, 0].Value = "Name";
worksheet.Cells[0, 1].Value = "Age";
worksheet.Cells[1, 0].Value = "John Doe";
worksheet.Cells[1, 1].Value = 30;
worksheet.Cells[2, 0].Value = "Jane Smith";
worksheet.Cells[2, 1].Value = 25;
// Create TxtSaveOptions and set the QuoteType
TxtSaveOptions saveOptions = new TxtSaveOptions();
saveOptions.QuoteType = TxtValueQuoteType.Always;
// Save the workbook as a text file with the specified quote type
workbook.Save("TxtValueQuoteTypeExample.txt", saveOptions);
Console.WriteLine("Workbook saved with TxtValueQuoteType.Always");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
