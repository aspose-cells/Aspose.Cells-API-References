---
title: "Класс RenderingWatermark"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Rendering.RenderingWatermark. Водяной знак для рендеринга"
type: docs
url: /ru/net/aspose.cells.rendering/renderingwatermark/
---
## RenderingWatermark class

Водяной знак для рендеринга.

```csharp
public class RenderingWatermark
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [RenderingWatermark](renderingwatermark/#constructor)(byte[]) | Создает экземпляр водяного знака изображения. |
| [RenderingWatermark](renderingwatermark/#constructor_1)(string, RenderingFont) | Создает экземпляр текстового водяного знака. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Font](../../aspose.cells.rendering/renderingwatermark/font/) { get; } | Получает шрифт водяного знака. |
| [HAlignment](../../aspose.cells.rendering/renderingwatermark/halignment/) { get; set; } | Получает или задает горизонтальное выравнивание водяного знака относительно страницы. |
| [Image](../../aspose.cells.rendering/renderingwatermark/image/) { get; } | Получает изображение водяного знака. |
| [IsBackground](../../aspose.cells.rendering/renderingwatermark/isbackground/) { get; set; } | Указывает, размещён ли водяной знак за содержимым страницы. |
| [OffsetX](../../aspose.cells.rendering/renderingwatermark/offsetx/) { get; set; } | Получает или задает значение смещения для [`HAlignment`](./halignment/) |
| [OffsetY](../../aspose.cells.rendering/renderingwatermark/offsety/) { get; set; } | Получает или задает значение смещения для [`VAlignment`](./valignment/) |
| [Opacity](../../aspose.cells.rendering/renderingwatermark/opacity/) { get; set; } | Получает или задает непрозрачность водяного знака в диапазоне [0, 1]. |
| [Rotation](../../aspose.cells.rendering/renderingwatermark/rotation/) { get; set; } | Получает или задает вращение водяного знака в градусах. |
| [ScaleToPagePercent](../../aspose.cells.rendering/renderingwatermark/scaletopagepercent/) { get; set; } | Получает или задает масштаб относительно целевой страницы в процентах. |
| [Text](../../aspose.cells.rendering/renderingwatermark/text/) { get; } | Получает текст водяного знака. |
| [VAlignment](../../aspose.cells.rendering/renderingwatermark/valignment/) { get; set; } | Получает или задает вертикальное выравнивание водяного знака относительно страницы. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.Drawing;

    public class RenderingWatermarkDemo
    {
        public static void RenderingWatermarkExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This is a sample worksheet.");

            // Создать шрифт для водяного знака
            RenderingFont font = new RenderingFont("Calibri", 68);
            font.Italic = true;
            font.Bold = true;
            font.Color = Color.Blue;

            // Создать водяной знак из текста и указанного шрифта
            RenderingWatermark watermark = new RenderingWatermark("Watermark", font);

            // Установить свойства водяного знака
            watermark.HAlignment = TextAlignmentType.Center;
            watermark.VAlignment = TextAlignmentType.Center;
            watermark.Rotation = 30;
            watermark.Opacity = 0.6f;
            watermark.ScaleToPagePercent = 50;
            watermark.IsBackground = true;

            // Указать водяной знак для рендеринга в PDF
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark;

            // Сохранить книгу в формате PDF с водяным знаком
            workbook.Save("output_watermark.pdf", options);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


