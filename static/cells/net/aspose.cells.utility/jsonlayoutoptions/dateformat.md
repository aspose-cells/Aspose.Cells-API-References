##JsonLayoutOptions.DateFormat
JsonLayoutOptions property. Gets and sets the format of date value
## JsonLayoutOptions.DateFormat property
Gets and sets the format of date value.
```csharp
public string DateFormat { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;
namespace AsposeCellsExamples
{
public class JsonLayoutOptionsPropertyDateFormatDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Configure JSON import options with custom date format
JsonLayoutOptions layoutOptions = new JsonLayoutOptions();
layoutOptions.ArrayAsTable = true;
layoutOptions.ConvertNumericOrDate = true;
layoutOptions.DateFormat = "DD-MM-YYYY";
// Import JSON data with date values
string jsonData = "{\"date\":\"15-05-2023\",\"name\":\"John Doe\"}";
JsonUtility.ImportData(jsonData, worksheet.Cells, 0, 0, layoutOptions);
// Verify the date was imported with correct formatting
Cell dateCell = worksheet.Cells["A2"];
Console.WriteLine("Imported date value: " + dateCell.StringValue);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)
