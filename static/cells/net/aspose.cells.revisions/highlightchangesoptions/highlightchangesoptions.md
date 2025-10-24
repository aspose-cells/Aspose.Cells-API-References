##HighlightChangesOptions.HighlightChangesOptions
HighlightChangesOptions constructor. Represents options of highlighting revsions or changes of shared Excel files
## HighlightChangesOptions constructor
Represents options of highlighting revsions or changes of shared Excel files.
```csharp
public HighlightChangesOptions(bool highlightOnScreen, bool listOnNewSheet)
```
| Parameter | Type | Description |
| --- | --- | --- |
| highlightOnScreen | Boolean | Indicates whether highlighting changes on screen. |
| listOnNewSheet | Boolean | Indicates whether listing changes on a new worksheet. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;
namespace AsposeCellsExamples
{
public class HighlightChangesOptionsMethodCtorWithBooleanBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add some sample data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Original Value");
worksheet.Cells["A2"].PutValue(100);
// Create HighlightChangesOptions with boolean parameters
HighlightChangesOptions options = new HighlightChangesOptions(true, true);
// Simulate tracking changes (normally you'd have actual revisions)
Console.WriteLine("HighlightChangesOptions created with:");
Console.WriteLine($"First parameter (show changes): {true}");
Console.WriteLine($"Second parameter (changes on new sheet): {true}");
// Save the workbook
workbook.Save("HighlightChangesDemo.xlsx");
}
}
}
```
### See Also
* class [HighlightChangesOptions](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
