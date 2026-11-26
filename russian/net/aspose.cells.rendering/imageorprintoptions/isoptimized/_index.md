---
title: "ImageOrPrintOptions.IsOptimized"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Указывает, следует ли оптимизировать выходные элементы"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/isoptimized/
---
## ImageOrPrintOptions.IsOptimized property

Указывает, следует ли оптимизировать выводимые элементы.

```csharp
public bool IsOptimized { get; set; }
```

### Примечания

Значение по умолчанию — false. В настоящее время, когда это свойство установлено в true, будут выполнены следующие оптимизации: 1. оптимизация линий границы. 2. оптимизация размера файла при рендеринге в изображение Svg.

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyIsOptimizedDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в ячейки
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].PutValue($"Data {i}-{j}");
                }
            }

            // Настройте параметры рендеринга изображения
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnePagePerSheet = true;
            
            // Продемонстрируйте свойство IsOptimized
            options.IsOptimized = true; // Enable optimization
            
            // Отрендерьте лист в изображение
            SheetRender renderer = new SheetRender(sheet, options);
            MemoryStream stream = new MemoryStream();
            renderer.ToImage(0, stream);
            
            Console.WriteLine($"Image rendered with optimization: {options.IsOptimized}");
            Console.WriteLine($"Image size: {stream.Length} bytes");
        }
    }
}
```

### См. также

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


