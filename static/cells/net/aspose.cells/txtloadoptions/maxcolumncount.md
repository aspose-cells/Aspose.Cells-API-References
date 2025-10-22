##TxtLoadOptions.MaxColumnCount
TxtLoadOptions property. The maximum count of columns to be imported for one sheet
## TxtLoadOptions.MaxColumnCount property
The maximum count of columns to be imported for one sheet.
```csharp
public int MaxColumnCount { get; set; }
```
### Remarks
Those columns exceeding this limit will be ignored or extended to next sheet according to [`ExtendToNextSheet`](../extendtonextsheet/). This count includes the header columns([`HeaderColumnsCount`](../headercolumnscount/)). The maximum value of it is the column limit of corresponding file format, such as for xlsx file it 16384. If this property has not been specified or the specified value is not positive, then the maximum limit will be used too.
### Examples
```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TxtLoadOptionsPropertyMaxColumnCountDemo
{
public static void Run()
{
// Create sample CSV content
string content = "A,B,C,D,E,F,G,H,I,J,K\n" +
"1,2,3,4,5,6,7,8,9,10,11\n" +
"a,b,c,d,e,f,g,h,i,j,k";
// Create TxtLoadOptions with MaxColumnCount set to 5
TxtLoadOptions options = new TxtLoadOptions
{
MaxColumnCount = 5  // Only load first 5 columns
};
// Load the CSV with limited columns
using (MemoryStream stream = new MemoryStream(Encoding.UTF8.GetBytes(content)))
{
Workbook workbook = new Workbook(stream, options);
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Output the loaded data (only first 5 columns should be present)
Console.WriteLine("Data loaded with MaxColumnCount = 5:");
for (int row = 0; row < cells.MaxDataRow + 1; row++)
{
for (int col = 0; col < cells.MaxDataColumn + 1; col++)
{
Console.Write(cells[row, col].StringValue + "\t");
}
Console.WriteLine();
}
// Verify only 5 columns were loaded
Console.WriteLine($"\nMax loaded columns: {cells.MaxDataColumn + 1}");
}
}
}
}
```
### See Also
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
