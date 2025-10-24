##OdsPageBackground.GraphicData
OdsPageBackground property. Gets and sets the graphic data
## OdsPageBackground.GraphicData property
Gets and sets the graphic data.
```csharp
public byte[] GraphicData { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Ods;
namespace AsposeCellsExamples
{
public class OdsPageBackgroundPropertyGraphicDataDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet and its page setup
Worksheet worksheet = workbook.Worksheets[0];
PageSetup pageSetup = worksheet.PageSetup;
// Set ODS page background properties
OdsPageBackground background = pageSetup.ODSPageBackground;
background.Type = OdsPageBackgroundType.Graphic;
// Load image data and set as background
string imagePath = "sample.png"; // Replace with actual image path
if (File.Exists(imagePath))
{
background.GraphicData = File.ReadAllBytes(imagePath);
background.GraphicType = OdsPageBackgroundGraphicType.Area;
// Save the workbook
workbook.Save("output.ods");
Console.WriteLine("ODS file with graphic background created successfully.");
}
else
{
Console.WriteLine("Image file not found: " + imagePath);
}
}
}
}
```
### See Also
* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)
