##FormatConditionCollection.RangeCount
FormatConditionCollection property. Gets count of conditionally formatted ranges
## FormatConditionCollection.RangeCount property
Gets count of conditionally formatted ranges.
```csharp
public int RangeCount { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FormatConditionCollectionPropertyRangeCountDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
worksheet.Cells["A4"].PutValue(40);
// Add conditional formatting
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
// Add ranges using AddArea method instead of AddRange
fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 3, EndColumn = 0 });
fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "50");
// Demonstrate RangeCount property
Console.WriteLine($"Number of ranges in FormatConditionCollection: {fcc.RangeCount}");
// Validate RangeCount
if (fcc.RangeCount < 1)
{
Console.WriteLine("Error: No ranges applied to conditional formatting");
}
else
{
Console.WriteLine("Conditional formatting ranges applied successfully");
}
}
}
}
```
### See Also
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
