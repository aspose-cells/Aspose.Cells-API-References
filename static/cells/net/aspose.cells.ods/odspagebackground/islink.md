##OdsPageBackground.IsLink
OdsPageBackground property. Indicates whether its a linked graphic
## OdsPageBackground.IsLink property
Indicates whether it's a linked graphic.
```csharp
public bool IsLink { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Ods;
using System;
public class OdsPageBackgroundPropertyIsLinkDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook(FileFormatType.Ods);
Worksheet worksheet = workbook.Worksheets[0];
// Access the OdsPageBackground
OdsPageBackground background = worksheet.PageSetup.ODSPageBackground;
// Display the current IsLink value
Console.WriteLine("Current IsLink value: " + background.IsLink);
// Modify the existing background properties instead of creating a new one
background.Type = OdsPageBackgroundType.Graphic;
background.GraphicType = OdsPageBackgroundGraphicType.Position;
background.GraphicPositionType = OdsPageBackgroundGraphicPositionType.TopLeft;
background.LinkedGraphic = "path/to/image.png";
// Display the new IsLink value
Console.WriteLine("New IsLink value: " + worksheet.PageSetup.ODSPageBackground.IsLink);
// Save the result
workbook.Save("OdsPageBackgroundIsLinkDemo.ods");
}
}
}
```
### See Also
* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)
