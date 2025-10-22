##FontSettingCollection.DeleteText
FontSettingCollection method. Delete some characters
## FontSettingCollection.DeleteText method
Delete some characters.
```csharp
public void DeleteText(int index, int count)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The start index. |
| count | Int32 | The count of characters. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing.Texts;
using System;
public class FontSettingCollectionMethodDeleteTextWithInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box to the worksheet
var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
var fontSettingCollection = textBox.TextBody;
// Set initial text
fontSettingCollection.Text = "This is sample text to demonstrate DeleteText method";
try
{
// Display original text
Console.WriteLine("Original text: " + fontSettingCollection.Text);
// Call DeleteText method to remove 7 characters starting at index 5
fontSettingCollection.DeleteText(5, 7);
// Display modified text
Console.WriteLine("Text after deletion: " + fontSettingCollection.Text);
// Save the workbook
workbook.Save("FontSettingCollectionDeleteTextDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing DeleteText method: {ex.Message}");
}
}
}
}
```
### See Also
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
