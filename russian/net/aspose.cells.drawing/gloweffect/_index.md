---
title: "Класс GlowEffect"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.GlowEffect. Этот класс определяет эффект свечения, при котором цветная размазанная обводка добавляется за пределами краёв объекта"
type: docs
url: /ru/net/aspose.cells.drawing/gloweffect/
---
## GlowEffect class

Этот класс задает эффект свечения, при котором вокруг объекта добавляется размытая цветная обводка.

```csharp
public class GlowEffect
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Color](../../aspose.cells.drawing/gloweffect/color/) { get; set; } | Получает цвет эффекта свечения. |
| [Radius](../../aspose.cells.drawing/gloweffect/radius/) { get; set; } | (**Obsolete.**) Получает и задает радиус свечения в единицах пунктов. |
| [Size](../../aspose.cells.drawing/gloweffect/size/) { get; set; } | Получает и задает радиус свечения в единицах пунктов. |
| [Transparency](../../aspose.cells.drawing/gloweffect/transparency/) { get; set; } | Получает и задает степень прозрачности эффекта свечения. Диапазон от 0.0 (непрозрачно) до 1.0 (прозрачно). |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GlowEffectDemo
    {
        public static void GlowEffectExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте форму дуги в лист
            ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);

            // Установить расположение дуги
            arcShape.Placement = PlacementType.FreeFloating;

            // Установить формат заливки
            arcShape.Fill.FillType = FillType.Solid;
            arcShape.Fill.SolidFill.Color = Color.Blue;

            // Установить стиль линии
            arcShape.Line.CompoundType = MsoLineStyle.Single;
            arcShape.Line.Weight = 2;
            arcShape.Line.FillType = FillType.Solid;
            arcShape.Line.SolidFill.Color = Color.Red;
            arcShape.Line.DashStyle = MsoLineDashStyle.Solid;

            // Создать экземпляр GlowEffect и установить его свойства
            GlowEffect glowEffect = arcShape.Glow;
            glowEffect.Color = workbook.CreateCellsColor();
            glowEffect.Color.Color = Color.Yellow;
            glowEffect.Radius = 10.0;
            glowEffect.Transparency = 0.5;

            // Сохраните книгу
            workbook.Save("GlowEffectExample.xlsx");
            workbook.Save("GlowEffectExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


