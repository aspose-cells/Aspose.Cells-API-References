##AbstractTextLoadOptions.ConvertNumericData
AbstractTextLoadOptions property. Gets or sets a value that indicates whether the string in text file is converted to numeric data. Default value is true
## AbstractTextLoadOptions.ConvertNumericData property
Gets or sets a value that indicates whether the string in text file is converted to numeric data. Default value is true.
```csharp
public bool ConvertNumericData { get; set; }
```
### Examples
```csharp
using System;
using System.Text;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class AbstractTextLoadOptionsPropertyConvertNumericDataDemo
{
public static void Run()
{
// Create sample CSV data with numeric and string values
string csvData = "ID,Name,Price,Quantity\n" +
"1,Product A,19.99,5\n" +
"2,Product B,\"24.50\",\"10\"\n" +
"3,Product C,15.75,\"N/A\"";
// Create TxtLoadOptions with ConvertNumericData set to true
TxtLoadOptions options = new TxtLoadOptions(LoadFormat.Csv)
{
ConvertNumericData = true,
ConvertDateTimeData = true
};
// Load the CSV data into a workbook
Workbook workbook = new Workbook(new System.IO.MemoryStream(Encoding.UTF8.GetBytes(csvData)), options);
Worksheet worksheet = workbook.Worksheets[0];
// Demonstrate numeric conversion
Console.WriteLine("Cell B2 (Product A Price) value type: " + worksheet.Cells["B2"].Value.GetType());
Console.WriteLine("Cell B2 value: " + worksheet.Cells["B2"].Value);
// Demonstrate string values that couldn't be converted
Console.WriteLine("\nCell D4 (N/A) value type: " + worksheet.Cells["D4"].Value.GetType());
Console.WriteLine("Cell D4 value: " + worksheet.Cells["D4"].Value);
// Show how quoted numbers are still converted when ConvertNumericData is true
Console.WriteLine("\nCell C3 (Quoted \"24.50\") value type: " + worksheet.Cells["C3"].Value.GetType());
Console.WriteLine("Cell C3 value: " + worksheet.Cells["C3"].Value);
}
}
}
```
### See Also
* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
