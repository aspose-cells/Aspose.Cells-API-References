##Worksheet.Type
Worksheet property. Represents worksheet type
## Worksheet.Type property
Represents worksheet type.
```csharp
public SheetType Type { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set some basic properties
worksheet.Name = "DemoSheet";
worksheet.IsVisible = true;
// Demonstrate Type property usage
Console.WriteLine("Worksheet Type: " + worksheet.Type);
// Add a chart sheet to demonstrate different worksheet type
workbook.Worksheets.Add(SheetType.Chart);
Worksheet chartSheet = workbook.Worksheets[1];
// Compare worksheet types
Console.WriteLine("Regular Sheet Type: " + worksheet.Type);
Console.WriteLine("Chart Sheet Type: " + chartSheet.Type);
// Save the workbook
workbook.Save("WorksheetTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [SheetType](../../sheettype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
