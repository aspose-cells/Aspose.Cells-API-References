---
title: "ImageOrPrintOptions.SetDesiredSize"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ImageOrPrintOptions. Устанавливает желаемую ширину и высоту изображения"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/setdesiredsize/
---
## SetDesiredSize(int, int) {#setdesiredsize}

Задает желаемую ширину и высоту изображения.

```csharp
[Obsolete("Use SetDesiredSize(int, int, bool) by setting param keepAspectRatio to false instead.")]
public void SetDesiredSize(int desiredWidth, int desiredHeight)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| desiredWidth | Int32 | желаемая ширина в пикселях |
| desiredHeight | Int32 | желаемая высота в пикселях |

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо этого, пожалуйста, используйте `SetDesiredSize`, установив параметр keepAspectRatio в false. Это свойство будет удалено через 12 месяцев, начиная с мая 2023 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsMethodSetDesiredSizeWithInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Sample Data");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue(i);
            }

            // Установить область печати
            worksheet.PageSetup.PrintArea = "A1:A11";

            // Создать параметры изображения
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;
            options.SetDesiredSize(800, 600); // Using SetDesiredSize with Int32 parameters
            options.ImageType = Aspose.Cells.Drawing.ImageType.Jpeg;

            // Отрисовать лист в изображение
            SheetRender render = new SheetRender(worksheet, options);
            render.ToImage(0, "output.jpg");

            Console.WriteLine("Image generated with desired size 800x600");
        }
    }
}
```

### См. также

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## SetDesiredSize(int, int, bool) {#setdesiredsize_1}

Задает желаемую ширину и высоту изображения.

```csharp
public void SetDesiredSize(int desiredWidth, int desiredHeight, bool keepAspectRatio)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| desiredWidth | Int32 | желаемая ширина в пикселях |
| desiredHeight | Int32 | желаемая высота в пикселях |
| keepAspectRatio | Boolean | нужно ли сохранять соотношение сторон исходного изображения |

### Примечания

Ширина и высота выходного изображения в пикселях будут определяться только установленными желаемыми шириной и высотой.

[`HorizontalResolution`](../horizontalresolution/) и [`VerticalResolution`](../verticalresolution/) не будут влиять на ширину и высоту выходного изображения в этом случае.

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsMethodSetDesiredSizeWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные и создайте диаграмму
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);
            chart.NSeries.CategoryData = "B1:B3";

            // Получить форму диаграммы
            Shape chartShape = worksheet.Shapes[0];

            // Установить параметры изображения
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png;
            options.SetDesiredSize(800, 600, false); // Using SetDesiredSize with width, height, and keepAspectRatio

            // Сохранить диаграмму как изображение
            MemoryStream stream = new MemoryStream();
            chartShape.ToImage(stream, options);

            // Сохранить изображение в файл
            File.WriteAllBytes("output_chart.png", stream.ToArray());
        }
    }
}
```

### См. также

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


