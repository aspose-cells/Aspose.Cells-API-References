##OdsPageBackground.LinkedGraphic
OdsPageBackground property. Gets and sets the linked graphic path
## OdsPageBackground.LinkedGraphic property
Gets and sets the linked graphic path.
```csharp
public string LinkedGraphic { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Ods;
namespace AsposeCellsExamples
{
public class OdsPageBackgroundPropertyLinkedGraphicDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
PageSetup pageSetup = worksheet.PageSetup;
OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;
odsPageBackground.Color = Color.LightBlue;
odsPageBackground.GraphicType = OdsPageBackgroundGraphicType.Tile;
odsPageBackground.LinkedGraphic = "background_image.png";
workbook.Save("OdsPageBackgroundLinkedGraphicDemo.ods");
}
}
}
```
### See Also
* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)
