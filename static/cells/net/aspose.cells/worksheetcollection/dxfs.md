##WorksheetCollection.Dxfs
WorksheetCollection property. Gets the master differential formatting records
## WorksheetCollection.Dxfs property
Gets the master differential formatting records.
```csharp
public DxfCollection Dxfs { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetCollectionPropertyDxfsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
// Add conditional formatting
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
// Set condition and style
fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "15");
Style style = workbook.CreateStyle();
style.Pattern = BackgroundType.Solid;
style.ForegroundColor = System.Drawing.Color.LightGreen;
fcc[0].Style = style;
// Demonstrate Dxfs property
Console.WriteLine("Dxfs count before applying formatting: " + workbook.Worksheets.Dxfs.Count);
// Apply formatting which will add to Dxfs
worksheet.ConditionalFormattings[0][0].Priority = 1;
Console.WriteLine("Dxfs count after applying formatting: " + workbook.Worksheets.Dxfs.Count);
}
}
}
```
### See Also
* class [DxfCollection](../../dxfcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
