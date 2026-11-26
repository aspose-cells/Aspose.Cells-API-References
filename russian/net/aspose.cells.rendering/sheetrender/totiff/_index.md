---
title: "SheetRender.ToTiff"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SheetRender. Отрисовать весь worksheet как Tiff Image в поток."
type: docs
url: /ru/net/aspose.cells.rendering/sheetrender/totiff/
---
## ToTiff(Stream) {#totiff}

Отрисовать весь лист как изображение Tiff в поток.

```csharp
public void ToTiff(Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Stream | поток выходного изображения |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SheetRenderMethodToTiffWithStreamDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите доступ к первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерное содержимое для демонстрации отрисовки.
            worksheet.Cells["A1"].PutValue("Aspose.Cells TIFF Rendering Demo");
            
            // Настройте параметры изображения для отрисовки.
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;

            // Создайте рендер листа с настроенными параметрами.
            SheetRender renderer = new SheetRender(worksheet, options);
            try
            {
                // Создайте выходной поток для TIFF-изображения.
                using (FileStream tiffStream = new FileStream("output.tiff", FileMode.Create))
                {
                    // Отрисуйте worksheet в TIFF, используя поток.
                    renderer.ToTiff(tiffStream);
                    Console.WriteLine("Worksheet successfully rendered to TIFF stream.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during TIFF rendering: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToTiff(string) {#totiff_1}

Отрисовать весь лист как изображение Tiff в файл.

```csharp
public void ToTiff(string filename)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| имя файла | String | имя файла выходного изображения |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodToTiffWithStringDemo
    {
        public static void Run()
        {
            // Загрузить исходный файл Excel
            Workbook workbook = new Workbook("Book1.xlsx");

            // Создать параметры изображения или печати
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.SaveFormat = SaveFormat.Tiff;

            // Создать рендер листа для первого рабочего листа
            SheetRender sheetRender = new SheetRender(workbook.Worksheets[0], options);

            // Сохраните все страницы листа как многостраничный TIFF-файл.
            sheetRender.ToTiff("output.tiff");
        }
    }
}
```

### См. также

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


