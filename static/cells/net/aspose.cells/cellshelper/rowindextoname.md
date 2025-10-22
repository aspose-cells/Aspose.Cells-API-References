##CellsHelper.RowIndexToName
CellsHelper method. Gets row name according to row index
## CellsHelper.RowIndexToName method
Gets row name according to row index.
```csharp
public static string RowIndexToName(int row)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index. |
### Return Value
Name of row.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsHelperMethodRowIndexToNameWithInt32Demo
{
public static void Run()
{
int rowIndex = 10;
string rowName = CellsHelper.RowIndexToName(rowIndex);
Console.WriteLine("Row index {0} corresponds to row name: {1}", rowIndex, rowName);
int convertedBackIndex = CellsHelper.RowNameToIndex(rowName);
Console.WriteLine("Row name {0} converted back to index: {1}", rowName, convertedBackIndex);
}
}
}
```
### See Also
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
