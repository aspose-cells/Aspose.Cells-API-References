##CellsHelper.ColumnNameToIndex
CellsHelper method. Gets column index according to column name
## CellsHelper.ColumnNameToIndex method
Gets column index according to column name.
```csharp
public static int ColumnNameToIndex(string columnName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| columnName | String | Column name. |
### Return Value
Column index.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsHelperMethodColumnNameToIndexWithStringDemo
{
public static void Run()
{
int columnIndex = CellsHelper.ColumnNameToIndex("BAA");
string columnName = CellsHelper.ColumnIndexToName(columnIndex);
Console.WriteLine("Column Name: " + columnName);
Console.WriteLine("Column Index: " + columnIndex);
}
}
}
```
### See Also
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
