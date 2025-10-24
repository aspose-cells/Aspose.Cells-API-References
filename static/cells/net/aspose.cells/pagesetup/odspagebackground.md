##PageSetup.ODSPageBackground
PageSetup property. Gets the background of ODS
## PageSetup.ODSPageBackground property
Gets the background of ODS.
```csharp
public OdsPageBackground ODSPageBackground { get; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Ods;
namespace AsposeCellsExamples
{
public class PageSetupPropertyODSPageBackgroundDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
OdsPageBackground background = sheet.PageSetup.ODSPageBackground;
// Set color background
background.Type = OdsPageBackgroundType.Color;
background.Color = Color.LightGreen;
// Alternatively, set graphic background
background.Type = OdsPageBackgroundType.Graphic;
background.GraphicType = OdsPageBackgroundGraphicType.Tile;
background.GraphicPositionType = OdsPageBackgroundGraphicPositionType.TopLeft;
workbook.Save("ODSPageBackgroundDemo.ods");
}
}
}
```
### See Also
* class [OdsPageBackground](../../../aspose.cells.ods/odspagebackground/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
