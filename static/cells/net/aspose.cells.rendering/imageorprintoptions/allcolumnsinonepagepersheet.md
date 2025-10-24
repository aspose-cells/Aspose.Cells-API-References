##ImageOrPrintOptions.AllColumnsInOnePagePerSheet
ImageOrPrintOptions property. If AllColumnsInOnePagePerSheet is true  all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be invalid and the other settings of pagesetup will still take effect
## ImageOrPrintOptions.AllColumnsInOnePagePerSheet property
If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.
```csharp
public bool AllColumnsInOnePagePerSheet { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ImageOrPrintOptionsPropertyAllColumnsInOnePagePerSheetDemo
{
public static void Run()
{
// Create a workbook and add sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Fill some data in the worksheet
for (int i = 0; i < 10; i++)
{
for (int j = 0; j < 5; j++)
{
worksheet.Cells[i, j].PutValue($"Data {i},{j}");
}
}
// Create image save options
ImageSaveOptions pngOptions = new ImageSaveOptions(SaveFormat.Png);
pngOptions.ImageOrPrintOptions.AllColumnsInOnePagePerSheet = true;
pngOptions.ImageOrPrintOptions.OnePagePerSheet = true;
// Save workbook to memory stream as PNG
using (MemoryStream ms = new MemoryStream())
{
workbook.Save(ms, pngOptions);
Console.WriteLine("Workbook saved as PNG with all columns in one page per sheet.");
}
}
}
}
```
### See Also
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
