##FontSettingCollection.InsertText
FontSettingCollection method. Insert index at the position
## FontSettingCollection.InsertText method
Insert index at the position.
```csharp
public void InsertText(int index, string text)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The start index. |
| text | String | The text. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing.Texts;
using System;
public class FontSettingCollectionMethodInsertTextWithInt32StringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box to the worksheet
var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 100, 100);
var fontSettingCollection = textBox.TextBody;
// Set initial text
fontSettingCollection.Text = "Initial Text";
try
{
// Call InsertText method to insert text at index 7
fontSettingCollection.InsertText(7, " Inserted");
// Display the modified text
Console.WriteLine("Text after insertion: " + fontSettingCollection.Text);
// Save the workbook
workbook.Save("FontSettingCollectionInsertTextDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing InsertText method: {ex.Message}");
}
}
}
}
```
### See Also
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
