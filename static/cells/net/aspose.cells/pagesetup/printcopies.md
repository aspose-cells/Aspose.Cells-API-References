##PageSetup.PrintCopies
PageSetup property. Get and sets number of copies to print
## PageSetup.PrintCopies property
Get and sets number of copies to print.
```csharp
public int PrintCopies { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyPrintCopiesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set the number of print copies to 3
worksheet.PageSetup.PrintCopies = 3;
// Display the current print copies setting
Console.WriteLine("Print Copies: " + worksheet.PageSetup.PrintCopies);
// Save the workbook
workbook.Save("PageSetup_PrintCopies_Output.xlsx");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
