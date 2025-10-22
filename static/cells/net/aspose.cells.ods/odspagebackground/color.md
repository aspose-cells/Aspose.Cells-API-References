##OdsPageBackground.Color
OdsPageBackground property. Gets and sets the color of background
## OdsPageBackground.Color property
Gets and sets the color of background.
```csharp
public Color Color { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;
using System.Drawing;
namespace AsposeCellsExamples
{
public class OdsPageBackgroundPropertyColorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
PageSetup ps = workbook.Worksheets[0].PageSetup;
OdsPageBackground b = ps.ODSPageBackground;
b.Type = OdsPageBackgroundType.Color;
b.Color = Color.Red;
workbook.Save("output.ods");
Workbook loadedWorkbook = new Workbook("output.ods");
PageSetup loadedPs = loadedWorkbook.Worksheets[0].PageSetup;
OdsPageBackground loadedB = loadedPs.ODSPageBackground;
Console.WriteLine("Background Type: " + loadedB.Type);
Console.WriteLine("Background Color: " + loadedB.Color);
}
}
}
```
### See Also
* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)
