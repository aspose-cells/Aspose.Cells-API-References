---
title: "Класс RenderingFont"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Rendering.RenderingFont. Шрифт для рендеринга"
type: docs
url: /ru/net/aspose.cells.rendering/renderingfont/
---
## RenderingFont class

Шрифт для рендеринга.

```csharp
public class RenderingFont
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [RenderingFont](renderingfont/)(string, float) | Инициализирует новый экземпляр `RenderingFont` |

## Свойства

| Имя | Описание |
| --- | --- |
| [Bold](../../aspose.cells.rendering/renderingfont/bold/) { get; set; } | Получает или задает полужирное начертание для шрифта. |
| [Color](../../aspose.cells.rendering/renderingfont/color/) { get; set; } | Получает или задает цвет шрифта. |
| [Italic](../../aspose.cells.rendering/renderingfont/italic/) { get; set; } | Получает или задает курсив для шрифта. |
| [Name](../../aspose.cells.rendering/renderingfont/name/) { get; } | Получает имя шрифта. |
| [Size](../../aspose.cells.rendering/renderingfont/size/) { get; } | Получает размер шрифта в пунктах. |

### Примеры

```csharp
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingFontDemo
    {
        public static void RenderingFontExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            sheet.Cells["A1"].PutValue("Hello World!");

            // Создать объект RenderingFont
            RenderingFont renderingFont = new RenderingFont("Arial", 12)
            {
                Bold = true,
                Italic = true,
                Color = Color.Blue
            };

            // Создать объект RenderingWatermark, используя RenderingFont
            RenderingWatermark watermark = new RenderingWatermark("Sample Watermark", renderingFont)
            {
                Rotation = 45,
                ScaleToPagePercent = 100,
                Opacity = 0.5f,
                IsBackground = true,
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                OffsetX = 0,
                OffsetY = 0
            };

            // Создать PdfSaveOptions и установить водяной знак
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions
            {
                Watermark = watermark,
                EmbedStandardWindowsFonts = true,
                CalculateFormula = true,
                ExportDocumentStructure = true,
                DisplayDocTitle = true
            };

            // Сохранить книгу в PDF с водяным знаком
            workbook.Save("RenderingFontExample.pdf", pdfSaveOptions);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


