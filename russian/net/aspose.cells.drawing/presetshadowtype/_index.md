---
title: "Перечисление PresetShadowType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.PresetShadowType enum. Представляет предустановленный тип тени"
type: docs
url: /ru/net/aspose.cells.drawing/presetshadowtype/
---
## PresetShadowType enumeration

Представляет тип предустановленной тени.

```csharp
public enum PresetShadowType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| NoShadow | `0` | Без тени. |
| Custom | `1` | Пользовательская тень. |
| OffsetDiagonalBottomRight | `2` | Внешнее смещение тени по диагонали вниз вправо. |
| OffsetBottom | `3` | Внешнее смещение тени вниз. |
| OffsetDiagonalBottomLeft | `4` | Внешнее смещение тени по диагонали снизу слева. |
| OffsetRight | `5` | Внешнее смещение тени вправо. |
| OffsetCenter | `6` | Внешнее смещение тени по центру. |
| OffsetLeft | `7` | Внешнее смещение тени влево. |
| OffsetDiagonalTopRight | `8` | Внешнее смещение тени по диагонали сверху справа. |
| OffsetTop | `9` | Внешнее смещение тени вверх. |
| OffsetDiagonalTopLeft | `10` | Внешнее смещение тени по диагонали сверху слева. |
| InsideDiagonalTopLeft | `11` | Внутренняя тень внутри по диагонали сверху слева. |
| InsideTop | `12` | Внутренняя тень внутри сверху. |
| InsideDiagonalTopRight | `13` | Внутренняя тень внутри по диагонали сверху справа. |
| InsideLeft | `14` | Внутренняя тень внутри слева. |
| InsideCenter | `15` | Внутренняя тень внутри по центру. |
| InsideRight | `16` | Внутренняя тень внутри справа. |
| InsideDiagonalBottomLeft | `17` | Внутренняя тень внутри по диагонали снизу слева. |
| InsideBottom | `18` | Внутренняя тень внутри снизу. |
| InsideDiagonalBottomRight | `19` | Внутренняя тень внутри по диагонали снизу справа. |
| PerspectiveDiagonalUpperLeft | `20` | Внешняя тень в перспективе по диагонали сверху слева. |
| PerspectiveDiagonalUpperRight | `21` | Внешняя тень в перспективе по диагонали сверху справа. |
| Below | `22` | Внешняя тень снизу. |
| PerspectiveDiagonalLowerLeft | `23` | Внешняя тень в перспективе по диагонали снизу слева. |
| PerspectiveDiagonalLowerRight | `24` | Внешняя тень в перспективе по диагонали снизу справа. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassPresetShadowTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте форму, чтобы продемонстрировать эффекты тени
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            
            // Установите разные предустановленные типы теней
            shape.ShadowEffect.PresetType = PresetShadowType.OffsetDiagonalBottomRight;
            Console.WriteLine("Shadow type set to: " + shape.ShadowEffect.PresetType);

            // Перейдите к другому типу тени
            shape.ShadowEffect.PresetType = PresetShadowType.OffsetBottom;
            Console.WriteLine("Shadow type changed to: " + shape.ShadowEffect.PresetType);

            // Сохраните книгу
            workbook.Save("PresetShadowTypeDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


