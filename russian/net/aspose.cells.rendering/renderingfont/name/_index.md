---
title: "RenderingFont.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RenderingFont. Получает имя шрифта"
type: docs
url: /ru/net/aspose.cells.rendering/renderingfont/name/
---
## RenderingFont.Name property

Получает имя шрифта.

```csharp
public string Name { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingFontPropertyNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Создайте параметры сохранения PDF
            PdfSaveOptions options = new PdfSaveOptions();

            // Создайте начальный рендеринговый шрифт с "Arial"
            RenderingFont fontArial = new RenderingFont("Arial", 16);
            Console.WriteLine("Initial font name: " + fontArial.Name);

            // Создайте водяной знак с начальным шрифтом
            RenderingWatermark watermark = new RenderingWatermark("Confidential", fontArial);
            watermark.Opacity = 0.5f;
            watermark.Rotation = 45;
            options.Watermark = watermark;

            // Сохраните с водяным знаком начального шрифта
            workbook.Save("WatermarkInitial.pdf", options);

            // Создайте новый рендеринговый шрифт с "Times New Roman"
            RenderingFont fontTimesNewRoman = new RenderingFont("Times New Roman", 16);
            Console.WriteLine("\nModified font name: " + fontTimesNewRoman.Name);

            // Обновите водяной знак новым шрифтом
            RenderingWatermark updatedWatermark = new RenderingWatermark("Confidential", fontTimesNewRoman);
            updatedWatermark.Opacity = 0.5f;
            updatedWatermark.Rotation = 45;
            options.Watermark = updatedWatermark;

            // Сохраните с изменённым водяным знаком шрифта
            workbook.Save("WatermarkModified.pdf", options);
        }
    }
}
```

### См. также

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


