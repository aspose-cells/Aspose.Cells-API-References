##Enum CopyFormatType
Aspose.Cells.CopyFormatType enum. Represents type of copying format when inserting rows
## CopyFormatType enumeration
Represents type of copying format when inserting rows.
```csharp
public enum CopyFormatType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| SameAsAbove | `0` | Formats same as above row. |
| SameAsBelow | `1` | Formats same as below row. |
| Clear | `2` | Clears formatting. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CopyFormatTypeDemo
{
public static void CopyFormatTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Fill some data in the worksheet
worksheet.Cells["A1"].PutValue("Header1");
worksheet.Cells["A2"].PutValue("Data1");
worksheet.Cells["A3"].PutValue("Data2");
// Create InsertOptions and set CopyFormatType
InsertOptions insertOptions = new InsertOptions();
insertOptions.CopyFormatType = CopyFormatType.SameAsAbove;
// Insert a row at the second position with the specified format type
worksheet.Cells.InsertRows(1, 1, insertOptions);
// Save the workbook
workbook.Save("CopyFormatTypeExample.xlsx");
workbook.Save("CopyFormatTypeExample.pdf");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
