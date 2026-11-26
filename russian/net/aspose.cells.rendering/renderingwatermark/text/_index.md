---
title: "RenderingWatermark.Text"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RenderingWatermark. Возвращает текст водяного знака"
type: docs
url: /ru/net/aspose.cells.rendering/renderingwatermark/text/
---
## RenderingWatermark.Text property

Получает текст водяного знака.

```csharp
public string Text { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingWatermarkPropertyTextDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать шрифт рендеринга для текста водяного знака
            RenderingFont font = new RenderingFont("Arial", 36);

            // Инициализировать текстовый водяной знак с конфигурацией шрифта
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);

            // Отобразить текущий текст водяного знака
            Console.WriteLine("Watermark Text: " + watermark.Text);

            // Настроить внешний вид водяного знака
            watermark.Rotation = 45f;
            watermark.Opacity = 0.3f;
            watermark.IsBackground = true;
            watermark.ScaleToPagePercent = 150;

            // Применить водяной знак к параметрам сохранения PDF
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark; // Fixed property name

            // Сохранить в PDF для визуализации эффектов водяного знака
            workbook.Save("WatermarkDemo.pdf", options);
        }
    }
}
```

### См. также

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


