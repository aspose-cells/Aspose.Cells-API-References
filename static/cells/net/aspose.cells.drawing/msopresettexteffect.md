##Enum MsoPresetTextEffect
Aspose.Cells.Drawing.MsoPresetTextEffect enum. Represents preset text effect type of WordArt
## MsoPresetTextEffect enumeration
Represents preset text effect type of WordArt.
```csharp
public enum MsoPresetTextEffect
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| TextEffect1 | `0` | TextEffect1 |
| TextEffect2 | `1` | TextEffect2 |
| TextEffect3 | `2` | TextEffect3 |
| TextEffect4 | `3` | TextEffect4 |
| TextEffect5 | `4` | TextEffect5 |
| TextEffect6 | `5` | TextEffect6 |
| TextEffect7 | `6` | TextEffect7 |
| TextEffect8 | `7` | TextEffect8 |
| TextEffect9 | `8` | TextEffect9 |
| TextEffect10 | `9` | TextEffect10 |
| TextEffect11 | `10` | TextEffect11 |
| TextEffect12 | `11` | TextEffect12 |
| TextEffect13 | `12` | TextEffect13 |
| TextEffect14 | `13` | TextEffect14 |
| TextEffect15 | `14` | TextEffect15 |
| TextEffect16 | `15` | TextEffect16 |
| TextEffect17 | `16` | TextEffect17 |
| TextEffect18 | `17` | TextEffect18 |
| TextEffect19 | `18` | TextEffect19 |
| TextEffect20 | `19` | TextEffect20 |
| TextEffect21 | `20` | TextEffect21 |
| TextEffect22 | `21` | TextEffect22 |
| TextEffect23 | `22` | TextEffect23 |
| TextEffect24 | `23` | TextEffect24 |
| TextEffect25 | `24` | TextEffect25 |
| TextEffect26 | `25` | TextEffect26 |
| TextEffect27 | `26` | TextEffect27 |
| TextEffect28 | `27` | TextEffect28 |
| TextEffect29 | `28` | TextEffect29 |
| TextEffect30 | `29` | TextEffect30 |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class DrawingClassMsoPresetTextEffectDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
Shape shape = sheet.Shapes.AddTextEffect(
MsoPresetTextEffect.TextEffect1,
"CONFIDENTIAL",
"Arial Black",
50,
false,
true,
0, 0, 0, 0, 130, 800);
shape.Font.Underline = FontUnderlineType.Single;
shape.Font.Color = System.Drawing.Color.Red;
wb.Save("MsoPresetTextEffectDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
