---
title: "ShadowEffect.Distance"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ShadowEffect. Получает и задает расстояние тени. Диапазон от 0 до 200 пунктов"
type: docs
url: /ru/net/aspose.cells.drawing/shadoweffect/distance/
---
## ShadowEffect.Distance property

Получает и задает расстояние тени. Диапазон от 0 до 200 пунктов.

```csharp
public double Distance { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertyDistanceDemo
    {
        public static void Run()
        {
            // Создайте новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную форму
            RectangleShape rectangle = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 150, 100);
            
            // Настройте эффект тени
            ShadowEffect shadow = rectangle.ShadowEffect;
            shadow.PresetType = PresetShadowType.OffsetDiagonalTopRight;
            
            // Создайте объект CellsColor и задайте значения ARGB
            CellsColor color = workbook.CreateCellsColor();
            color.Argb = (128 << 24) | (255 << 16) | (0 << 8) | 0; // Semi-transparent red
            shadow.Color = color;
            
            shadow.Transparency = 0.3;
            shadow.Blur = 15;
            shadow.Angle = 45;
            shadow.Distance = 20; // Set distance to 20 points

            // Отобразите расстояние тени
            Console.WriteLine("Shadow Distance: " + shadow.Distance + " points");

            // Сохраните книгу с эффектом тени
            workbook.Save("ShadowEffectPropertyDistanceDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


