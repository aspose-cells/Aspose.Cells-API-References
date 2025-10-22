##FontSettingCollection.Text
FontSettingCollection property. Gets and sets the text of the shape
## FontSettingCollection.Text property
Gets and sets the text of the shape.
```csharp
public string Text { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using System;
public class FontSettingCollectionPropertyTextDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box to the worksheet
var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
var fontSettingCollection = textBox.TextBody;
try
{
// Set initial text
fontSettingCollection.Text = "Initial Text Value";
Console.WriteLine("Initial Text value: " + fontSettingCollection.Text);
// Modify the text
fontSettingCollection.Text = "Modified Text Value";
Console.WriteLine("Modified Text value: " + fontSettingCollection.Text);
// Demonstrate appending text
fontSettingCollection.AppendText(" (Appended)");
Console.WriteLine("After AppendText: " + fontSettingCollection.Text);
// Save the workbook
workbook.Save("FontSettingCollectionTextDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
}
}
```
### See Also
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
