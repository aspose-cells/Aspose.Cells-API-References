##TxtLoadOptions.MaxRowCount
TxtLoadOptions property. The maximum count of rows to be imported for one sheet
## TxtLoadOptions.MaxRowCount property
The maximum count of rows to be imported for one sheet.
```csharp
public int MaxRowCount { get; set; }
```
### Remarks
Those rows exceeding this limit will be ignored or extended to next sheet according to [`ExtendToNextSheet`](../extendtonextsheet/). This count includes the header rows([`HeaderRowsCount`](../headerrowscount/)). The maximum allowed value of it is the row limit of corresponding file format, such as for xlsx file it 1048576. If this property has not been specified or the specified value is not positive, then the maximum limit will be used too.
### Examples
```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TxtLoadOptionsPropertyMaxRowCountDemo
{
public static void Run()
{
// Create sample CSV content
string content = "Header1,Header2,Header3\n" +
"Data1,Data2,Data3\n" +
"Data4,Data5,Data6\n" +
"Data7,Data8,Data9\n" +
"Data10,Data11,Data12\n" +
"Data13,Data14,Data15\n" +
"Data16,Data17,Data18";
// Create TxtLoadOptions with MaxRowCount set to 4
TxtLoadOptions opts = new TxtLoadOptions
{
MaxRowCount = 4,  // Only load first 4 rows (including header)
HeaderRowsCount = 1  // First row is header
};
// Load the CSV into workbook
using (MemoryStream ms = new MemoryStream(Encoding.UTF8.GetBytes(content)))
{
Workbook wb = new Workbook(ms, opts);
// Verify only 4 rows were loaded (1 header + 3 data rows)
Worksheet sheet = wb.Worksheets[0];
Console.WriteLine($"Total rows loaded: {sheet.Cells.MaxDataRow + 1}");
Console.WriteLine($"Row 1 (Header): {sheet.Cells[0, 0].StringValue}");
Console.WriteLine($"Row 2 (Data): {sheet.Cells[1, 0].StringValue}");
Console.WriteLine($"Row 3 (Data): {sheet.Cells[2, 0].StringValue}");
Console.WriteLine($"Row 4 (Data): {sheet.Cells[3, 0].StringValue}");
// This would be null since we only loaded 4 rows (index 0-3)
if (sheet.Cells[4, 0] == null || string.IsNullOrEmpty(sheet.Cells[4, 0].StringValue))
{
Console.WriteLine("Row 5 was not loaded due to MaxRowCount limitation");
}
}
}
}
}
```
### See Also
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
