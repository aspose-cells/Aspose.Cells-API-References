##Class CellValue
Aspose.Cells.CellValue class. Represents the cell value and corresponding type
## CellValue class
Represents the cell value and corresponding type.
```csharp
public class CellValue
```
## Constructors
| Name | Description |
| --- | --- |
| [CellValue](cellvalue/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [Type](../../aspose.cells/cellvalue/type/) { get; set; } | Gets/sets the type of cell value. |
| [Value](../../aspose.cells/cellvalue/value/) { get; set; } | Gets/sets the cell value. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellValueDemo
{
public static void CellValueExample()
{
// Create a new workbook and get the first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a CellValue instance
CellValue cellValue = new CellValue();
// Set the type and value of the cell
cellValue.Type = CellValueType.IsNumeric;
cellValue.Value = 123.45;
// Assign the CellValue to a cell in the worksheet
Cell cell = worksheet.Cells["A1"];
cell.PutValue(cellValue.Value);
// Save the workbook
workbook.Save("CellValueExample.xlsx");
workbook.Save("CellValueExample.pdf");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
