##HtmlSaveOptions.ShowAllSheets
HtmlSaveOptions property. Indicates whether showing all sheets when saving as a single html file
## HtmlSaveOptions.ShowAllSheets property
Indicates whether showing all sheets when saving as a single html file.
```csharp
public bool ShowAllSheets { get; set; }
```
### Remarks
Only works when [`SaveAsSingleFile`](../saveassinglefile/) is True.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyShowAllSheetsDemo
{
public static void Run()
{
// Create a new workbook with multiple sheets
Workbook workbook = new Workbook();
// Add data to first sheet
Worksheet sheet1 = workbook.Worksheets[0];
sheet1.Name = "FirstSheet";
sheet1.Cells["A1"].PutValue("Sheet 1 Content");
// Add second sheet
Worksheet sheet2 = workbook.Worksheets.Add("SecondSheet");
sheet2.Cells["B2"].PutValue("Sheet 2 Content");
// Add third sheet
Worksheet sheet3 = workbook.Worksheets.Add("ThirdSheet");
sheet3.Cells["C3"].PutValue("Sheet 3 Content");
// Create HTML save options
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
// Set ShowAllSheets property to true to export all sheets
saveOptions.ShowAllSheets = true;
// Save workbook with all sheets visible in HTML
workbook.Save("ShowAllSheetsDemo.html", saveOptions);
Console.WriteLine("HTML file with all sheets exported successfully.");
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
