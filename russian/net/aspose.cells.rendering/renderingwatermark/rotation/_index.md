---
title: "RenderingWatermark.Rotation"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RenderingWatermark. Получает или задает вращение водяного знака в градусах"
type: docs
url: /ru/net/aspose.cells.rendering/renderingwatermark/rotation/
---
## RenderingWatermark.Rotation property

Получает или задает вращение водяного знака в градусах.

```csharp
public float Rotation { get; set; }
```

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyRotationDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample data for watermark demo");

            // Создать шрифт для водяного знака
            RenderingFont font = new RenderingFont("Arial", 72);
            font.Color = Color.FromArgb(128, 0, 0, 255);
            font.Bold = true;

            // Создать водяной знак с вращением
            RenderingWatermark watermark = new RenderingWatermark("ROTATED WATERMARK", font);
            watermark.Rotation = 45; // 45 degree rotation
            watermark.Opacity = 0.5f;
            watermark.IsBackground = true;

            // Установить параметры сохранения PDF с водяным знаком
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark;

            // Сохранить с водяным знаком
            workbook.Save("WatermarkRotationDemo.pdf", options);
        }
    }
}
```

### См. также

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


