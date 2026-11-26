---
title: "ShadowEffect.Transparency"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ShadowEffect. Получает и задает степень прозрачности тени. Диапазон от 0.0 — непрозрачный до 1.0 — полностью прозрачный"
type: docs
url: /ru/net/aspose.cells.drawing/shadoweffect/transparency/
---
## ShadowEffect.Transparency property

Получает и задает степень прозрачности тени. Диапазон от 0,0 (непрозрачный) до 1,0 (прозрачный).

```csharp
public double Transparency { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте форму, чтобы продемонстрировать эффект тени
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            
            // Получите эффект тени и задайте свойства, включая Transparency
            ShadowEffect shadow = shape.ShadowEffect;
            shadow.Angle = 150;
            shadow.Blur = 30;
            shadow.Size = 1.3;
            shadow.Transparency = 0.4; // Setting transparency to 40%
            shadow.Distance = 80;
            
            // Сохраните книгу
            workbook.Save("ShadowEffectDemo.xlsx");
            
            Console.WriteLine("Workbook saved with shadow effect transparency set to 0.4");
        }
    }
}
```

### См. также

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


