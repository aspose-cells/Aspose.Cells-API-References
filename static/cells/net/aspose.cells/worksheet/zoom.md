##Worksheet.Zoom
Worksheet property. Represents the scaling factor in percentage. It should be between 10 and 400
## Worksheet.Zoom property
Represents the scaling factor in percentage. It should be between 10 and 400.
```csharp
public int Zoom { get; set; }
```
### Remarks
Please set the view type first.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyZoomDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set the zoom factor to 120%
worksheet.Zoom = 120;
// Display the current zoom factor
Console.WriteLine("Current worksheet zoom: " + worksheet.Zoom + "%");
// Save the workbook
workbook.Save("WorksheetZoomDemo.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
