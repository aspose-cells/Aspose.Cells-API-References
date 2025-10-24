##OdsPageBackground.Type
OdsPageBackground property. Gets and sets the page background type
## OdsPageBackground.Type property
Gets and sets the page background type.
```csharp
public OdsPageBackgroundType Type { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Ods;
namespace AsposeCellsExamples
{
public class OdsPageBackgroundPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet's page setup
PageSetup ps = workbook.Worksheets[0].PageSetup;
// Get the ODS page background
OdsPageBackground background = ps.ODSPageBackground;
// Set background type to graphic and configure it
background.Type = OdsPageBackgroundType.Graphic;
background.GraphicData = File.ReadAllBytes("image1.png");
background.GraphicType = OdsPageBackgroundGraphicType.Area;
// Save the workbook
workbook.Save("output.ods");
// Reload the saved file to verify the settings
Workbook verifyWorkbook = new Workbook("output.ods");
PageSetup verifyPs = verifyWorkbook.Worksheets[0].PageSetup;
OdsPageBackground verifyBackground = verifyPs.ODSPageBackground;
// Output the verification results
Console.WriteLine("Background Type: " + verifyBackground.Type);
Console.WriteLine("Graphic Type: " + verifyBackground.GraphicType);
}
}
}
```
### See Also
* enum [OdsPageBackgroundType](../../odspagebackgroundtype/)
* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)
