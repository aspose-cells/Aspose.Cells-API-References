##FontSettingCollection.Format
FontSettingCollection method. Format the text with font setting
## FontSettingCollection.Format method
Format the text with font setting.
```csharp
public void Format(int startIndex, int length, Font font, StyleFlag flag)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | Int32 | The start index. |
| length | Int32 | The length. |
| font | Font | The font. |
| flag | StyleFlag | The flags of the font. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing.Texts;
using System;
public class FontSettingCollectionMethodFormatWithInt32Int32FontStyleFlagDemo
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
fontSettingCollection.Text = "Sample Text for Formatting";
try
{
// Create a style and set its font properties
Style style = workbook.CreateStyle();
style.Font.Name = "Arial";
style.Font.Size = 14;
style.Font.IsBold = true;
style.Font.Color = System.Drawing.Color.Red;
// Create style flag to specify which font properties to apply
StyleFlag styleFlag = new StyleFlag();
styleFlag.FontName = true;
styleFlag.FontSize = true;
styleFlag.FontBold = true;
styleFlag.FontColor = true;
// Format characters from index 7 to 11 (the word "Text")
fontSettingCollection.Format(7, 4, style.Font, styleFlag);
// Save the workbook to show the effect
workbook.Save("FontSettingCollectionFormatDemo.xlsx");
Console.WriteLine("Format method executed successfully. Text 'Text' is now bold, red Arial 14pt.");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Format method: {ex.Message}");
}
}
}
}
```
### See Also
* class [Font](../../../aspose.cells/font/)
* class [StyleFlag](../../../aspose.cells/styleflag/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
