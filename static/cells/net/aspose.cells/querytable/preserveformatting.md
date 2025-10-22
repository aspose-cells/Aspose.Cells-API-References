##QueryTable.PreserveFormatting
QueryTable property. Returns or sets the PreserveFormatting of the object
## QueryTable.PreserveFormatting property
Returns or sets the PreserveFormatting of the object.
```csharp
public bool PreserveFormatting { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class QueryTablePropertyPreserveFormattingDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data and formatting
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Price");
worksheet.Cells["A2"].PutValue("Laptop");
worksheet.Cells["B2"].PutValue(1200);
worksheet.Cells["A3"].PutValue("Phone");
worksheet.Cells["B3"].PutValue(800);
// Apply formatting to the data range
Style style = workbook.CreateStyle();
style.Font.IsBold = true;
style.ForegroundColor = System.Drawing.Color.LightBlue;
style.Pattern = BackgroundType.Solid;
// Apply style to each cell in the range
worksheet.Cells["A1"].SetStyle(style);
worksheet.Cells["B1"].SetStyle(style);
// Create a query table (simulated since actual creation requires external data source)
// In real usage, you would create this from an external connection
QueryTable queryTable = worksheet.QueryTables[0];
// Display current PreserveFormatting value
Console.WriteLine("Initial PreserveFormatting value: " + queryTable.PreserveFormatting);
// Set PreserveFormatting to false (won't preserve existing formatting during refresh)
queryTable.PreserveFormatting = false;
Console.WriteLine("PreserveFormatting set to: " + queryTable.PreserveFormatting);
// Simulate refreshing the query table (would normally clear formatting when PreserveFormatting is false)
// In a real scenario, this would happen when the query table refreshes its data
Console.WriteLine("After refresh with PreserveFormatting=false, formatting would be lost");
// Set PreserveFormatting back to true
queryTable.PreserveFormatting = true;
Console.WriteLine("PreserveFormatting set to: " + queryTable.PreserveFormatting);
// Simulate refreshing again (would now preserve formatting)
Console.WriteLine("After refresh with PreserveFormatting=true, formatting is preserved");
// Save the workbook
workbook.Save("QueryTablePreserveFormattingDemo.xlsx");
}
}
}
```
### See Also
* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
