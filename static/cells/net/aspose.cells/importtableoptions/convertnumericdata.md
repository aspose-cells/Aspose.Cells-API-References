##ImportTableOptions.ConvertNumericData
ImportTableOptions property. Gets or sets a value that indicates whether the string value should be converted to numeric or date value
## ImportTableOptions.ConvertNumericData property
Gets or sets a value that indicates whether the string value should be converted to numeric or date value.
```csharp
public bool ConvertNumericData { get; set; }
```
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ImportTableOptionsPropertyConvertNumericDataDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Create sample data table with numeric and string values
DataTable dt = new DataTable();
dt.Columns.Add("Numbers");
dt.Columns.Add("Text");
dt.Rows.Add("123", "456");
dt.Rows.Add("ABC", "DEF");
// Get the first worksheet cells
Cells cells = workbook.Worksheets[0].Cells;
// Create import options with ConvertNumericData set to true
ImportTableOptions options = new ImportTableOptions();
options.ConvertNumericData = true;
options.IsFieldNameShown = true;
// Import data with numeric conversion
cells.ImportData(dt, 0, 0, options);
// Display results
Console.WriteLine("A2 (numeric converted): " + cells["A2"].Value + " - Type: " + cells["A2"].Type);
Console.WriteLine("B2 (string remains): " + cells["B2"].StringValue + " - Type: " + cells["B2"].Type);
}
}
}
```
### See Also
* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
