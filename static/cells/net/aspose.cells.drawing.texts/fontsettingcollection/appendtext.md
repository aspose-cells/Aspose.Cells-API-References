##FontSettingCollection.AppendText
FontSettingCollection method. Appends the text
## FontSettingCollection.AppendText method
Appends the text.
```csharp
public void AppendText(string text)
```
| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The text. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing.Texts;
using System;
public class FontSettingCollectionMethodAppendTextWithStringDemo
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
fontSettingCollection.Text = "Hello, ";
try
{
// Call AppendText method to append additional text
fontSettingCollection.AppendText("World!");
// Display the modified text
Console.WriteLine("Text after append: " + fontSettingCollection.Text);
// Save the workbook
workbook.Save("FontSettingCollectionAppendTextDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing AppendText method: {ex.Message}");
}
}
}
}
```
### See Also
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
