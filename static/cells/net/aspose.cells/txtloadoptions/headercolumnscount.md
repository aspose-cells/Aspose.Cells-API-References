##TxtLoadOptions.HeaderColumnsCount
TxtLoadOptions property. The count of header columns to be repeated for extended sheets
## TxtLoadOptions.HeaderColumnsCount property
The count of header columns to be repeated for extended sheets.
```csharp
public int HeaderColumnsCount { get; set; }
```
### Remarks
The header columns specified by this property will be duplicated for those extended sheets. This property only takes effect when [`ExtendToNextSheet`](../extendtonextsheet/) is true.
### Examples
```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TxtLoadOptionsPropertyHeaderColumnsCountDemo
{
public static void Run()
{
// Create sample CSV content
string csvData = "Header1,Header2,Header3,Data1,Data2,Data3\n" +
"H1,H2,H3,D1,D2,D3\n" +
"A,B,C,D,E,F\n" +
"G,H,I,J,K,L";
// Create TxtLoadOptions with HeaderColumnsCount set to 3
TxtLoadOptions options = new TxtLoadOptions
{
HeaderColumnsCount = 3, // First 3 columns will be treated as headers
Encoding = Encoding.UTF8
};
// Load the CSV data into a workbook
using (MemoryStream stream = new MemoryStream(Encoding.UTF8.GetBytes(csvData)))
{
Workbook workbook = new Workbook(stream, options);
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Demonstrate header columns (first 3 columns)
Console.WriteLine("Header Columns:");
for (int row = 0; row < 2; row++)
{
for (int col = 0; col < options.HeaderColumnsCount; col++)
{
Console.Write(cells[row, col].StringValue + "\t");
}
Console.WriteLine();
}
// Demonstrate data columns (remaining columns)
Console.WriteLine("\nData Columns:");
for (int row = 0; row < cells.MaxDataRow + 1; row++)
{
for (int col = options.HeaderColumnsCount; col < cells.MaxDataColumn + 1; col++)
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
