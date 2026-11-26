---
title: "RenderingWatermark.RenderingWatermark"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор RenderingWatermark. Создает экземпляр текстового водяного знака"
type: docs
url: /ru/net/aspose.cells.rendering/renderingwatermark/renderingwatermark/
---
## RenderingWatermark(string, RenderingFont) {#constructor_1}

Создает экземпляр текстового водяного знака.

```csharp
public RenderingWatermark(string text, RenderingFont renderingFont)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| текст | String | текст водяного знака |
| renderingFont | RenderingFont | шрифт водяного знака |

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkMethodCtorWithStringRenderingFontDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Создать объект RenderingFont
            RenderingFont renderingFont = new RenderingFont("Arial", 12)
            {
                Bold = true,
                Color = Color.Blue
            };

            // Создать объект RenderingWatermark с использованием #ctor(string, RenderingFont)
            RenderingWatermark watermark = new RenderingWatermark("DEMO WATERMARK", renderingFont)
            {
                Rotation = 45,
                Opacity = 0.3f
            };

            // Создать PdfSaveOptions и установить водяной знак
            PdfSaveOptions saveOptions = new PdfSaveOptions
            {
                Watermark = watermark
            };

            // Сохранить книгу с водяным знаком
            workbook.Save("WatermarkDemo.pdf", saveOptions);
        }
    }
}
```

### См. также

* class [RenderingFont](../../renderingfont/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## RenderingWatermark(byte[]) {#constructor}

Создает экземпляр водяного знака изображения.

```csharp
public RenderingWatermark(byte[] imageData)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| imageData | Byte[] |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class RenderingWatermarkMethodCtorWithByteArrayDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Подготовить данные изображения для водяного знака
            string imagePath = "watermark.png";
            
            if (!File.Exists(imagePath))
            {
                Console.WriteLine($"Image file not found: {imagePath}");
                return;
            }

            try
            {
                byte[] imageData = File.ReadAllBytes(imagePath);
                
                // Создать RenderingWatermark с конструктором Byte[]
                RenderingWatermark watermark = new RenderingWatermark(imageData);
                
                // Настроить свойства водяного знака
                watermark.Rotation = 45;
                watermark.Opacity = 0.5f;
                watermark.ScaleToPagePercent = 50;
                watermark.IsBackground = true;
                watermark.HAlignment = TextAlignmentType.Center;
                watermark.VAlignment = TextAlignmentType.Center;

                // Создать параметры сохранения PDF и применить водяной знак
                PdfSaveOptions saveOptions = new PdfSaveOptions();
                saveOptions.Watermark = watermark; // Fixed property name

                // Сохранить книгу с эффектом водяного знака
                workbook.Save("WatermarkOutput.pdf", saveOptions);
                
                Console.WriteLine("Watermark applied successfully using Byte[] constructor. Output saved to WatermarkOutput.pdf");
            }
            catch (FileNotFoundException ex)
            {
                Console.WriteLine($"Error loading image file: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RenderingWatermark constructor: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


