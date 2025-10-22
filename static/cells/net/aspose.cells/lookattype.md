##Enum LookAtType
Aspose.Cells.LookAtType enum. Represents look at type
## LookAtType enumeration
Represents look at type.
```csharp
public enum LookAtType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Contains | `0` | Cell value Contains the find object. |
| StartWith | `1` | Cell value Starts with the find object. |
| EndWith | `2` | Cell value ends with the find object. |
| EntireContent | `3` | Cell value is same as the find object. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class LookAtTypeDemo
{
public static void LookAtTypeExample()
{
// Instantiate the workbook object
Workbook workbook = new Workbook("LookAtTypeExample_original.xlsx");
// Get Cells collection
Cells cells = workbook.Worksheets[0].Cells;
// Instantiate FindOptions Object
FindOptions findOptions = new FindOptions();
// Create a Cells Area
CellArea ca = new CellArea();
ca.StartRow = 8;
ca.StartColumn = 2;
ca.EndRow = 17;
ca.EndColumn = 13;
// Set cells area for find options
findOptions.SetRange(ca);
// Set searching properties
findOptions.SearchBackward = false;
findOptions.SeachOrderByRows = true;
findOptions.LookInType = LookInType.Values;
// Set LookAtType to Contains
findOptions.LookAtType = LookAtType.Contains;
// Find the cell with a specific value
Cell cell = cells.Find("searchValue", null, findOptions);
if (cell != null)
{
Console.WriteLine($"Cell found at row {cell.Row}, column {cell.Column}");
}
else
{
Console.WriteLine("Cell not found.");
}
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
