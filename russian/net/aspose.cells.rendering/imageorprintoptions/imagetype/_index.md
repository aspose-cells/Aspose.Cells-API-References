---
title: "ImageOrPrintOptions.ImageType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Возвращает или задает формат создаваемых изображений. значение по умолчанию PNG"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/imagetype/
---
## ImageOrPrintOptions.ImageType property

Получает или задает формат сгенерированных изображений. значение по умолчанию: PNG.

```csharp
public virtual ImageType ImageType { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyImageTypeDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test SVG Image");

            // Установите параметры сохранения HTML с типом изображения SVG
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ImageOptions.ImageType = ImageType.Svg;
            options.ExportActiveWorksheetOnly = true;

            // Сохраните книгу в формате HTML
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "output.html");
            workbook.Save(outputPath, options);

            Console.WriteLine("File saved with SVG images: " + outputPath);
        }
    }
}
```

### См. также

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


