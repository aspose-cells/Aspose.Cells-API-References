##PageSetup.ClearHeaderFooter
PageSetup method. Clears header and footer setting
## PageSetup.ClearHeaderFooter method
Clears header and footer setting.
```csharp
public void ClearHeaderFooter()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupMethodClearHeaderFooterDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
PageSetup pageSetup = worksheet.PageSetup;
// Set initial headers and footers
pageSetup.SetHeader(0, "Initial Left Header");
pageSetup.SetFooter(0, "Initial Left Footer");
Console.WriteLine("Before ClearHeaderFooter:");
Console.WriteLine("Header: " + pageSetup.GetHeader(0));
Console.WriteLine("Footer: " + pageSetup.GetFooter(0));
// Clear headers and footers
pageSetup.ClearHeaderFooter();
Console.WriteLine("\nAfter ClearHeaderFooter:");
Console.WriteLine("Header: " + (string.IsNullOrEmpty(pageSetup.GetHeader(0)) ? "Cleared" : "Not Cleared"));
Console.WriteLine("Footer: " + (string.IsNullOrEmpty(pageSetup.GetFooter(0)) ? "Cleared" : "Not Cleared"));
// Set new headers and footers after clearing
pageSetup.SetHeader(0, "New Left Header");
pageSetup.SetFooter(0, "New Left Footer");
Console.WriteLine("\nAfter Setting New Values:");
Console.WriteLine("Header: " + pageSetup.GetHeader(0));
Console.WriteLine("Footer: " + pageSetup.GetFooter(0));
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
