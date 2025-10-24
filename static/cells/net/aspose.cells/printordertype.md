##Enum PrintOrderType
Aspose.Cells.PrintOrderType enum. Represent print order constants
## PrintOrderType enumeration
Represent print order constants.
```csharp
public enum PrintOrderType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| DownThenOver | `0` | Down, then over |
| OverThenDown | `1` | Over, then down |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class PrintOrderTypeDemo
{
public static void PrintOrderTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access the PageSetup object
PageSetup pageSetup = worksheet.PageSetup;
// Set the print order to DownThenOver
pageSetup.Order = PrintOrderType.DownThenOver;
// Set some other page setup properties for demonstration
pageSetup.PrintArea = "A1:D10";
pageSetup.PrintTitleRows = "$1:$1";
pageSetup.PrintTitleColumns = "$A:$A";
pageSetup.CenterHorizontally = true;
pageSetup.CenterVertically = true;
// Save the workbook
workbook.Save("PrintOrderTypeExample.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
