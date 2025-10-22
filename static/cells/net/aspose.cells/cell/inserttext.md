##Cell.InsertText
Cell method. Insert some characters to the cell. If the cell is rich formatted this method could keep the original formatting
## Cell.InsertText method
Insert some characters to the cell. If the cell is rich formatted, this method could keep the original formatting.
```csharp
public void InsertText(int index, string text)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The index. |
| text | String | Inserted text. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodInsertTextWithInt32StringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Access cell B3 and set initial value
Cell cell = worksheet.Cells["B3"];
cell.PutValue("OriginalText");
// Insert text at position 6
cell.InsertText(6, "Inserted");
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
