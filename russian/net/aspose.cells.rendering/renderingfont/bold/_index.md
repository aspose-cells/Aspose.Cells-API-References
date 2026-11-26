---
title: "RenderingFont.Bold"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RenderingFont. Получает или задает полужирный стиль для шрифта"
type: docs
url: /ru/net/aspose.cells.rendering/renderingfont/bold/
---
## RenderingFont.Bold property

Получает или задает полужирное начертание для шрифта.

```csharp
public bool Bold { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingFontPropertyBoldDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Bold Font Example");

            // Создать стиль для ячейки
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            worksheet.Cells["A1"].SetStyle(style);

            // Создать параметры сохранения PDF с водяным знаком, демонстрирующим жирный шрифт
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Создать шрифт рендеринга с жирным свойством
            RenderingFont font = new RenderingFont("Arial", 36)
            {
                Bold = true,
                Color = System.Drawing.Color.Red
            };
            
            // Создать водяной знак с жирным шрифтом
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font)
            {
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                Opacity = 0.3f
            };
            pdfSaveOptions.Watermark = watermark;

            // Сохраните книгу
            workbook.Save("BoldFontExample.pdf", pdfSaveOptions);
        }
    }
}
```

### См. также

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


