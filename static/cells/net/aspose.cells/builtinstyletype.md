##Enum BuiltinStyleType
Aspose.Cells.BuiltinStyleType enum. Represents all builtin style types
## BuiltinStyleType enumeration
Represents all built-in style types.
```csharp
public enum BuiltinStyleType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| TwentyPercentAccent1 | `30` |  |
| TwentyPercentAccent2 | `34` |  |
| TwentyPercentAccent3 | `38` |  |
| TwentyPercentAccent4 | `42` |  |
| TwentyPercentAccent5 | `46` |  |
| TwentyPercentAccent6 | `50` |  |
| FortyPercentAccent1 | `31` |  |
| FortyPercentAccent2 | `35` |  |
| FortyPercentAccent3 | `39` |  |
| FortyPercentAccent4 | `43` |  |
| FortyPercentAccent5 | `47` |  |
| FortyPercentAccent6 | `51` |  |
| SixtyPercentAccent1 | `32` |  |
| SixtyPercentAccent2 | `36` |  |
| SixtyPercentAccent3 | `40` |  |
| SixtyPercentAccent4 | `44` |  |
| SixtyPercentAccent5 | `48` |  |
| SixtyPercentAccent6 | `52` |  |
| Accent1 | `29` |  |
| Accent2 | `33` |  |
| Accent3 | `37` |  |
| Accent4 | `41` |  |
| Accent5 | `45` |  |
| Accent6 | `49` |  |
| Bad | `27` |  |
| Calculation | `22` |  |
| CheckCell | `23` |  |
| Comma | `3` |  |
| Comma1 | `6` |  |
| Currency | `4` |  |
| Currency1 | `7` |  |
| ExplanatoryText | `53` |  |
| Good | `26` |  |
| Header1 | `16` |  |
| Header2 | `17` |  |
| Header3 | `18` |  |
| Header4 | `19` |  |
| Hyperlink | `8` |  |
| FollowedHyperlink | `9` |  |
| Input | `20` |  |
| LinkedCell | `24` |  |
| Neutral | `28` |  |
| Normal | `0` |  |
| Note | `10` |  |
| Output | `21` |  |
| Percent | `5` |  |
| Title | `15` |  |
| Total | `25` |  |
| WarningText | `11` |  |
| RowLevel | `1` |  |
| ColumnLevel | `2` |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class BuiltinStyleTypeDemo
{
public static void BuiltinStyleTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Apply different built-in styles to cells
Style style;
// Apply Normal style
style = workbook.CreateBuiltinStyle(BuiltinStyleType.Normal);
worksheet.Cells["A1"].SetStyle(style);
worksheet.Cells["A1"].PutValue("Normal Style");
// Apply Title style
style = workbook.CreateBuiltinStyle(BuiltinStyleType.Title);
worksheet.Cells["A2"].SetStyle(style);
worksheet.Cells["A2"].PutValue("Title Style");
// Apply Header1 style
style = workbook.CreateBuiltinStyle(BuiltinStyleType.Header1);
worksheet.Cells["A3"].SetStyle(style);
worksheet.Cells["A3"].PutValue("Header1 Style");
// Apply Currency style
style = workbook.CreateBuiltinStyle(BuiltinStyleType.Currency);
worksheet.Cells["A4"].SetStyle(style);
worksheet.Cells["A4"].PutValue(1234.56);
// Apply Percent style
style = workbook.CreateBuiltinStyle(BuiltinStyleType.Percent);
worksheet.Cells["A5"].SetStyle(style);
worksheet.Cells["A5"].PutValue(0.56);
style = workbook.CreateBuiltinStyle(BuiltinStyleType.FortyPercentAccent1);
worksheet.Cells["A6"].SetStyle(style);
worksheet.Cells["A6"].PutValue(0.5555);
style = workbook.CreateBuiltinStyle(BuiltinStyleType.Accent1);
worksheet.Cells["A7"].SetStyle(style);
worksheet.Cells["A7"].PutValue(0.5555);
style = workbook.CreateBuiltinStyle(BuiltinStyleType.Hyperlink);
worksheet.Cells["A8"].SetStyle(style);
worksheet.Cells["A8"].PutValue(0.5555);
style = workbook.CreateBuiltinStyle(BuiltinStyleType.SixtyPercentAccent1);
worksheet.Cells["A8"].SetStyle(style);
worksheet.Cells["A8"].PutValue(0.5555);
// Save the workbook
workbook.Save("BuiltinStyleTypeExample.xlsx");
workbook.Save("BuiltinStyleTypeExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
