##WorkbookSettings.DisplayDrawingObjects
WorkbookSettings property. Indicates whether and how to show objects in the workbook
## WorkbookSettings.DisplayDrawingObjects property
Indicates whether and how to show objects in the workbook.
```csharp
public DisplayDrawingObjects DisplayDrawingObjects { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyDisplayDrawingObjectsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the workbook settings
WorkbookSettings settings = workbook.Settings;
// Add a sample shape to demonstrate the property
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
// Set to display all shapes
settings.DisplayDrawingObjects = DisplayDrawingObjects.DisplayShapes;
workbook.Save("DisplayShapes.xlsx");
// Set to show placeholders
settings.DisplayDrawingObjects = DisplayDrawingObjects.Placeholders;
workbook.Save("Placeholders.xlsx");
// Set to hide all shapes
settings.DisplayDrawingObjects = DisplayDrawingObjects.Hide;
workbook.Save("Hide.xlsx");
}
}
}
```
### See Also
* enum [DisplayDrawingObjects](../../displaydrawingobjects/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
