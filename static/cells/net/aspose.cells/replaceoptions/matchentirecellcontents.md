##ReplaceOptions.MatchEntireCellContents
ReplaceOptions property. Indicates whether to match entire cells contents
## ReplaceOptions.MatchEntireCellContents property
Indicates whether to match entire cells contents
```csharp
public bool MatchEntireCellContents { get; set; }
```
### Remarks
The default value is true.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ReplaceOptionsPropertyMatchEntireCellContentsDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set sample cell values
worksheet.Cells["A1"].PutValue("apple");
worksheet.Cells["A2"].PutValue("apple pie");
worksheet.Cells["A3"].PutValue("an apple");
worksheet.Cells["A4"].PutValue("apples");
// Replace with MatchEntireCellContents = true (exact match only)
ReplaceOptions options1 = new ReplaceOptions();
options1.MatchEntireCellContents = true;
workbook.Replace("apple", "orange", options1);
// Replace with MatchEntireCellContents = false (partial match)
ReplaceOptions options2 = new ReplaceOptions();
options2.MatchEntireCellContents = false;
workbook.Replace("apple", "banana", options2);
// Output results
Console.WriteLine("A1: " + worksheet.Cells["A1"].StringValue); // orange (exact match)
Console.WriteLine("A2: " + worksheet.Cells["A2"].StringValue); // banana pie (partial match)
Console.WriteLine("A3: " + worksheet.Cells["A3"].StringValue); // an banana (partial match)
Console.WriteLine("A4: " + worksheet.Cells["A4"].StringValue); // bananas (partial match)
}
}
}
```
### See Also
* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
