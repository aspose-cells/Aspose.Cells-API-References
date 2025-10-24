##PageSetup.Orientation
PageSetup property. Represents page print orientation
## PageSetup.Orientation property
Represents page print orientation.
```csharp
public PageOrientationType Orientation { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyOrientationDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set page orientation to Landscape
worksheet.PageSetup.Orientation = PageOrientationType.Landscape;
// Add some sample data to demonstrate the effect
worksheet.Cells["A1"].PutValue("Landscape Orientation Demo");
for (int i = 1; i <= 10; i++)
{
worksheet.Cells[$"A{i}"].PutValue($"Data Row {i}");
}
// Save the workbook
workbook.Save("PageOrientationDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* enum [PageOrientationType](../../pageorientationtype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
