---
title: "ImageOrPrintOptions.TiffColorDepth"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Получает или задает глубину цвета, применяемую только при сохранении страниц в формате Tiff"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/tiffcolordepth/
---
## ImageOrPrintOptions.TiffColorDepth property

Получает или задает глубину цвета, применяемую только при сохранении страниц в формат `Tiff`.

```csharp
public ColorDepth TiffColorDepth { get; set; }
```

### Примечания

Имеет эффект только при сохранении в TIFF. Если TiffCompression установлен в CCITT3 или CCITT4, это не будет применяться, глубина цвета сгенерированного tiff‑изображения всегда будет 1.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyTiffColorDepthDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте отформатированное содержимое для демонстрации глубины цвета
            worksheet.Cells["A1"].PutValue("TIFF Color Depth Demonstration");
            Cell cell = worksheet.Cells["B3"];
            cell.PutValue("24-bit Color Depth");
            Style style = cell.GetStyle();
            style.Font.Color = System.Drawing.Color.FromArgb(255, 0, 128, 0);
            style.BackgroundColor = System.Drawing.Color.FromArgb(255, 255, 192, 128);
            style.Pattern = BackgroundType.Solid;
            cell.SetStyle(style);

            // Инициализируйте ImageOrPrintOptions для рендеринга TIFF
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Tiff,
                TiffCompression = TiffCompression.CompressionLZW
            };

            // Отобразите и измените TiffColorDepth
            Console.WriteLine($"Initial TiffColorDepth: {options.TiffColorDepth}");
            
            // Отобразить с глубиной по умолчанию (1 бпп)
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToTiff("DefaultDepthOutput.tiff");

            // Изменить на 24‑битную глубину цвета
            options.TiffColorDepth = ColorDepth.Format24bpp;
            Console.WriteLine($"Modified TiffColorDepth: {options.TiffColorDepth}");

            // Отобразить с новой глубиной
            renderer.ToTiff("24BitDepthOutput.tiff");

            Console.WriteLine("Generated TIFF files with different color depths.");
        }
    }
}
```

### См. также

* enum [ColorDepth](../../colordepth/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


