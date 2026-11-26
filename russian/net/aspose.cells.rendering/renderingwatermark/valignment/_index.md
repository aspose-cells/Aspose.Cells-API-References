---
title: "RenderingWatermark.VAlignment"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RenderingWatermark. Получает или задает вертикальное выравнивание водяного знака относительно страницы"
type: docs
url: /ru/net/aspose.cells.rendering/renderingwatermark/valignment/
---
## RenderingWatermark.VAlignment property

Получает или задает вертикальное выравнивание водяного знака относительно страницы.

```csharp
public TextAlignmentType VAlignment { get; set; }
```

### Примечания

Допустимы только Top, Center, Bottom. По умолчанию Top.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyVAlignmentDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Watermark VAlignment Demo");

            // Создайте параметры сохранения PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Создать и настроить водяной знак с различными настройками VAlignment
            RenderingFont font = new RenderingFont("Arial", 48)
            {
                Bold = true,
                Color = System.Drawing.Color.Red
            };

            // Создать водяной знак с вертикальным выравниванием, установленным в Center
            RenderingWatermark watermark = new RenderingWatermark("CENTER ALIGNED", font)
            {
                VAlignment = TextAlignmentType.Center,
                HAlignment = TextAlignmentType.Center,
                Opacity = 0.5f
            };
            pdfSaveOptions.Watermark = watermark;

            // Сохранить книгу с водяным знаком
            workbook.Save("WatermarkVAlignmentDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### См. также

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


