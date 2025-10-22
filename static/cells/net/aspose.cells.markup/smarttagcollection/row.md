##SmartTagCollection.Row
SmartTagCollection property. Gets the row of the cell smart tags
## SmartTagCollection.Row property
Gets the row of the cell smart tags.
```csharp
public int Row { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Markup;
using System;
public class SmartTagCollectionPropertyRowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a smart tag to cell A1 (row 0, column 0)
worksheet.Cells["A1"].PutValue("Sample with SmartTag");
int index = worksheet.SmartTagSetting.Add("A1");
// Get the SmartTagCollection for cell A1
SmartTagCollection smartTags = worksheet.SmartTagSetting[index];
// Display the row of the cell containing these smart tags
Console.WriteLine("SmartTags are located at row: " + smartTags.Row);
// Note: Row property is read-only, so we cannot set it
// smartTags.Row = 5; // This would cause a compilation error
// Add another smart tag to cell B3 (row 2, column 1) to demonstrate different row
worksheet.Cells["B3"].PutValue("Another SmartTag");
int index2 = worksheet.SmartTagSetting.Add("B3");
SmartTagCollection smartTags2 = worksheet.SmartTagSetting[index2];
Console.WriteLine("Second SmartTags are located at row: " + smartTags2.Row);
// Save the workbook
workbook.Save("SmartTagRowDemo.xlsx");
}
}
}
```
### See Also
* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)
