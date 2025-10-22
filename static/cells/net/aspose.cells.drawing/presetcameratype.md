##Enum PresetCameraType
Aspose.Cells.Drawing.PresetCameraType enum. Represent different algorithmic methods for setting all camera properties including position
## PresetCameraType enumeration
Represent different algorithmic methods for setting all camera properties, including position.
```csharp
public enum PresetCameraType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| IsometricBottomDown | `0` |  |
| IsometricBottomUp | `1` |  |
| IsometricLeftDown | `2` |  |
| IsometricLeftUp | `3` |  |
| IsometricOffAxis1Left | `4` |  |
| IsometricOffAxis1Right | `5` |  |
| IsometricOffAxis1Top | `6` |  |
| IsometricOffAxis2Left | `7` |  |
| IsometricOffAxis2Right | `8` |  |
| IsometricOffAxis2Top | `9` |  |
| IsometricOffAxis3Bottom | `10` |  |
| IsometricOffAxis3Left | `11` |  |
| IsometricOffAxis3Right | `12` |  |
| IsometricOffAxis4Bottom | `13` |  |
| IsometricOffAxis4Left | `14` |  |
| IsometricOffAxis4Right | `15` |  |
| IsometricRightDown | `16` |  |
| IsometricRightUp | `17` |  |
| IsometricTopDown | `18` |  |
| IsometricTopUp | `19` |  |
| LegacyObliqueBottom | `20` |  |
| LegacyObliqueBottomLeft | `21` |  |
| LegacyObliqueBottomRight | `22` |  |
| LegacyObliqueFront | `23` |  |
| LegacyObliqueLeft | `24` |  |
| LegacyObliqueRight | `25` |  |
| LegacyObliqueTop | `26` |  |
| LegacyObliqueTopLeft | `27` |  |
| LegacyObliqueTopRight | `28` |  |
| LegacyPerspectiveBottom | `29` |  |
| LegacyPerspectiveBottomLeft | `30` |  |
| LegacyPerspectiveBottomRight | `31` |  |
| LegacyPerspectiveFront | `32` |  |
| LegacyPerspectiveLeft | `33` |  |
| LegacyPerspectiveRight | `34` |  |
| LegacyPerspectiveTop | `35` |  |
| LegacyPerspectiveTopLeft | `36` |  |
| LegacyPerspectiveTopRight | `37` |  |
| ObliqueBottom | `38` |  |
| ObliqueBottomLeft | `39` |  |
| ObliqueBottomRight | `40` |  |
| ObliqueLeft | `41` |  |
| ObliqueRight | `42` |  |
| ObliqueTop | `43` |  |
| ObliqueTopLeft | `44` |  |
| ObliqueTopRight | `45` |  |
| OrthographicFront | `46` |  |
| PerspectiveAbove | `47` |  |
| PerspectiveAboveLeftFacing | `48` |  |
| PerspectiveAboveRightFacing | `49` |  |
| PerspectiveBelow | `50` |  |
| PerspectiveContrastingLeftFacing | `51` |  |
| PerspectiveContrastingRightFacing | `52` |  |
| PerspectiveFront | `53` |  |
| PerspectiveHeroicExtremeLeftFacing | `54` |  |
| PerspectiveHeroicExtremeRightFacing | `55` |  |
| PerspectiveHeroicLeftFacing | `56` |  |
| PerspectiveHeroicRightFacing | `57` |  |
| PerspectiveLeft | `58` |  |
| PerspectiveRelaxed | `59` |  |
| PerspectiveRelaxedModerately | `60` |  |
| PerspectiveRight | `61` |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class DrawingClassPresetCameraTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to apply camera preset
Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 300, 200, 0, 0);
// Set 3D format properties with different preset camera types
shape.ThreeDFormat.PresetCameraType = PresetCameraType.IsometricLeftUp;
shape.ThreeDFormat.LightAngle = 45;
shape.ThreeDFormat.LightingDirection = LightRigDirectionType.Top;
shape.ThreeDFormat.Z = 10;
// Create another shape with different camera preset
Shape shape2 = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 10, 300, 200, 0, 0);
shape2.ThreeDFormat.PresetCameraType = PresetCameraType.PerspectiveHeroicRightFacing;
shape2.ThreeDFormat.ContourWidth = 5;
shape2.ThreeDFormat.ExtrusionHeight = 30;
// Save the workbook
workbook.Save("PresetCameraTypeDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
