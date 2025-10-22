##OdsSaveOptions.OdsSaveOptions
OdsSaveOptions constructor. Creates the options of saving ods file
## OdsSaveOptions() {#constructor}
Creates the options of saving ods file.
```csharp
public OdsSaveOptions()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class OdsSaveOptionsMethodCtorDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample cells with different border styles
worksheet.Cells["B2"].PutValue("Medium Border");
worksheet.Cells["B4"].PutValue("Thick Border");
worksheet.Cells["B7"].PutValue("Double Border");
Style style = workbook.CreateStyle();
style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Medium;
worksheet.Cells["B2"].SetStyle(style);
style = workbook.CreateStyle();
style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thick;
worksheet.Cells["B4"].SetStyle(style);
style = workbook.CreateStyle();
style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Double;
worksheet.Cells["B7"].SetStyle(style);
// Demonstrate OdsSaveOptions constructor
OdsSaveOptions saveOptions = new OdsSaveOptions();
saveOptions.GeneratorType = Aspose.Cells.Ods.OdsGeneratorType.LibreOffice;
// Save as ODS file
workbook.Save("output.ods", saveOptions);
Console.WriteLine("File saved with OdsSaveOptions constructor demo.");
}
}
}
```
### See Also
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## OdsSaveOptions(SaveFormat) {#constructor_1}
Creates the options of saving ods file.
```csharp
public OdsSaveOptions(SaveFormat saveFormat)
```
| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The file format. It should be Ods, Ots, Fods or Sxc, otherwise the saved format will be set as Ods automatically. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Ods;
using System;
public class OdsSaveOptionsMethodCtorWithSaveFormatDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data to the worksheet
worksheet.Cells["A1"].PutValue("Sample Data");
worksheet.Cells["B1"].PutValue(123.45);
try
{
// Call the #ctor method with SaveFormat parameter
OdsSaveOptions saveOptions = new OdsSaveOptions(SaveFormat.Ods);
// Set some properties of the save options
saveOptions.GeneratorType = OdsGeneratorType.LibreOffice;
saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf12;
Console.WriteLine("OdsSaveOptions constructor executed successfully with SaveFormat.Ods parameter");
// Save the workbook with the specified options
workbook.Save("OdsSaveOptionsCtorDemo.ods", saveOptions);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing OdsSaveOptions constructor: {ex.Message}");
}
}
}
}
```
### See Also
* enum [SaveFormat](../../saveformat/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
