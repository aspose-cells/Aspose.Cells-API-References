##FontSetting.FontSetting
FontSetting constructor.
## FontSetting constructor
```csharp
public FontSetting(int startIndex, int length, WorksheetCollection sheets)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | Int32 |  |
| length | Int32 |  |
| sheets | WorksheetCollection |  |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FontSettingMethodCtorWithInt32Int32WorksheetCollectionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample text to cell
worksheet.Cells["A1"].PutValue("Hello World");
// Create font setting for the first 5 characters (0-4) in all worksheets
FontSetting fontSetting = new FontSetting(0, 5, workbook.Worksheets);
// Apply formatting
fontSetting.Font.Color = System.Drawing.Color.Red;
fontSetting.Font.IsBold = true;
fontSetting.Font.Size = 14;
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [WorksheetCollection](../../worksheetcollection/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
