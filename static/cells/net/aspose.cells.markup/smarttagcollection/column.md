##SmartTagCollection.Column
SmartTagCollection property. Gets the column of the cell smart tags
## SmartTagCollection.Column property
Gets the column of the cell smart tags.
```csharp
public int Column { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Markup;
using System;
public class SmartTagCollectionPropertyColumnDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a smart tag to cell C5 (row 4, column 2)
worksheet.Cells["C5"].PutValue("SmartTag Demo");
int index = worksheet.SmartTagSetting.Add("C5");
// Get the SmartTagCollection for cell C5
SmartTagCollection smartTags = worksheet.SmartTagSetting[index];
// Display the column of the cell containing these smart tags
Console.WriteLine("SmartTags are located at column: " + smartTags.Column);
// Add another smart tag to cell E2 (row 1, column 4) to demonstrate different column
worksheet.Cells["E2"].PutValue("Another SmartTag");
int index2 = worksheet.SmartTagSetting.Add("E2");
SmartTagCollection smartTags2 = worksheet.SmartTagSetting[index2];
Console.WriteLine("Second SmartTags are located at column: " + smartTags2.Column);
// Save the workbook
workbook.Save("SmartTagColumnDemo.xlsx");
}
}
}
```
### See Also
* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)
