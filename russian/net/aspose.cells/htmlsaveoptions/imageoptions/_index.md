---
title: "HtmlSaveOptions.ImageOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Получите объект ImageOrPrintOptions перед экспортом"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/imageoptions/
---
## HtmlSaveOptions.ImageOptions property

Получите объект ImageOrPrintOptions перед экспортом

```csharp
public ImageOrPrintOptions ImageOptions { get; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyImageOptionsDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample HTML Export");
            
            // Установите параметры сохранения HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportImagesAsBase64 = true;
            
            // Настройте параметры изображения
            ImageOrPrintOptions imageOptions = saveOptions.ImageOptions;
            imageOptions.ImageType = ImageType.Svg;
            imageOptions.HorizontalResolution = 300;
            imageOptions.VerticalResolution = 300;
            
            // Сохранить рабочую книгу с параметрами HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("HTML file saved with SVG images.");
        }
    }
}
```

### См. также

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


