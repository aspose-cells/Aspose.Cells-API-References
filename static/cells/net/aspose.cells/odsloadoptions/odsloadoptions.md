##OdsLoadOptions.OdsLoadOptions
OdsLoadOptions constructor. Represents the options of loading ods file
## OdsLoadOptions() {#constructor}
Represents the options of loading ods file.
```csharp
public OdsLoadOptions()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class OdsLoadOptionsMethodCtorDemo
{
public static void Run()
{
// Create OdsLoadOptions using the constructor
OdsLoadOptions loadOptions = new OdsLoadOptions();
// Set hyperlink style to use Excel defaults
loadOptions.ApplyExcelDefaultStyleToHyperlink = true;
// Load ODS file with the load options
Workbook workbook = new Workbook("example.ods", loadOptions);
// Save as XLSX
workbook.Save("output.xlsx");
// Verify hyperlink style was applied
Console.WriteLine("Hyperlink style color: " +
workbook.Worksheets[0].Cells["B1"].GetStyle().Font.Color);
}
}
}
```
### See Also
* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## OdsLoadOptions(LoadFormat) {#constructor_1}
Represents the options of loading ods file.
```csharp
public OdsLoadOptions(LoadFormat type)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | LoadFormat | The load format type. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.IO;
public class OdsLoadOptionsMethodCtorWithLoadFormatDemo
{
public static void Run()
{
// Create sample ODS file if it doesn't exist
string inputFile = "input.ods";
if (!File.Exists(inputFile))
{
using (Workbook sampleWorkbook = new Workbook())
{
sampleWorkbook.Worksheets[0].Hyperlinks.Add("A1", 1, 1, "https://example.com");
sampleWorkbook.Save(inputFile, SaveFormat.Ods);
}
}
// Create OdsLoadOptions with LoadFormat parameter
OdsLoadOptions loadOptions = new OdsLoadOptions(LoadFormat.Ods);
loadOptions.ApplyExcelDefaultStyleToHyperlink = true;
try
{
// Load workbook with created load options
using (Workbook workbook = new Workbook(inputFile, loadOptions))
{
Console.WriteLine($"Hyperlink style applied: {loadOptions.ApplyExcelDefaultStyleToHyperlink}");
// Save to demonstrate successful load
workbook.Save("OdsLoadOptionsCtorDemo.xlsx");
}
}
catch (FileNotFoundException)
{
Console.WriteLine("Error: Created sample file missing - please verify permissions");
}
catch (Exception ex)
{
Console.WriteLine($"Error loading ODS file: {ex.Message}");
}
}
}
}
```
### See Also
* enum [LoadFormat](../../loadformat/)
* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
