##Worksheet.GridlineColor
Worksheet property. Gets and sets the color of gridline
## Worksheet.GridlineColor property
Gets and sets the color of gridline
```csharp
public Color GridlineColor { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyGridlineColorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set gridline color to red
worksheet.GridlineColor = Color.Red;
// Save the workbook
string outputPath = "GridlineColorDemo.xlsx";
workbook.Save(outputPath);
Console.WriteLine("Gridline color set to red and saved to: " + outputPath);
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
