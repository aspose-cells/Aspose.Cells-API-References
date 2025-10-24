##OoxmlSaveOptions.OoxmlSaveOptions
OoxmlSaveOptions constructor. Creates the options for saving office open xml file
## OoxmlSaveOptions() {#constructor}
Creates the options for saving office open xml file.
```csharp
public OoxmlSaveOptions()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class OoxmlSaveOptionsMethodCtorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet and add some data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Hello World!");
// Demonstrate OoxmlSaveOptions constructor
OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
saveOptions.CompressionType = OoxmlCompressionType.Level6;
// Save the workbook with OOXML options
workbook.Save("output.xlsx", saveOptions);
Console.WriteLine("Workbook saved with OOXML options.");
}
}
}
```
### See Also
* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## OoxmlSaveOptions(SaveFormat) {#constructor_1}
Creates the options for saving office open xml file.
```csharp
public OoxmlSaveOptions(SaveFormat saveFormat)
```
| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The file format. It should be one of following types: Xlsx, Xltx, Xlam, Xlsm or Xltm, otherwise the saved format will be set as Xlsx automatically. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class OoxmlSaveOptionsMethodCtorWithSaveFormatDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data to the worksheet
worksheet.Cells["A1"].PutValue("Sample Data");
try
{
// Create OoxmlSaveOptions with SaveFormat parameter
OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx);
// Set some properties of the save options
saveOptions.ExportCellName = true;
saveOptions.CompressionType = OoxmlCompressionType.Level6;
Console.WriteLine("OoxmlSaveOptions created successfully with SaveFormat.Xlsx");
// Save the workbook with the specified options
workbook.Save("OoxmlSaveOptionsCtorDemo.xlsx", saveOptions);
}
catch (Exception ex)
{
Console.WriteLine($"Error creating OoxmlSaveOptions: {ex.Message}");
}
}
}
}
```
### See Also
* enum [SaveFormat](../../saveformat/)
* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
