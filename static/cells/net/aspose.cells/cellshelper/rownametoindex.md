##CellsHelper.RowNameToIndex
CellsHelper method. Gets row index according to row name
## CellsHelper.RowNameToIndex method
Gets row index according to row name.
```csharp
public static int RowNameToIndex(string rowName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowName | String | Row name. |
### Return Value
Row index.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsHelperMethodRowNameToIndexWithStringDemo
{
public static void Run()
{
string rowName = "11";
int rowIndex = CellsHelper.RowNameToIndex(rowName);
Console.WriteLine("Row name '{0}' converted to index: {1}", rowName, rowIndex);
}
}
}
```
### See Also
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
