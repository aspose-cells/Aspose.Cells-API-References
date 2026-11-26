---
title: "ImageOrPrintOptions.TiffCompression"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Возвращает или задает тип сжатия, применяемый только при сохранении страниц в формате Tiff"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/tiffcompression/
---
## ImageOrPrintOptions.TiffCompression property

Получает или задает тип сжатия, применяемый только при сохранении страниц в формат `Tiff`.

```csharp
public TiffCompression TiffCompression { get; set; }
```

### Примечания

Имеет эффект только при сохранении в TIFF. Значение по умолчанию — Lzw.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyTiffCompressionDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("TIFF Compression Test");

            // Установить параметры изображения
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Tiff;
            options.HorizontalResolution = 300;
            options.VerticalResolution = 300;

            // Протестировать различные типы сжатия
            string outputPath = "OutputTIFF_";

            options.TiffCompression = TiffCompression.CompressionNone;
            SaveAsTiff(workbook, options, outputPath + "None.tiff");

            options.TiffCompression = TiffCompression.CompressionRle;
            SaveAsTiff(workbook, options, outputPath + "Rle.tiff");

            options.TiffCompression = TiffCompression.CompressionLZW;
            SaveAsTiff(workbook, options, outputPath + "LZW.tiff");

            options.TiffCompression = TiffCompression.CompressionCCITT3;
            SaveAsTiff(workbook, options, outputPath + "CCITT3.tiff");

            options.TiffCompression = TiffCompression.CompressionCCITT4;
            SaveAsTiff(workbook, options, outputPath + "CCITT4.tiff");
        }

        private static void SaveAsTiff(Workbook workbook, ImageOrPrintOptions options, string fileName)
        {
            WorkbookRender renderer = new WorkbookRender(workbook, options);
            renderer.ToImage(fileName);
        }
    }
}
```

### См. также

* enum [TiffCompression](../../tiffcompression/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


