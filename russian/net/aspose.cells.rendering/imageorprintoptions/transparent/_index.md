---
title: "ImageOrPrintOptions.Transparent"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Указывает, должен ли фон сгенерированного изображения быть прозрачным"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/transparent/
---
## ImageOrPrintOptions.Transparent property

Указывает, должен ли фон сгенерированного изображения быть прозрачным.

```csharp
public bool Transparent { get; set; }
```

### Примечания

Значение по умолчанию — false. Это означает, что фон сгенерированных изображений белый.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyTransparentDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Transparent Image Demo");
            
            // Установить параметры сохранения HTML с прозрачным PNG‑изображением
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ImageOptions.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.ImageOptions.Transparent = true;
            options.ExportImagesAsBase64 = true;

            // Сохранить книгу с параметрами прозрачного изображения
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML with transparent images saved successfully.");
        }
    }
}
```

### См. также

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


