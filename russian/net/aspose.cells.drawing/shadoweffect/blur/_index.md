---
title: "ShadowEffect.Blur"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ShadowEffect. Получает и задает размытие тени. Диапазон от 0 до 100 пунктов"
type: docs
url: /ru/net/aspose.cells.drawing/shadoweffect/blur/
---
## ShadowEffect.Blur property

Получает и задает размытие тени. Диапазон от 0 до 100 пунктов.

```csharp
public double Blur { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertyBlurDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерную фигуру
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            
            // Получите эффект тени
            ShadowEffect shadow = shape.ShadowEffect;
            
            // Задайте свойства тени, включая Blur
            shadow.Angle = 150;
            shadow.Blur = 30;
            shadow.Size = 1.3;
            shadow.Transparency = 0.4;
            shadow.Distance = 80;
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Shadow effect with blur applied successfully.");
        }
    }
}
```

### См. также

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


