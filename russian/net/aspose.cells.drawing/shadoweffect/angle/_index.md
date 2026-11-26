---
title: "ShadowEffect.Angle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ShadowEffect. Получает и задает угол освещения. Диапазон от 0 до 359.9 градусов"
type: docs
url: /ru/net/aspose.cells.drawing/shadoweffect/angle/
---
## ShadowEffect.Angle property

Получает и задает угол освещения. Диапазон от 0 до 359,9 градусов.

```csharp
public double Angle { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertyAngleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте форму и задайте угол эффекта тени
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
            shape.ShadowEffect.Angle = 45;

            // Проверьте и выведите значение угла
            Console.WriteLine("Shadow Effect Angle: " + shape.ShadowEffect.Angle);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


