##XlsSaveOptions.XlsSaveOptions
XlsSaveOptions constructor. Creates options for saving Excel 972003 xls file
## XlsSaveOptions() {#constructor}
Creates options for saving Excel 97-2003 xls file.
```csharp
public XlsSaveOptions()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class XlsSaveOptionsMethodCtorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Sample XLS File");
worksheet.Cells["A2"].PutValue("Created using XlsSaveOptions");
// Initialize XlsSaveOptions using the constructor
XlsSaveOptions saveOptions = new XlsSaveOptions();
// Set some options (removed unsupported properties)
saveOptions.IsTemplate = false;
// Save the workbook with the options
workbook.Save("output.xls", saveOptions);
Console.WriteLine("File saved successfully with XlsSaveOptions.");
}
}
}
```
### See Also
* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## XlsSaveOptions(SaveFormat) {#constructor_1}
Creates options for saving Excel 97-2003 xls/xlt file.
```csharp
public XlsSaveOptions(SaveFormat saveFormat)
```
| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The file format. It should be Excel97To2003 or Xlt, otherwise the saved format will be set as Excel97To2003 automatically. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class XlsSaveOptionsMethodCtorWithSaveFormatDemo
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
XlsSaveOptions saveOptions = new XlsSaveOptions(SaveFormat.Excel97To2003);
// Set additional properties
saveOptions.MatchColor = true;
saveOptions.WpsCompatibility = false;
Console.WriteLine("XlsSaveOptions constructor executed successfully with SaveFormat parameter");
// Save the workbook with the specified options
workbook.Save("XlsSaveOptionsCtorDemo.xls", saveOptions);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing XlsSaveOptions constructor: {ex.Message}");
}
}
}
}
```
### See Also
* enum [SaveFormat](../../saveformat/)
* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
