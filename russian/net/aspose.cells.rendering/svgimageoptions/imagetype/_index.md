---
title: "SvgImageOptions.ImageType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SvgImageOptions. Получает или задает формат генерируемых изображений. значение по умолчанию PNG"
type: docs
url: /ru/net/aspose.cells.rendering/svgimageoptions/imagetype/
---
## SvgImageOptions.ImageType property

Получает или задает формат сгенерированных изображений. значение по умолчанию: PNG.

```csharp
public override ImageType ImageType { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SvgImageOptionsPropertyImageTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте пример данных и изображение
            worksheet.Cells["A1"].PutValue("Embedded Image Type Demonstration");
            int pictureIndex = worksheet.Pictures.Add(0, 1, "inputImage.png");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Создать параметры рендеринга SVG
            SvgImageOptions svgOptions = new SvgImageOptions();

            // Отобразить текущий ImageType (по умолчанию: PNG)
            Console.WriteLine("Current ImageType: " + svgOptions.ImageType);

            // Изменить формат изображения для встроенных растровых изображений
            svgOptions.ImageType = ImageType.Jpeg;

            // Сохранить содержимое листа как SVG с различными форматами изображений
            using (MemoryStream stream = new MemoryStream())
            {
                picture.ToImage(stream, svgOptions);
                File.WriteAllBytes("output_with_jpeg.svg", stream.ToArray());
            }

            // Сбросить к формату PNG
            svgOptions.ImageType = ImageType.Png;
            
            using (MemoryStream stream = new MemoryStream())
            {
                picture.ToImage(stream, svgOptions);
                File.WriteAllBytes("output_with_png.svg", stream.ToArray());
            }

            Console.WriteLine("SVG files created with different embedded image formats.");
        }
    }
}
```

### См. также

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


