##FontSetting.Length
FontSetting property. Gets the length of the characters
## FontSetting.Length property
Gets the length of the characters.
```csharp
public int Length { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FontSettingPropertyLengthDemo
{
public static void Run()
{
// Create a workbook and access its first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some text to cell A1
worksheet.Cells["A1"].PutValue("Hello World");
// Create font settings for the text in cell A1
FontSetting fontSetting = worksheet.Cells["A1"].Characters(0, 5);
// Demonstrate Length property usage
Console.WriteLine("Original Length: " + fontSetting.Length);
// Modify the length of the font setting
fontSetting = worksheet.Cells["A1"].Characters(0, 11);
Console.WriteLine("Modified Length: " + fontSetting.Length);
// Apply formatting to the font setting
fontSetting.Font.Color = System.Drawing.Color.Red;
fontSetting.Font.IsBold = true;
// Save the workbook
workbook.Save("FontSettingLengthDemo.xlsx");
}
}
}
```
### See Also
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
