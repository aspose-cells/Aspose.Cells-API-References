##FontSettingCollection.Replace
FontSettingCollection method. Replace the text
## Replace(int, int, string) {#replace}
Replace the text.
```csharp
public void Replace(int index, int count, string text)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The start index. |
| count | Int32 | The count of characters. |
| text | String | The text. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing.Texts;
using System;
public class FontSettingCollectionMethodReplaceWithInt32Int32StringDemo
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
fontSettingCollection.Text = "Original text to be modified";
try
{
// Call Replace method to replace 8 characters starting at index 9 with new text
fontSettingCollection.Replace(9, 8, "replaced");
// Display the modified text
Console.WriteLine("Text after replacement: " + fontSettingCollection.Text);
// Save the workbook
workbook.Save("FontSettingCollectionReplaceDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Replace method: {ex.Message}");
}
}
}
}
```
### See Also
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
## Replace(string, string) {#replace_1}
Replace the text.
```csharp
public void Replace(string oldValue, string newValue)
```
| Parameter | Type | Description |
| --- | --- | --- |
| oldValue | String | The old text. |
| newValue | String | The new text. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class FontSettingCollectionMethodReplaceWithStringStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape and set text
Shape shape = worksheet.Shapes.AddTextBox(1, 0, 0, 100, 100, 100);
shape.Text = "Sample text ３４ for replacement";
// Replace text in the shape
shape.TextBody.Replace("３４", "ABC");
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
