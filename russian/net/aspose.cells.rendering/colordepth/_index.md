---
title: "Перечисление ColorDepth"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Rendering.ColorDepth. Перечисляет тип глубины цвета для tiff-изображения"
type: docs
url: /ru/net/aspose.cells.rendering/colordepth/
---
## ColorDepth enumeration

Перечисляет тип глубины цвета для TIFF‑изображения.

```csharp
public enum ColorDepth
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Default | `0` | Значение по умолчанию, не установленное значение. |
| Format1bpp | `1` | 1 бит на пиксель |
| Format4bpp | `4` | 4 бита на пиксель |
| Format8bpp | `8` | 8 бит на пиксель |
| Format24bpp | `24` | 24 бита на пиксель |
| Format32bpp | `32` | 32 бита на пиксель |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Drawing;
    using System;

    public class RenderingClassColorDepthDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("TIFF Color Depth Demonstration");
            worksheet.Cells["B2"].PutValue(12345);
            
            // Настройте параметры изображения TIFF
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Tiff;
            options.TiffColorDepth = ColorDepth.Format8bpp;

            // Отрендерите лист в TIFF с указанной глубиной цвета
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "output_8bpp.tiff");

            // Продемонстрируйте другой вариант глубины цвета
            options.TiffColorDepth = ColorDepth.Format24bpp;
            renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "output_24bpp.tiff");

            Console.WriteLine("TIFF files created with different color depths.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


