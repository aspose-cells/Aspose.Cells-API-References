##HtmlSaveOptions.IsBorderCollapsed
HtmlSaveOptions property. Indicates whether the table borders are collapsed. The default value is true
## HtmlSaveOptions.IsBorderCollapsed property
Indicates whether the table borders are collapsed. The default value is true.
```csharp
public bool IsBorderCollapsed { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using System.Threading;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyIsBorderCollapsedDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data and borders
Style style = workbook.CreateStyle();
style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
worksheet.Cells["A1"].PutValue("Sample Data");
worksheet.Cells["A1"].SetStyle(style);
worksheet.Cells["B2"].PutValue("With Borders");
worksheet.Cells["B2"].SetStyle(style);
// Set culture for demonstration
var culture = new System.Globalization.CultureInfo("de-DE");
Thread.CurrentThread.CurrentCulture = culture;
Thread.CurrentThread.CurrentUICulture = culture;
workbook.Settings.CultureInfo = culture;
// Create HTML save options and set IsBorderCollapsed
HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
saveOptions.IsBorderCollapsed = false;
// Save the workbook with HTML options
string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "HtmlWithBorders.html");
workbook.Save(outputPath, saveOptions);
Console.WriteLine("File saved with collapsed borders: " + outputPath);
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
