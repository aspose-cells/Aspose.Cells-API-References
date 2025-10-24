##OdsPageBackground.GraphicType
OdsPageBackground property. Gets and sets the page background graphic type
## OdsPageBackground.GraphicType property
Gets and sets the page background graphic type.
```csharp
public OdsPageBackgroundGraphicType GraphicType { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Ods;
namespace AsposeCellsExamples
{
public class OdsPageBackgroundPropertyGraphicTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
PageSetup pageSetup = sheet.PageSetup;
OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;
odsPageBackground.Type = OdsPageBackgroundType.Graphic;
odsPageBackground.GraphicType = OdsPageBackgroundGraphicType.Tile;
odsPageBackground.LinkedGraphic = "background.png";
workbook.Save("OdsPageBackgroundGraphicTypeDemo.ods");
}
}
}
```
### See Also
* enum [OdsPageBackgroundGraphicType](../../odspagebackgroundgraphictype/)
* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)
