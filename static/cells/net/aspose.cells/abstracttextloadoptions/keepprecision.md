##AbstractTextLoadOptions.KeepPrecision
AbstractTextLoadOptions property. Indicates whether not parsing a string value if the length is 15
## AbstractTextLoadOptions.KeepPrecision property
Indicates whether not parsing a string value if the length is 15.
```csharp
public bool KeepPrecision { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class AbstractTextLoadOptionsPropertyKeepPrecisionDemo
{
public static void Run()
{
// Create HTML load options and set KeepPrecision to true
HtmlLoadOptions loadOptions = new HtmlLoadOptions();
loadOptions.KeepPrecision = true;
// Load workbook with the options
Workbook workbook = new Workbook("input.html", loadOptions);
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Demonstrate precision is maintained (e.g., numeric values with many decimal places)
Cell cell = worksheet.Cells["A1"];
Console.WriteLine("Value with precision: " + cell.Value);
// Save the workbook
workbook.Save("output.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
