---
title: "RenderingWatermark.IsBackground"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RenderingWatermark. Указывает, размещён ли водяной знак за содержимым страницы"
type: docs
url: /ru/net/aspose.cells.rendering/renderingwatermark/isbackground/
---
## RenderingWatermark.IsBackground property

Указывает, размещён ли водяной знак за содержимым страницы.

```csharp
public bool IsBackground { get; set; }
```

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyIsBackgroundDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue("Sample Content");

            // Создать водяной знак с IsBackground, установленным в true
            RenderingFont font = new RenderingFont("Arial", 36)
            {
                Color = Color.LightGray
            };
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font)
            {
                IsBackground = true,
                Rotation = 45,
                Opacity = 0.2f
            };

            // Настроить параметры сохранения с водяным знаком
            PdfSaveOptions options = new PdfSaveOptions
            {
                Watermark = watermark
            };

            // Сохранить с фоновым водяным знаком
            workbook.Save("WatermarkIsBackgroundDemo.pdf", options);
        }
    }
}
```

### См. также

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


