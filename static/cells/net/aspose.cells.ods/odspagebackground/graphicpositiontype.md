##OdsPageBackground.GraphicPositionType
OdsPageBackground property. Gets and set the background graphic position
## OdsPageBackground.GraphicPositionType property
Gets and set the background graphic position.
```csharp
public OdsPageBackgroundGraphicPositionType GraphicPositionType { get; set; }
```
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Ods;
namespace AsposeCellsExamples
{
public class OdsPageBackgroundPropertyGraphicPositionTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
PageSetup pageSetup = sheet.PageSetup;
OdsPageBackground background = pageSetup.ODSPageBackground;
background.Type = OdsPageBackgroundType.Graphic;
background.GraphicType = OdsPageBackgroundGraphicType.Tile;
background.GraphicPositionType = OdsPageBackgroundGraphicPositionType.CenterCenter;
background.LinkedGraphic = "sample/image.png";
workbook.Save("OdsPageBackgroundGraphicPositionDemo.ods");
}
}
}
```
### See Also
* enum [OdsPageBackgroundGraphicPositionType](../../odspagebackgroundgraphicpositiontype/)
* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)
