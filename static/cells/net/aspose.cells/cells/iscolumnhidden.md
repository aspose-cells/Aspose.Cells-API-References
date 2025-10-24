##Cells.IsColumnHidden
Cells method. Checks whether a column at given index is hidden
## Cells.IsColumnHidden method
Checks whether a column at given index is hidden.
```csharp
public bool IsColumnHidden(int columnIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | column index |
### Return Value
true if the column is hidden.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodIsColumnHiddenWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Hide column C (index 2)
cells.HideColumn(2);
// Check if column C is hidden
bool isHidden = cells.IsColumnHidden(2);
Console.WriteLine("Is column C (index 2) hidden? " + isHidden);
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
