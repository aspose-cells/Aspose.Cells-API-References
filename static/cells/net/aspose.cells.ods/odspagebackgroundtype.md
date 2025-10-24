##Enum OdsPageBackgroundType
Aspose.Cells.Ods.OdsPageBackgroundType enum. Represents the page background type of ods
## OdsPageBackgroundType enumeration
Represents the page background type of ods.
```csharp
public enum OdsPageBackgroundType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | No background. |
| Color | `1` | Formats the background with color. |
| Graphic | `2` | Formats the background with image. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Ods;
using System;
using System.Drawing;
public class OdsPageBackgroundTypeDemo
{
public static void OdsPageBackgroundTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Access the PageSetup of the worksheet
PageSetup pageSetup = worksheet.PageSetup;
// Access the ODSPageBackground property
OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;
// Set the background type to Color
odsPageBackground.Type = OdsPageBackgroundType.Color;
// Set the background color
odsPageBackground.Color = Color.LightBlue;
// Save the workbook
workbook.Save("OdsPageBackgroundTypeExample.ods");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)
