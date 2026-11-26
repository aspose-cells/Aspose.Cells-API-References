---
title: "RenderingWatermark.Image"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RenderingWatermark. Возвращает изображение водяного знака"
type: docs
url: /ru/net/aspose.cells.rendering/renderingwatermark/image/
---
## RenderingWatermark.Image property

Получает изображение водяного знака.

```csharp
public byte[] Image { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System.IO;

    public class RenderingWatermarkPropertyImageDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Загрузить данные изображения из файла
            byte[] originalImage = File.ReadAllBytes("watermark.png");

            // Создать водяной знак на основе изображения с начальным изображением
            RenderingWatermark watermark = new RenderingWatermark(originalImage);
            Console.WriteLine("Initial image size: " + watermark.Image.Length + " bytes");

            // Изменить свойства водяного знака
            watermark.Rotation = 45f;
            watermark.Opacity = 0.5f;
            watermark.ScaleToPagePercent = 75;
            watermark.IsBackground = true;
            watermark.HAlignment = TextAlignmentType.Center;
            watermark.VAlignment = TextAlignmentType.Center;

            // Создать параметры сохранения PDF с водяным знаком
            PdfSaveOptions pdfOptions = new PdfSaveOptions();
            pdfOptions.Watermark = watermark; // Fixed property name

            // Сохранить в PDF с выводом, содержащим водяной знак
            workbook.Save("WatermarkedOutput.pdf", pdfOptions);

            // Создать новый водяной знак с другим изображением
            byte[] updatedImage = File.ReadAllBytes("updated_watermark.png");
            RenderingWatermark newWatermark = new RenderingWatermark(updatedImage);
            Console.WriteLine("Updated image size: " + newWatermark.Image.Length + " bytes");

            // Сохранить с новым водяным знаком
            pdfOptions.Watermark = newWatermark; // Fixed property name
            workbook.Save("UpdatedWatermark.pdf", pdfOptions);
        }
    }
}
```

### См. также

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


