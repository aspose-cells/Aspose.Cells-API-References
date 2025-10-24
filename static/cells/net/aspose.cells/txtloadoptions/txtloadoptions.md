##TxtLoadOptions.TxtLoadOptions
TxtLoadOptions constructor. Creates the options for loading text file
## TxtLoadOptions() {#constructor}
Creates the options for loading text file.
```csharp
public TxtLoadOptions()
```
### Remarks
The default load file type is CSV .
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TxtLoadOptionsMethodCtorDemo
{
public static void Run()
{
// Create new TxtLoadOptions using constructor
TxtLoadOptions loadOptions = new TxtLoadOptions();
// Set separator for CSV file
loadOptions.Separator = ',';
// Create workbook with load options
Workbook workbook = new Workbook("example.csv", loadOptions);
// Output some information from the loaded file
Console.WriteLine("Worksheet count: " + workbook.Worksheets.Count);
Console.WriteLine("First cell value: " + workbook.Worksheets[0].Cells["A1"].Value);
}
}
}
```
### See Also
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## TxtLoadOptions(LoadFormat) {#constructor_1}
Creates the options for loading text file.
```csharp
public TxtLoadOptions(LoadFormat loadFormat)
```
| Parameter | Type | Description |
| --- | --- | --- |
| loadFormat | LoadFormat | The loading format |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.IO;
public class TxtLoadOptionsMethodCtorWithLoadFormatDemo
{
public static void Run()
{
// Create sample CSV content and temporary file
string csvData = "Column1,Column2,Column3\nData1,Data2,Data3";
string tempFile = Path.GetTempFileName();
File.WriteAllText(tempFile, csvData);
try
{
// Create TxtLoadOptions with LoadFormat.Csv
TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv);
loadOptions.Separator = ',';
loadOptions.HasTextQualifier = true;
// Load CSV using the configured options
Workbook workbook = new Workbook(tempFile, loadOptions);
Worksheet worksheet = workbook.Worksheets[0];
// Demonstrate loaded data
Console.WriteLine($"A1 Cell Value: {worksheet.Cells["A1"].StringValue}");
Console.WriteLine($"B2 Cell Value: {worksheet.Cells["B2"].StringValue}");
// Save processed workbook
workbook.Save("TxtLoadOptionsCtorDemoOutput.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing constructor: {ex.Message}");
}
finally
{
// Cleanup temporary file
if (File.Exists(tempFile))
{
File.Delete(tempFile);
}
}
}
}
}
```
### See Also
* enum [LoadFormat](../../loadformat/)
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
