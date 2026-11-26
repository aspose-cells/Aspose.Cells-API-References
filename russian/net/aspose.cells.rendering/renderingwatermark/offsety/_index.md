---
title: "RenderingWatermark.OffsetY"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RenderingWatermark. Получает или задает значение смещения для VAlignment"
type: docs
url: /ru/net/aspose.cells.rendering/renderingwatermark/offsety/
---
## RenderingWatermark.OffsetY property

Получает или задает значение смещения для [`VAlignment`](../valignment/)

```csharp
public float OffsetY { get; set; }
```

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyOffsetYDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue("OffsetY Demo");

            // Создайте шрифт водяного знака
            RenderingFont font = new RenderingFont("Arial", 24)
            {
                Color = Color.Red,
                Bold = true
            };

            // Создать водяной знак с разными значениями OffsetY
            RenderingWatermark watermark = new RenderingWatermark("VERTICAL OFFSET", font)
            {
                Rotation = 0,
                Opacity = 0.3f,
                IsBackground = true,
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                OffsetX = 0,
                OffsetY = 100 // Demonstrating OffsetY property
            };

            // Установить параметры сохранения с водяным знаком
            PdfSaveOptions options = new PdfSaveOptions
            {
                Watermark = watermark
            };

            // Сохранить с смещением водяного знака
            workbook.Save("WatermarkOffsetYDemo.pdf", options);
        }
    }
}
```

### См. также

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


