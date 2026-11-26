---
title: "RenderingWatermark.HAlignment"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RenderingWatermark. Получает или задает горизонтальное выравнивание водяного знака относительно страницы"
type: docs
url: /ru/net/aspose.cells.rendering/renderingwatermark/halignment/
---
## RenderingWatermark.HAlignment property

Получает или задает горизонтальное выравнивание водяного знака относительно страницы.

```csharp
public TextAlignmentType HAlignment { get; set; }
```

### Примечания

Допустимы только Left, Center, Right. По умолчанию — Left.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyHAlignmentDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Watermark HAlignment Demo");

            // Создайте параметры сохранения PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Создать и настроить водяной знак с разными настройками HAlignment
            RenderingFont font = new RenderingFont("Arial", 48)
            {
                Bold = true,
                Color = System.Drawing.Color.Blue
            };

            // Создать водяной знак с выравниванием по Center
            RenderingWatermark watermark = new RenderingWatermark("CENTER ALIGNED", font)
            {
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                Opacity = 0.5f
            };
            pdfSaveOptions.Watermark = watermark;

            // Сохранить с центрированным водяным знаком
            workbook.Save("WatermarkCenterAlignment.pdf", pdfSaveOptions);

            // Изменить на выравнивание Left
            watermark.HAlignment = TextAlignmentType.Left;
            workbook.Save("WatermarkLeftAlignment.pdf", pdfSaveOptions);

            // Изменить на выравнивание Right
            watermark.HAlignment = TextAlignmentType.Right;
            workbook.Save("WatermarkRightAlignment.pdf", pdfSaveOptions);
        }
    }
}
```

### См. также

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


