##Enum TextDirectionType
Aspose.Cells.TextDirectionType enum. Represents the direction of the text flow for this paragraph
## TextDirectionType enumeration
Represents the direction of the text flow for this paragraph.
```csharp
public enum TextDirectionType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Context | `0` |  |
| LeftToRight | `1` |  |
| RightToLeft | `2` |  |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassTextDirectionTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set RightToLeft text direction
Style style = cells["A1"].GetStyle();
style.TextDirection = TextDirectionType.RightToLeft;
cells["A1"].SetStyle(style);
cells["A1"].PutValue("Right to Left Text");
// Set LeftToRight text direction
style = cells["A2"].GetStyle();
style.TextDirection = TextDirectionType.LeftToRight;
cells["A2"].SetStyle(style);
cells["A2"].PutValue("Left to Right Text");
// Set Context text direction
style = cells["A3"].GetStyle();
style.TextDirection = TextDirectionType.Context;
cells["A3"].SetStyle(style);
cells["A3"].PutValue("Context Text Direction");
workbook.Save("TextDirectionTypeDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
