##Workbook.GetFonts
Workbook method. Gets all fonts in the style pool
## Workbook.GetFonts method
Gets all fonts in the style pool.
```csharp
public Font[] GetFonts()
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodGetFontsDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create cells with different fonts
worksheet.Cells["A1"].PutValue("Sample Text 1");
worksheet.Cells["A2"].PutValue("Sample Text 2");
// Get and modify fonts
Font font1 = worksheet.Cells["A1"].GetStyle().Font;
font1.Name = "Arial";
font1.Size = 12;
Font font2 = worksheet.Cells["A2"].GetStyle().Font;
font2.Name = "Times New Roman";
font2.Size = 14;
font2.IsBold = true;
// Get all fonts used in the workbook
Font[] fonts = workbook.GetFonts();
Console.WriteLine("Total fonts in workbook: " + fonts.Length);
// Display font information
foreach (Font font in fonts)
{
Console.WriteLine($"Font: {font.Name}, Size: {font.Size}, Bold: {font.IsBold}");
}
// Save and reload to demonstrate persistence
using (MemoryStream stream = new MemoryStream())
{
workbook.Save(stream, SaveFormat.Xlsx);
Workbook loadedWorkbook = new Workbook(stream);
Console.WriteLine("Fonts after save/load: " + loadedWorkbook.GetFonts().Length);
}
}
}
}
```
### See Also
* class [Font](../../font/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
