##PageSetup.FitToPagesWide
PageSetup property. Represents the number of pages wide the worksheet will be scaled to when its printed. The default value is 1
## PageSetup.FitToPagesWide property
Represents the number of pages wide the worksheet will be scaled to when it's printed. The default value is 1.
```csharp
public int FitToPagesWide { get; set; }
```
### Remarks
You have to set FitToPagesTall as zero if you want to fit all columns on one page.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyFitToPagesWideDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Sample Data 1");
worksheet.Cells["A2"].PutValue("Sample Data 2");
worksheet.Cells["B1"].PutValue("Sample Data 3");
worksheet.Cells["B2"].PutValue("Sample Data 4");
// Set page setup properties
worksheet.PageSetup.FitToPagesWide = 1;  // Fit to 1 page wide
worksheet.PageSetup.FitToPagesTall = 0; // Let height adjust automatically
// Save the workbook
workbook.Save("FitToPagesWideDemo.xlsx");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
