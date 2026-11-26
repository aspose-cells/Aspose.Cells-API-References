---
title: "Enum TiffCompression"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Rendering.TiffCompression enum. Указывает тип сжатия, который следует применять при сохранении изображений в файл формата TIFF"
type: docs
url: /ru/net/aspose.cells.rendering/tiffcompression/
---
## TiffCompression enumeration

Указывает, какой тип сжатия применять при сохранении изображений в файл формата TIFF.

```csharp
public enum TiffCompression
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| CompressionNone | `0` | Указывает отсутствие сжатия. |
| CompressionRle | `1` | Указывает схему сжатия RLE. |
| CompressionLZW | `2` | Указывает схему сжатия LZW. |
| CompressionCCITT3 | `3` | Указывает схему сжатия CCITT3. |
| CompressionCCITT4 | `4` | Указывает схему сжатия CCITT4. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingClassTiffCompressionDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            ws.Cells["A1"].PutValue("TIFF Compression Test");
            ws.Cells["A2"].PutValue(DateTime.Now.ToString());

            // Установить параметры изображения
            ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
            imgOpt.HorizontalResolution = 300;
            imgOpt.VerticalResolution = 300;
            imgOpt.ImageType = ImageType.Tiff;

            // Протестировать различные типы сжатия
            string outputPath = "output_compression_";

            // Сжатие LZW
            imgOpt.TiffCompression = TiffCompression.CompressionLZW;
            new WorkbookRender(wb, imgOpt).ToImage(outputPath + "LZW.tiff");

            // Сжатие CCITT3
            imgOpt.TiffCompression = TiffCompression.CompressionCCITT3;
            new WorkbookRender(wb, imgOpt).ToImage(outputPath + "CCITT3.tiff");

            // Сжатие CCITT4
            imgOpt.TiffCompression = TiffCompression.CompressionCCITT4;
            new WorkbookRender(wb, imgOpt).ToImage(outputPath + "CCITT4.tiff");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


