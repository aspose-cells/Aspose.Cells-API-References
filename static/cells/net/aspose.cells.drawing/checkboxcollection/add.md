##CheckBoxCollection.Add
CheckBoxCollection method. Adds a checkBox to the collection
## CheckBoxCollection.Add method
Adds a checkBox to the collection.
```csharp
public int Add(int upperLeftRow, int upperLeftColumn, int height, int width)
```
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| upperLeftColumn | Int32 | Upper left column index. |
| height | Int32 | Height of checkBox, in unit of pixel. |
| width | Int32 | Width of checkBox, in unit of pixel. |
### Return Value
[`CheckBox`](../../checkbox/) object index.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class CheckBoxCollectionMethodAddWithInt32Int32Int32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add checkbox using Int32 parameters (upperLeftRow, upperLeftColumn, height, width)
int index = worksheet.CheckBoxes.Add(10, 2, 20, 100);
CheckBox checkBox = worksheet.CheckBoxes[index];
checkBox.Text = "Sample CheckBox";
checkBox.Value = true;
checkBox.LinkedCell = "B11";
workbook.Save("CheckBoxDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [CheckBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
