##Worksheet.RemoveAllDrawingObjects
Worksheet method. Removes all drawing objects in this worksheet
## Worksheet.RemoveAllDrawingObjects method
Removes all drawing objects in this worksheet.
```csharp
public void RemoveAllDrawingObjects()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodRemoveAllDrawingObjectsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add some drawing objects to the worksheet
worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 50);
worksheet.Shapes.AddLine(1, 0, 5, 100, 5, 150);
// Save before removing objects
workbook.Save("BeforeRemove.xlsx", SaveFormat.Xlsx);
// Remove all drawing objects
worksheet.RemoveAllDrawingObjects();
// Save after removing objects
workbook.Save("AfterRemove.xlsx", SaveFormat.Xlsx);
// Dispose the workbook
workbook.Dispose();
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
