##Worksheet.DisplayRightToLeft
Worksheet property. Indicates if the specified worksheet is displayed from right to left instead of from left to right. Default is false
## Worksheet.DisplayRightToLeft property
Indicates if the specified worksheet is displayed from right to left instead of from left to right. Default is false.
```csharp
public bool DisplayRightToLeft { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyDisplayRightToLeftDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set display right to left
worksheet.DisplayRightToLeft = true;
// Save the workbook
workbook.Save("output.ods");
// Reload the workbook to verify the setting
Workbook loadedWorkbook = new Workbook("output.ods");
Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
Console.WriteLine("DisplayRightToLeft: " + loadedWorksheet.DisplayRightToLeft);
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
