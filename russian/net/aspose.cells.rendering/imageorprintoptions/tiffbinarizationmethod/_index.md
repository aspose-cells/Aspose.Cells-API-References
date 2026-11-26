---
title: "ImageOrPrintOptions.TiffBinarizationMethod"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Получает или задает метод, используемый при преобразовании изображений в формат 1 bpp, когда ImageType имеет значение Tiff и TiffCompression равно Ccitt3 или Ccitt4"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/tiffbinarizationmethod/
---
## ImageOrPrintOptions.TiffBinarizationMethod property

Получает или задает метод, используемый при преобразовании изображений в формат 1 bpp, когда [`ImageType`](../imagetype/) имеет значение Tiff и [`TiffCompression`](../tiffcompression/) равно Ccitt3 или Ccitt4.

```csharp
public ImageBinarizationMethod TiffBinarizationMethod { get; set; }
```

### Примечания

Значение по умолчанию — FloydSteinbergDithering.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class ImageOrPrintOptionsPropertyTiffBinarizationMethodDemo
    {
        public static void Run()
        {
            // Создать книгу с образцовыми данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить данные градиента для визуальной демонстрации
            for (int i = 0; i < 15; i++)
            {
                Cell cell = worksheet.Cells[i, 0];
                cell.PutValue(i * 7);
                Style style = cell.GetStyle();
                style.BackgroundColor = Color.FromArgb(i * 18, i * 18, i * 18);
                cell.SetStyle(style);
            }

            // Настроить параметры рендеринга TIFF
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Tiff,
                TiffCompression = TiffCompression.CompressionCCITT3,
                TiffColorDepth = ColorDepth.Format1bpp
            };

            // Отобразить текущий метод бинаризации
            Console.WriteLine("Initial TiffBinarizationMethod: " + options.TiffBinarizationMethod);

            // Визуализировать с методом порога по умолчанию
            new SheetRender(worksheet, options).ToImage(0, "ThresholdBinarization.tiff");

            // Переключиться на дизеринг Floyd-Steinberg
            options.TiffBinarizationMethod = ImageBinarizationMethod.FloydSteinbergDithering;
            Console.WriteLine("\nModified TiffBinarizationMethod: " + options.TiffBinarizationMethod);

            // Визуализировать новым методом
            new SheetRender(worksheet, options).ToImage(0, "DitheringBinarization.tiff");

            Console.WriteLine("\nGenerated TIFF files demonstrate different 1bpp conversion methods.");
        }
    }
}
```

### См. также

* enum [ImageBinarizationMethod](../../imagebinarizationmethod/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


