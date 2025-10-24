##ShapeCollection.AddSpinner
ShapeCollection method. Adds a Spinner to the worksheet
## ShapeCollection.AddSpinner method
Adds a Spinner to the worksheet.
```csharp
public Spinner AddSpinner(int upperLeftRow, int top, int upperLeftColumn, int left, int height,
int width)
```
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of Spinner from its left row, in unit of pixel. |
| upperLeftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of Spinner from its left column, in unit of pixel. |
| height | Int32 | Represents the height of Spinner, in unit of pixel. |
| width | Int32 | Represents the width of Spinner, in unit of pixel. |
### Return Value
A Spinner object.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeCollectionMethodAddSpinnerWithInt32Int32Int32Int32Int32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a spinner to the worksheet
Aspose.Cells.Drawing.Spinner spinner = (Aspose.Cells.Drawing.Spinner)worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 50);
// Set spinner properties
spinner.LinkedCell = "A1";
spinner.Min = 0;
spinner.Max = 100;
spinner.IncrementalChange = 1;
// Save the workbook
workbook.Save("AddSpinnerDemo.xlsx");
}
}
}
```
### See Also
* class [Spinner](../../spinner/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
