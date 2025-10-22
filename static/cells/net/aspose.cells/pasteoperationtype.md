##Enum PasteOperationType
Aspose.Cells.PasteOperationType enum. Represents operation type when pasting range
## PasteOperationType enumeration
Represents operation type when pasting range.
```csharp
public enum PasteOperationType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | No operation. |
| Add | `1` | Add |
| Subtract | `2` | Subtract |
| Multiply | `3` | Multiply |
| Divide | `4` | Divide |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassPasteOperationTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data to cells
sheet.Cells["A1"].PutValue(10);
sheet.Cells["B1"].PutValue(20);
sheet.Cells["C1"].PutValue(30);
// Create paste options with PasteOperationType.None
var pasteOptions = new PasteOptions()
{
PasteType = PasteType.Values,
OperationType = PasteOperationType.None,
SkipBlanks = false,
Transpose = false
};
// Create range and copy with paste options
Aspose.Cells.Range sourceRange = sheet.Cells.CreateRange("A1", "C1");
Aspose.Cells.Range destRange = sheet.Cells.CreateRange("A2", "C2");
sourceRange.Copy(destRange, pasteOptions);
// Save the workbook
workbook.Save("PasteOperationTypeDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
