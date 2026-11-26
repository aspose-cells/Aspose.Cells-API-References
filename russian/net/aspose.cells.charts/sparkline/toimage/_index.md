---
title: "Sparkline.ToImage"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Sparkline. Преобразует спарклайн в изображение"
type: docs
url: /ru/net/aspose.cells.charts/sparkline/toimage/
---
## ToImage(ImageOrPrintOptions) {#toimage}

Преобразует спарклайн в изображение.

```csharp
public Bitmap ToImage(ImageOrPrintOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| опции | ImageOrPrintOptions | Параметры изображения |

### Возвращаемое значение

Возвращает объект Bitmap.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SparklineMethodToImageWithImageOrPrintOptDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные для спарклайна
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["B1"].PutValue(20);
            sheet.Cells["C1"].PutValue(15);
            sheet.Cells["D1"].PutValue(30);

            // Определить расположение спарклайна
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 0,
                StartColumn = 4,
                EndColumn = 4
            };

            // Добавьте группу спарклайнов в лист
            int groupIndex = sheet.SparklineGroups.Add(SparklineType.Line, sheet.Name + "!A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[groupIndex];
            Sparkline sparkline = group.Sparklines[0];

            try
            {
                // Создать параметры изображения с реалистичными настройками
                ImageOrPrintOptions options = new ImageOrPrintOptions
                {
                    ImageType = Aspose.Cells.Drawing.ImageType.Jpeg,
                    HorizontalResolution = 200,
                    VerticalResolution = 200,
                    Quality = 90,
                    Transparent = false
                };

                // Сохранить спарклайн в файл, используя ToImage с ImageOrPrintOptions
                sparkline.ToImage("sparkline_demo.jpg", options);

                Console.WriteLine("Sparkline successfully saved as image with custom options.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving sparkline as image: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageOrPrintOptions) {#toimage_2}

Преобразует спарклайн в изображение.

```csharp
public void ToImage(string fileName, ImageOrPrintOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | String | Имя файла изображения. |
| опции | ImageOrPrintOptions | Параметры изображения |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SparklineMethodToImageWithStringImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            int idx = sheet.SparklineGroups.Add(SparklineType.Line, sheet.Name + "!A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];
            Sparkline line = group.Sparklines[0];

            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = Aspose.Cells.Drawing.ImageType.Png,
                HorizontalResolution = 300,
                VerticalResolution = 300
            };
            
            line.ToImage("sparkline_output.png", options);
        }
    }
}
```

### См. также

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageOrPrintOptions) {#toimage_1}

Преобразует спарклайн в изображение.

```csharp
public void ToImage(Stream stream, ImageOrPrintOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Stream | Поток изображения. |
| опции | ImageOrPrintOptions | Параметры изображения. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SparklineMethodToImageWithStreamImageOrPrintOptDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Определите CellArea для спарклайна
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Добавьте группу спарклайнов в лист
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, sheet.Name + "!A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];
            Sparkline line = group.Sparklines[0];

            try
            {
                // Создать поток памяти для сохранения изображения
                using (MemoryStream stream = new MemoryStream())
                {
                    // Создать параметры изображения
                    ImageOrPrintOptions options = new ImageOrPrintOptions
                    {
                        ImageType = Aspose.Cells.Drawing.ImageType.Png,
                        HorizontalResolution = 300,
                        VerticalResolution = 300
                    };

                    // Вызвать метод ToImage с параметрами Stream и ImageOrPrintOptions
                    line.ToImage(stream, options);

                    // Сохранить поток в файл
                    File.WriteAllBytes("sparkline_stream_output.png", stream.ToArray());
                    Console.WriteLine("Sparkline image saved successfully using stream.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling ToImage: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


