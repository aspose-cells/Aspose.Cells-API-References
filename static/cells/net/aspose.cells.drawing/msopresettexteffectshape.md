##Enum MsoPresetTextEffectShape
Aspose.Cells.Drawing.MsoPresetTextEffectShape enum. Represents preset text effect shape type of WordArt
## MsoPresetTextEffectShape enumeration
Represents preset text effect shape type of WordArt.
```csharp
public enum MsoPresetTextEffectShape
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| PlainText | `136` | PlainText |
| Stop | `137` | Stop |
| TriangleUp | `138` | TriangleUp |
| TriangleDown | `139` | TriangleDown |
| ChevronUp | `140` | ChevronUp |
| ChevronDown | `141` | ChevronDown |
| RingInside | `142` | RingInside |
| RingOutside | `143` | RingOutside |
| ArchUpCurve | `144` | ArchUpCurve |
| ArchDownCurve | `145` | ArchDownCurve |
| CircleCurve | `146` | CircleCurve |
| ButtonCurve | `147` | ButtonCurve |
| ArchUpPour | `148` | ArchUpPour |
| ArchDownPour | `149` | ArchDownPour |
| CirclePour | `150` | CirclePour |
| ButtonPour | `151` | ButtonPour |
| CurveUp | `152` | CurveUp |
| CurveDown | `153` | CurveDown |
| CanUp | `174` | CanUp |
| CanDown | `175` | CanDown |
| Wave1 | `156` | Wave1 |
| Wave2 | `157` | Wave2 |
| DoubleWave1 | `158` | DoubleWave1 |
| DoubleWave2 | `159` | DoubleWave2 |
| Inflate | `160` | Inflate |
| Deflate | `161` | Deflate |
| InflateBottom | `162` | InflateBottom |
| DeflateBottom | `163` | DeflateBottom |
| InflateTop | `164` | InflateTop |
| DeflateTop | `165` | DeflateTop |
| DeflateInflate | `166` | DeflateInflate |
| DeflateInflateDeflate | `167` | DeflateInflateDeflate |
| FadeRight | `168` | FadeRight |
| FadeLeft | `169` | FadeLeft |
| FadeUp | `170` | FadeUp |
| FadeDown | `171` | FadeDown |
| SlantUp | `172` | SlantUp |
| SlantDown | `173` | SlantDown |
| CascadeUp | `154` | CascadeUp |
| CascadeDown | `155` | CascadeDown |
| Mixed | `255` | Mixed |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class MsoPresetTextEffectShapeDemo
{
public static void MsoPresetTextEffectShapeExample()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
ShapeCollection shapes = worksheet.Shapes;
// Adding a WordArt text effect shape
shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Aspose", "Arial", 30, false, false, 0, 0, 0, 0, 100, 200);
TextEffectFormat textEffectFormat = shapes[0].TextEffect;
// Setting the preset shape type
textEffectFormat.PresetShape = MsoPresetTextEffectShape.ArchUpCurve;
// Save the workbook
workbook.Save("MsoPresetTextEffectShapeExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
