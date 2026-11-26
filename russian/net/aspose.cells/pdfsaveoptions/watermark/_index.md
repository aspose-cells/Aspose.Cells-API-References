---
title: "PdfSaveOptions.Watermark"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PdfSaveOptions. Получает или задает водяной знак для вывода"
type: docs
url: /ru/net/aspose.cells/pdfsaveoptions/watermark/
---
## PdfSaveOptions.Watermark property

Получает или задаёт водяной знак для вывода.

```csharp
public RenderingWatermark Watermark { get; set; }
```

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyWatermarkDemo
    {
        public static void Run()
        {
            // Создайте рабочую книгу с 3 листами
            Workbook wb = new Workbook();
            wb.Worksheets[0].Cells["A1"].PutValue("Page1");
            int index = wb.Worksheets.Add();
            wb.Worksheets[index].Cells["A1"].PutValue("Page2");
            index = wb.Worksheets.Add();
            wb.Worksheets[index].Cells["A1"].PutValue("Page3");

            // Создайте шрифт водяного знака
            RenderingFont font = new RenderingFont("Calibri", 68);
            font.Italic = true;
            font.Bold = true;
            font.Color = Color.Blue;

            // Создайте водяной знак с текстом и шрифтом
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);
            watermark.HAlignment = TextAlignmentType.Center;
            watermark.VAlignment = TextAlignmentType.Center;
            watermark.Rotation = 45;
            watermark.Opacity = 0.3f;
            watermark.ScaleToPagePercent = 75;

            // Установите водяной знак в параметрах сохранения PDF
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark;

            // Сохраните рабочую книгу с водяным знаком
            wb.Save("output_watermark.pdf", options);
        }
    }
}
```

### См. также

* class [RenderingWatermark](../../../aspose.cells.rendering/renderingwatermark/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


