##Enum AutoFillType
Aspose.Cells.AutoFillType enum. Represents the auto fill type
## AutoFillType enumeration
Represents the auto fill type.
```csharp
public enum AutoFillType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Copy | `1` | Copies the value and format of the source area to the target area |
| Default | `0` | Automatically fills the target area with the value and format. |
| Formats | `3` | Copies only the format of the source area to the target area, |
| Series | `2` | Extend the value in the source area to the target area in the form of a series and copy format to the target area. |
| Values | `4` | Copies only the value of the source area to the target area, |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class AutoFillTypeDemo
{
public static void AutoFillTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create a range (A1:A10) and fill it with some values
Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1:A10");
for (int i = 0; i < 10; i++)
{
sourceRange[i, 0].PutValue(i + 1);
}
// Create a target range (B1:B10)
Aspose.Cells.Range targetRange = worksheet.Cells.CreateRange("B1:B10");
//Series type error, ticket has been created
// Use AutoFill method with AutoFillType.Series to fill the target range
//sourceRange.AutoFill(targetRange, AutoFillType.Series);
// Use AutoFill method with AutoFillType.Copy to fill the target range
sourceRange.AutoFill(targetRange, AutoFillType.Copy);
// Save the workbook
workbook.Save("AutoFillTypeExample.xlsx");
workbook.Save("AutoFillTypeExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
