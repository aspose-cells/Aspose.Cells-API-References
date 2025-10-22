##PptxSaveOptions.PptxSaveOptions
PptxSaveOptions constructor. Represents the pptx save options
## PptxSaveOptions() {#constructor}
Represents the pptx save options.
```csharp
public PptxSaveOptions()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PptxSaveOptionsMethodCtorDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Visible Data");
worksheet.Cells["A2"].PutValue("Hidden Data");
worksheet.Cells["B1"].PutValue(100);
worksheet.Cells["B2"].PutValue(200);
// Hide the second row
worksheet.Cells.Rows[1].IsHidden = true;
// Create PptxSaveOptions using constructor
PptxSaveOptions saveOptions = new PptxSaveOptions();
saveOptions.IgnoreHiddenRows = true;
// Save workbook to PPTX with options
workbook.Save("output.pptx", saveOptions);
Console.WriteLine("Workbook saved to PPTX with hidden rows ignored.");
}
}
}
```
### See Also
* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## PptxSaveOptions(bool) {#constructor_1}
Represents options of saving .pptx file.
```csharp
public PptxSaveOptions(bool saveAsImage)
```
| Parameter | Type | Description |
| --- | --- | --- |
| saveAsImage | Boolean | If True, the workbook will be converted into some pictures of .pptx file. If False, the workbook will be converted into some tables of .pptx file. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Slides;
using System;
public class PptxSaveOptionsMethodCtorWithBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Sample Data");
worksheet.Cells["A2"].PutValue(123);
worksheet.Cells["A3"].PutValue(DateTime.Now);
try
{
// Call the #ctor method with boolean parameter
bool saveAsImage = true;
PptxSaveOptions options = new PptxSaveOptions(saveAsImage);
// Set additional properties
options.IgnoreHiddenRows = true;
options.ExportViewType = SlideViewType.View;
// Save the workbook with PPTX options
workbook.Save("PptxSaveOptionsCtorDemo.pptx", options);
Console.WriteLine("PptxSaveOptions constructor executed successfully with parameter: " + saveAsImage);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing PptxSaveOptions constructor: {ex.Message}");
}
}
}
}
```
### See Also
* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
