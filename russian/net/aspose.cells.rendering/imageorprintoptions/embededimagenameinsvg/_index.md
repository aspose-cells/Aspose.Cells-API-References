---
title: "ImageOrPrintOptions.EmbededImageNameInSvg"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Указывает имя файла встроенного изображения в svg. Должен быть полный путь с каталогом, например cxpsEmbedded"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg/
---
## ImageOrPrintOptions.EmbededImageNameInSvg property

Указывает имя файла встроенного изображения в svg. Это должен быть полный путь с каталогом, например "c:\\xpsEmbedded"

```csharp
[Obsolete("Images are now always embedded in Svg with base64 format, please remove this property.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string EmbededImageNameInSvg { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо этого, пожалуйста, удалите это свойство, так как изображения теперь всегда встраиваются в Svg в формате base64. Это свойство будет удалено через 12 месяцев, начиная с апреля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertyEmbededImageNameInSvgDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите доступ к первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте простое изображение в памяти и добавьте его в лист
            byte[] redPngBytes = Convert.FromBase64String("iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");
            worksheet.Pictures.Add(0, 0, new MemoryStream(redPngBytes));

            // Создайте параметры рендеринга изображения в формате SVG
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Svg
            };

            // Отобразить текущий путь к встроенному изображению
            Console.WriteLine("Initial EmbededImageNameInSvg: " + options.EmbededImageNameInSvg);

            // Настройте новый каталог для встроенных изображений
            string imageDir = "svg_embedded_images/";
            options.EmbededImageNameInSvg = imageDir;
            Directory.CreateDirectory(imageDir);

            // Отобразите лист в SVG с настроенными параметрами
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "worksheet_output.svg");

            Console.WriteLine("Generated SVG with embedded images in: " + Path.GetFullPath(imageDir));
        }
    }
}
```

### См. также

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


