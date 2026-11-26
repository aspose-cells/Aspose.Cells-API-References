---
title: "Класс ShadowEffect"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.ShadowEffect. Этот класс задает эффект тени элемента диаграммы или фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/shadoweffect/
---
## ShadowEffect class

Этот класс задает эффект тени элемента диаграммы или фигуры.

```csharp
public class ShadowEffect
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Angle](../../aspose.cells.drawing/shadoweffect/angle/) { get; set; } | Получает и задает угол освещения. Диапазон от 0 до 359,9 градусов. |
| [Blur](../../aspose.cells.drawing/shadoweffect/blur/) { get; set; } | Получает и задает размытие тени. Диапазон от 0 до 100 пунктов. |
| [Color](../../aspose.cells.drawing/shadoweffect/color/) { get; set; } | Получает и задает цвет тени. |
| [Distance](../../aspose.cells.drawing/shadoweffect/distance/) { get; set; } | Получает и задает расстояние тени. Диапазон от 0 до 200 пунктов. |
| [PresetType](../../aspose.cells.drawing/shadoweffect/presettype/) { get; set; } | Получает и задает предустановленный тип тени. |
| [Size](../../aspose.cells.drawing/shadoweffect/size/) { get; set; } | Получает и задает размер тени. Диапазон от 0 до 2,0. Не имеет смысла для внутренней тени. |
| [Transparency](../../aspose.cells.drawing/shadoweffect/transparency/) { get; set; } | Получает и задает степень прозрачности тени. Диапазон от 0,0 (непрозрачный) до 1,0 (прозрачный). |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShadowEffectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образец фигуры со всеми необходимыми параметрами
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 100);

            // Получите эффект тени фигуры
            ShadowEffect shadow = shape.ShadowEffect;

            // Установите свойства тени
            shadow.Angle = 150;
            shadow.Blur = 30;
            shadow.Size = 1.3;
            shadow.Transparency = 0.4;
            shadow.Distance = 80;

            // Сохраните книгу
            workbook.Save("output.xlsx");

            Console.WriteLine("Shadow effect demo completed successfully.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


