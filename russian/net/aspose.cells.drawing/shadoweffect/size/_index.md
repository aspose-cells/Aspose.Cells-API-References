---
title: "ShadowEffect.Size"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ShadowEffect. Получает и задает размер тени. Диапазон от 0 до 2.0. Не имеет смысла во внутренней тени"
type: docs
url: /ru/net/aspose.cells.drawing/shadoweffect/size/
---
## ShadowEffect.Size property

Получает и задает размер тени. Диапазон от 0 до 2,0. Не имеет смысла для внутренней тени.

```csharp
public double Size { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertySizeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook book = new Workbook();
            
            // Получите доступ к первому листу и добавьте форму
            Worksheet sheet = book.Worksheets[0];
            Shape shape = sheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Получите эффект тени и задайте свойства, включая Size
            ShadowEffect shadow = shape.ShadowEffect;
            shadow.Angle = 150;
            shadow.Blur = 30;
            shadow.Size = 1.3; // Demonstrating Size property usage
            shadow.Transparency = 0.4;
            shadow.Distance = 80;

            // Сохраните книгу
            book.Save("ShadowEffectExample.xlsx");
            
            Console.WriteLine("Shadow effect with Size property set to 1.3 has been applied.");
        }
    }
}
```

### См. также

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


