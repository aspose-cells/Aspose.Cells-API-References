##Class LowCodeHtmlSaveOptions
Aspose.Cells.LowCode.LowCodeHtmlSaveOptions class. Options for saving html in low code way
## LowCodeHtmlSaveOptions class
Options for saving html in low code way.
```csharp
public class LowCodeHtmlSaveOptions : LowCodeSaveOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [LowCodeHtmlSaveOptions](lowcodehtmlsaveoptions/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [HtmlOptions](../../aspose.cells.lowcode/lowcodehtmlsaveoptions/htmloptions/) { get; set; } | The general options for saving html. |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | Gets and sets the file(with path if needed) for saving the generated data. When setting this property with value other than null or empty string, [`OutputStream`](../lowcodesaveoptions/outputstream/) will be ignored.(Inherited from [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | Gets and sets the Stream for writing the generated data to. When setting this property with value other than null, [`OutputFile`](../lowcodesaveoptions/outputfile/) will be ignored.(Inherited from [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| override [SaveFormat](../../aspose.cells.lowcode/lowcodehtmlsaveoptions/saveformat/) { get; set; } | Gets and sets the format of spreadsheet. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class LowCodeClassLowCodeHtmlSaveOptionsDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Price");
worksheet.Cells["A2"].PutValue("Widget");
worksheet.Cells["B2"].PutValue(29.99);
// Create and configure LowCodeHtmlSaveOptions
LowCodeHtmlSaveOptions saveOptions = new LowCodeHtmlSaveOptions
{
HtmlOptions = new HtmlSaveOptions()
{
ExportWorksheetCSSSeparately = false,
ExportImagesAsBase64 = true
}
};
// Save workbook with configured HTML options using the save options parameter
workbook.Save("LowCodeHtmlExport.html", saveOptions.HtmlOptions);
Console.WriteLine("HTML file saved successfully with low code options.");
}
}
}
```
### See Also
* class [LowCodeSaveOptions](../lowcodesaveoptions/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)
