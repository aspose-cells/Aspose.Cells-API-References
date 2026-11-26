---
title: "Класс Sparkline"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Charts.Sparkline class. Спарклайн представляет собой крошечную диаграмму или графику в ячейке листа, которая предоставляет визуальное представление данных"
type: docs
url: /ru/net/aspose.cells.charts/sparkline/
---
## Sparkline class

Спарклайн представляет собой крошечную диаграмму или график в ячейке листа, предоставляющий визуальное представление данных.

```csharp
public class Sparkline
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Column](../../aspose.cells.charts/sparkline/column/) { get; } | Получает индекс столбца спарклайна. |
| [DataRange](../../aspose.cells.charts/sparkline/datarange/) { get; set; } | Представляет диапазон данных спарклайна. |
| [Row](../../aspose.cells.charts/sparkline/row/) { get; } | Получает индекс строки спарклайна. |

## Методы

| Имя | Описание |
| --- | --- |
| [ToImage](../../aspose.cells.charts/sparkline/toimage/#toimage)(ImageOrPrintOptions) | Преобразует спарклайн в изображение. |
| [ToImage](../../aspose.cells.charts/sparkline/toimage/#toimage_1)(Stream, ImageOrPrintOptions) | Преобразует спарклайн в изображение. |
| [ToImage](../../aspose.cells.charts/sparkline/toimage/#toimage_2)(string, ImageOrPrintOptions) | Преобразует спарклайн в изображение. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SparklineDemo
    {
        public static void SparklineExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить некоторые данные в лист
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

            // Добавить спарклайн в группу
            idx = group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 5);
            Sparkline line = group.Sparklines[idx];

            // Вывести детали спарклайна
            Console.WriteLine("Sparkline data range: " + line.DataRange + ", row: " + line.Row + ", column: " + line.Column);

            // Сохранить спарклайн как изображение
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = Aspose.Cells.Drawing.ImageType.Png,
                HorizontalResolution = 300,
                VerticalResolution = 300
            };
            line.ToImage("output.png", options);

            // Сохраните книгу
            workbook.Save("SparklineExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


