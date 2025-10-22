##Enum DisplayDrawingObjects
Aspose.Cells.DisplayDrawingObjects enum. Represents whether and how to show objects in the workbook
## DisplayDrawingObjects enumeration
Represents whether and how to show objects in the workbook.
```csharp
public enum DisplayDrawingObjects
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| DisplayShapes | `0` | Show all objects |
| Placeholders | `1` | Show placeholders |
| Hide | `2` | Hide all shapes. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class DisplayDrawingObjectsDemo
{
public static void DisplayDrawingObjectsExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the workbook settings
WorkbookSettings settings = workbook.Settings;
// Set the DisplayDrawingObjects property to show all objects
settings.DisplayDrawingObjects = DisplayDrawingObjects.DisplayShapes;
// Save the workbook
workbook.Save("DisplayDrawingObjectsExample_DisplayShapes.xlsx");
// Set the DisplayDrawingObjects property to show placeholders
settings.DisplayDrawingObjects = DisplayDrawingObjects.Placeholders;
// Save the workbook
workbook.Save("DisplayDrawingObjectsExample_Placeholders.xlsx");
// Set the DisplayDrawingObjects property to hide all shapes
settings.DisplayDrawingObjects = DisplayDrawingObjects.Hide;
// Save the workbook
workbook.Save("DisplayDrawingObjectsExample_Hide.xlsx");
workbook.Save("DisplayDrawingObjectsExample_Hide.pdf");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
