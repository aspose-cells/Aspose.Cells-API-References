---
title: "Перечисление PresetCameraType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.PresetCameraType. Представляет различные алгоритмические методы настройки всех свойств камеры, включая позицию"
type: docs
url: /ru/net/aspose.cells.drawing/presetcameratype/
---
## PresetCameraType enumeration

Представляет различные алгоритмические методы настройки всех свойств камеры, включая позицию.

```csharp
public enum PresetCameraType
```

### Значения

| Имя | Значение | Описание |
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

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте форму для применения предустановки камеры
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 300, 200, 0, 0);

            // Установите свойства 3D-формата с различными типами предустановок камеры
            shape.ThreeDFormat.PresetCameraType = PresetCameraType.IsometricLeftUp;
            shape.ThreeDFormat.LightAngle = 45;
            shape.ThreeDFormat.LightingDirection = LightRigDirectionType.Top;
            shape.ThreeDFormat.Z = 10;

            // Создайте другую форму с другой предустановкой камеры
            Shape shape2 = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 10, 300, 200, 0, 0);
            shape2.ThreeDFormat.PresetCameraType = PresetCameraType.PerspectiveHeroicRightFacing;
            shape2.ThreeDFormat.ContourWidth = 5;
            shape2.ThreeDFormat.ExtrusionHeight = 30;

            // Сохраните книгу
            workbook.Save("PresetCameraTypeDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


