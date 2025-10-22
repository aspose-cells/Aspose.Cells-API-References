##Enum TxtLoadStyleStrategy
Aspose.Cells.TxtLoadStyleStrategy enum. Specifies how to apply style for parsed values when converting string value to number or datetime
## TxtLoadStyleStrategy enumeration
Specifies how to apply style for parsed values when converting string value to number or datetime.
```csharp
public enum TxtLoadStyleStrategy
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | Does not set style for the parsed value. |
| BuiltIn | `1` | Set the style as built-in number/datetime when the parsed value are plain numeric/datetime values. |
| ExactFormat | `2` | Set the exact custom format for the parsed value to make the formatted value be same with the original input one. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class TxtLoadStyleStrategyDemo
{
public static void TxtLoadStyleStrategyExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Define a sample CSV content
string csvContent = "Name,Date,Value\nJohn,2023-01-01,100\nDoe,2023-01-02,200";
// Save the CSV content to a temporary file
string tempCsvFilePath = "sample.csv";
System.IO.File.WriteAllText(tempCsvFilePath, csvContent);
// Create TxtLoadOptions and set the LoadStyleStrategy
TxtLoadOptions loadOptions = new TxtLoadOptions();
loadOptions.LoadStyleStrategy = TxtLoadStyleStrategy.ExactFormat;
// Load the CSV file into the workbook
workbook = new Workbook(tempCsvFilePath, loadOptions);
// Save the workbook to an Excel file
workbook.Save("TxtLoadStyleStrategyExample.xlsx");
// Clean up the temporary CSV file
System.IO.File.Delete(tempCsvFilePath);
Console.WriteLine("Workbook created and saved successfully.");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
