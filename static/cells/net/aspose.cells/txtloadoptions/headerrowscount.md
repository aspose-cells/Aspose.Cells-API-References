##TxtLoadOptions.HeaderRowsCount
TxtLoadOptions property. The count of header rows to be repeated for extended sheets
## TxtLoadOptions.HeaderRowsCount property
The count of header rows to be repeated for extended sheets.
```csharp
public int HeaderRowsCount { get; set; }
```
### Remarks
The header rows specified by this property will be duplicated for those extended sheets. This property only takes effect when [`ExtendToNextSheet`](../extendtonextsheet/) is true.
### Examples
```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TxtLoadOptionsPropertyHeaderRowsCountDemo
{
public static void Run()
{
// Create sample CSV content
string csvData = "Header1,Header2,Header3\n" +
"Value1,Value2,Value3\n" +
"Value4,Value5,Value6\n" +
"Value7,Value8,Value9";
// Create TxtLoadOptions with HeaderRowsCount set to 1
TxtLoadOptions options = new TxtLoadOptions
{
HeaderRowsCount = 1
};
// Load the CSV data into a workbook
using (MemoryStream stream = new MemoryStream(Encoding.UTF8.GetBytes(csvData)))
{
Workbook workbook = new Workbook(stream, options);
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Demonstrate that the first row is treated as header
Console.WriteLine("Header Row:");
for (int col = 0; col < cells.MaxDataColumn + 1; col++)
{
Console.Write(cells[0, col].StringValue + "\t");
}
Console.WriteLine("\n");
// Show data rows (skipping the header)
Console.WriteLine("Data Rows:");
for (int row = 1; row < cells.MaxDataRow + 1; row++)
{
for (int col = 0; col < cells.MaxDataColumn + 1; col++)
{
Console.Write(cells[row, col].StringValue + "\t");
}
Console.WriteLine();
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
