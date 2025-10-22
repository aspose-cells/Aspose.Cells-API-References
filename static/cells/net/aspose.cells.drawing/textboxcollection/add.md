##TextBoxCollection.Add
TextBoxCollection method. Adds a textbox to the collection
## TextBoxCollection.Add method
Adds a textbox to the collection.
```csharp
public int Add(int upperLeftRow, int upperLeftColumn, int height, int width)
```
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| upperLeftColumn | Int32 | Upper left column index. |
| height | Int32 | Height of textbox, in unit of pixel. |
| width | Int32 | Width of textbox, in unit of pixel. |
### Return Value
[`TextBox`](../../textbox/) object index.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TextBoxCollectionMethodAddWithInt32Int32Int32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
int index = worksheet.TextBoxes.Add(1, 1, 50, 100);
Console.WriteLine("TextBox added at index: " + index);
}
}
}
```
### See Also
* class [TextBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
