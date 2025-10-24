##Enum PrintErrorsType
Aspose.Cells.PrintErrorsType enum. Represents print errors constants
## PrintErrorsType enumeration
Represents print errors constants.
```csharp
public enum PrintErrorsType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| PrintErrorsBlank | `0` | Represents not to print errors. |
| PrintErrorsDash | `1` | Represents to print errors as "--". |
| PrintErrorsDisplayed | `2` | Represents to print errors as displayed. |
| PrintErrorsNA | `3` | Represents to print errors as "#N/A". |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class PrintErrorsTypeDemo
{
public static void PrintErrorsTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access the PageSetup of the worksheet
PageSetup pageSetup = worksheet.PageSetup;
// Set different print error types
pageSetup.PrintErrors = PrintErrorsType.PrintErrorsBlank;
workbook.Save("PrintErrorsBlank.xlsx");
pageSetup.PrintErrors = PrintErrorsType.PrintErrorsDash;
workbook.Save("PrintErrorsDash.xlsx");
pageSetup.PrintErrors = PrintErrorsType.PrintErrorsDisplayed;
workbook.Save("PrintErrorsDisplayed.xlsx");
pageSetup.PrintErrors = PrintErrorsType.PrintErrorsNA;
workbook.Save("PrintErrorsNA.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
