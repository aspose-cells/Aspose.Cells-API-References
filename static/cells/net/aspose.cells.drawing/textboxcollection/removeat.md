##TextBoxCollection.RemoveAt
TextBoxCollection method. Remove a text box from the file
## TextBoxCollection.RemoveAt method
Remove a text box from the file.
```csharp
public void RemoveAt(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The text box index. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TextBoxCollectionMethodRemoveAtWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some text boxes to the worksheet
for (int i = 0; i < 3; i++)
{
worksheet.TextBoxes.Add(10, 10 + (i * 30), 200, 50);
worksheet.TextBoxes[i].Text = "TextBox " + (i + 1);
}
Console.WriteLine("Before removal - TextBox count: " + worksheet.TextBoxes.Count);
// Remove the last text box using RemoveAt with Int32 parameter
int lastIndex = worksheet.TextBoxes.Count - 1;
worksheet.TextBoxes.RemoveAt(lastIndex);
Console.WriteLine("After removal - TextBox count: " + worksheet.TextBoxes.Count);
}
}
}
```
### See Also
* class [TextBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
