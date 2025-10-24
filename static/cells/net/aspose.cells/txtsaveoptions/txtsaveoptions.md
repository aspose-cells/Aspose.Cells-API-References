##TxtSaveOptions.TxtSaveOptions
TxtSaveOptions constructor. Creates text file save options
## TxtSaveOptions() {#constructor}
Creates text file save options.
```csharp
public TxtSaveOptions()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TxtSaveOptionsMethodCtorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
// Demonstrate TxtSaveOptions constructor
TxtSaveOptions txtSaveOptions = new TxtSaveOptions();
txtSaveOptions.SeparatorString = "|";
// Save with custom separator
workbook.Save("output.txt", txtSaveOptions);
Console.WriteLine("File saved with custom separator successfully.");
}
}
}
```
### See Also
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## TxtSaveOptions(SaveFormat) {#constructor_1}
Creates text file save options.
```csharp
public TxtSaveOptions(SaveFormat saveFormat)
```
| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The file format. It should be Csv or Tsv, otherwise the saved format will be set as Csv automatically. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Text;
public class TxtSaveOptionsMethodCtorWithSaveFormatDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Jane");
worksheet.Cells["B3"].PutValue(25);
try
{
// Call the #ctor method with SaveFormat parameter
TxtSaveOptions saveOptions = new TxtSaveOptions(SaveFormat.Csv);
// Configure the save options
saveOptions.Separator = ',';
saveOptions.Encoding = Encoding.UTF8;
saveOptions.QuoteType = TxtValueQuoteType.Always;
Console.WriteLine("TxtSaveOptions created successfully with SaveFormat.Csv");
// Save the workbook with the configured options
workbook.Save("TxtSaveOptionsDemo.csv", saveOptions);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing TxtSaveOptions constructor: {ex.Message}");
}
}
}
}
```
### See Also
* enum [SaveFormat](../../saveformat/)
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
