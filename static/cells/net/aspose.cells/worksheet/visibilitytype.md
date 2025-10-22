##Worksheet.VisibilityType
Worksheet property. Indicates the visible state for this sheet
## Worksheet.VisibilityType property
Indicates the visible state for this sheet.
```csharp
public VisibilityType VisibilityType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyVisibilityTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add worksheets
workbook.Worksheets.Add();
workbook.Worksheets.Add();
// Set different visibility types for each worksheet
workbook.Worksheets[0].VisibilityType = VisibilityType.Hidden;
workbook.Worksheets[1].VisibilityType = VisibilityType.VeryHidden;
workbook.Worksheets[2].VisibilityType = VisibilityType.Visible;
// Save the workbook
string outputPath = "output_visibility.xlsx";
workbook.Save(outputPath);
// Reload the workbook to verify visibility settings
Workbook loadedWorkbook = new Workbook(outputPath);
// Output visibility types
Console.WriteLine("Worksheet 0 Visibility: " + loadedWorkbook.Worksheets[0].VisibilityType);
Console.WriteLine("Worksheet 1 Visibility: " + loadedWorkbook.Worksheets[1].VisibilityType);
Console.WriteLine("Worksheet 2 Visibility: " + loadedWorkbook.Worksheets[2].VisibilityType);
}
}
}
```
### See Also
* enum [VisibilityType](../../visibilitytype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
