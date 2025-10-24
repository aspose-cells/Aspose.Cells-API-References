##Worksheet.TabColor
Worksheet property. Represents worksheet tab color
## Worksheet.TabColor property
Represents worksheet tab color.
```csharp
public Color TabColor { get; set; }
```
### Remarks
This feature is only supported in ExcelXP(Excel2002) and later versions. If you save file as Excel97 or Excel2000 format, it will be omitted.
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyTabColorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set tab color to red
worksheet.TabColor = Color.Red;
Console.WriteLine("Tab color set to: " + worksheet.TabColor);
// Save the workbook
workbook.Save("output.xlsx");
// Clear the tab color
worksheet.TabColor = Color.Empty;
Console.WriteLine("Tab color cleared: " + worksheet.TabColor.IsEmpty);
// Save the modified workbook
workbook.Save("output_modified.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
