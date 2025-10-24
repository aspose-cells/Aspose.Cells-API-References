##PageSetup.PrintErrors
PageSetup property. Specifies the type of print error displayed
## PageSetup.PrintErrors property
Specifies the type of print error displayed.
```csharp
public PrintErrorsType PrintErrors { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyPrintErrorsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet sheet = workbook.Worksheets[0];
// Set print errors to display as blank
sheet.PageSetup.PrintErrors = PrintErrorsType.PrintErrorsBlank;
Console.WriteLine("PrintErrors set to: " + sheet.PageSetup.PrintErrors);
// Change print errors to display as dashes
sheet.PageSetup.PrintErrors = PrintErrorsType.PrintErrorsDash;
Console.WriteLine("PrintErrors changed to: " + sheet.PageSetup.PrintErrors);
// Save the workbook
workbook.Save("PrintErrorsDemo.xlsx");
}
}
}
```
### See Also
* enum [PrintErrorsType](../../printerrorstype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
