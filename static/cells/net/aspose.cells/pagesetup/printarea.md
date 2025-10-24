##PageSetup.PrintArea
PageSetup property. Represents the range to be printed
## PageSetup.PrintArea property
Represents the range to be printed.
```csharp
public string PrintArea { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyPrintAreaDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("Item1");
worksheet.Cells["B2"].PutValue(2);
worksheet.Cells["A3"].PutValue("Item2");
worksheet.Cells["B3"].PutValue(3);
// Set print area to A1:B3
worksheet.PageSetup.PrintArea = "A1:B3";
// Save with print area only
HtmlSaveOptions options = new HtmlSaveOptions
{
ExportPrintAreaOnly = true
};
workbook.Save("PrintAreaDemo.html", options);
Console.WriteLine("Print area demo created successfully.");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
