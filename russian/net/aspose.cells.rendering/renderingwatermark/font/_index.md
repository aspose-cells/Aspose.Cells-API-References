---
title: "RenderingWatermark.Font"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RenderingWatermark. Получает шрифт водяного знака"
type: docs
url: /ru/net/aspose.cells.rendering/renderingwatermark/font/
---
## RenderingWatermark.Font property

Получает шрифт водяного знака.

```csharp
public RenderingFont Font { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingWatermarkPropertyFontDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Создать шрифт рендеринга и задать начальные свойства
            RenderingFont font = new RenderingFont("Arial", 24);
            
            // Создать текстовый водяной знак с шрифтом рендеринга
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);
            
            // Отобразить начальные свойства шрифта
            Console.WriteLine("Initial Font Name: " + watermark.Font.Name);
            Console.WriteLine("Initial Font Size: " + watermark.Font.Size);
            Console.WriteLine("Initial Bold Status: " + watermark.Font.Bold);
            
            // Изменить свойства шрифта через ссылку RenderingFont
            font.Bold = true;
            
            // Отобразить обновленные свойства шрифта из водяного знака
            Console.WriteLine("\nUpdated Font Name: " + watermark.Font.Name);
            Console.WriteLine("Updated Font Size: " + watermark.Font.Size);
            Console.WriteLine("Updated Bold Status: " + watermark.Font.Bold);
            
            // Настроить свойства отображения водяного знака
            watermark.Opacity = 0.5f;
            watermark.Rotation = 45;
            watermark.IsBackground = true;
            
            // Создать параметры сохранения PDF и назначить водяной знак
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.Watermark = watermark;
            
            // Сохранить книгу с PDF, содержащим водяной знак, чтобы показать изменения шрифта
            workbook.Save("RenderingWatermarkFontDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### См. также

* class [RenderingFont](../../renderingfont/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


