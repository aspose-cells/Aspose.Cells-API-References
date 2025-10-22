##SpreadsheetML2003SaveOptions.SpreadsheetML2003SaveOptions
SpreadsheetML2003SaveOptions constructor. Creates the options for saving Excel 2003 spreadml file
## SpreadsheetML2003SaveOptions() {#constructor}
Creates the options for saving Excel 2003 spreadml file.
```csharp
public SpreadsheetML2003SaveOptions()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class SpreadsheetML2003SaveOptionsMethodCtorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet and add some sample data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Sample Data");
worksheet.Cells["A2"].PutValue(123);
worksheet.Cells["A3"].PutValue(DateTime.Now);
// Create SpreadsheetML2003SaveOptions with constructor
SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();
// Set options
saveOptions.LimitAsXls = true;
saveOptions.ExportColumnIndexOfCell = true;
// Save with the options
workbook.Save("output.xml", saveOptions);
Console.WriteLine("File saved with SpreadsheetML2003SaveOptions");
}
}
}
```
### See Also
* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## SpreadsheetML2003SaveOptions(SaveFormat) {#constructor_1}
Creates the options for saving Excel 2003 spreadml file.
```csharp
[Obsolete("Use SpreadsheetML2003SaveOptions() constructor instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public SpreadsheetML2003SaveOptions(SaveFormat saveFormat)
```
| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The save format. |
### Remarks
NOTE: This constructor is now obsolete. Instead, please use SpreadsheetML2003SaveOptions() constructor. This property will be removed 12 months later since January 2021. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class SpreadsheetML2003SaveOptionsMethodCtorWithSaveFormatDemo
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
SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();
// Set some properties of the save options
saveOptions.IsIndentedFormatting = true;
saveOptions.LimitAsXls = false;
saveOptions.ExportColumnIndexOfCell = true;
Console.WriteLine("SpreadsheetML2003SaveOptions created successfully with SaveFormat parameter");
// Save the workbook using the created save options
workbook.Save("SpreadsheetML2003Output.xml", saveOptions);
Console.WriteLine("Workbook saved successfully with SpreadsheetML2003SaveOptions");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SpreadsheetML2003SaveOptions constructor: {ex.Message}");
}
}
}
}
```
### See Also
* enum [SaveFormat](../../saveformat/)
* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
