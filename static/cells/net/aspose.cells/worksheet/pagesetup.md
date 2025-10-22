##Worksheet.PageSetup
Worksheet property. Represents the page setup description in this sheet
## Worksheet.PageSetup property
Represents the page setup description in this sheet.
```csharp
public PageSetup PageSetup { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyPageSetupDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set page setup properties
worksheet.PageSetup.PrintArea = "A1:L50";
worksheet.PageSetup.PrintTitleRows = "1:2";
worksheet.PageSetup.PrintTitleColumns = "A:B";
worksheet.PageSetup.Orientation = PageOrientationType.Landscape;
worksheet.PageSetup.PaperSize = PaperSizeType.PaperA4;
// Add some sample data
worksheet.Cells["A1"].PutValue("Sample Data");
for (int i = 1; i <= 10; i++)
{
worksheet.Cells["A" + (i + 1)].PutValue("Item " + i);
worksheet.Cells["B" + (i + 1)].PutValue(i * 100);
}
// Save the workbook
workbook.Save("PageSetupDemo.xlsx");
Console.WriteLine("Worksheet page setup demo completed successfully.");
}
}
}
```
### See Also
* class [PageSetup](../../pagesetup/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
