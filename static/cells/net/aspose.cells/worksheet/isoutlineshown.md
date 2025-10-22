##Worksheet.IsOutlineShown
Worksheet property. Indicates whether to show outline
## Worksheet.IsOutlineShown property
Indicates whether to show outline.
```csharp
public bool IsOutlineShown { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyIsOutlineShownDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set outline to be shown
worksheet.IsOutlineShown = true;
Console.WriteLine("Outline shown: " + worksheet.IsOutlineShown);
// Save and reload to demonstrate persistence
string filePath = "IsOutlineShownDemo.xlsx";
workbook.Save(filePath);
Workbook loadedWorkbook = new Workbook(filePath);
Console.WriteLine("Reloaded - Outline shown: " + loadedWorkbook.Worksheets[0].IsOutlineShown);
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
