---
title: "RenderingFont.Size"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RenderingFont. Получает размер шрифта в пунктах"
type: docs
url: /ru/net/aspose.cells.rendering/renderingfont/size/
---
## RenderingFont.Size property

Получает размер шрифта в пунктах.

```csharp
public float Size { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingFontPropertySizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Создайте начальный шрифт и продемонстрируйте чтение свойства Size
            RenderingFont smallFont = new RenderingFont("Arial", 12);
            Console.WriteLine("Initial font size: " + smallFont.Size);

            // Создайте водяной знак с начальным размером шрифта
            PdfSaveOptions optionsSmall = new PdfSaveOptions
            {
                Watermark = new RenderingWatermark("CONFIDENTIAL", smallFont)
            };
            workbook.Save("SmallWatermark.pdf", optionsSmall);

            // Создайте новый шрифт с большим размером
            RenderingFont largeFont = new RenderingFont("Arial", 24);
            Console.WriteLine("Modified font size: " + largeFont.Size);

            // Создайте водяной знак с большим размером шрифта
            PdfSaveOptions optionsLarge = new PdfSaveOptions
            {
                Watermark = new RenderingWatermark("CONFIDENTIAL", largeFont)
            };
            workbook.Save("LargeWatermark.pdf", optionsLarge);
        }
    }
}
```

### См. также

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


