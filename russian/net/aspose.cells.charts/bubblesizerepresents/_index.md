---
title: "Перечисление BubbleSizeRepresents."
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Charts.BubbleSizeRepresents. Описывает, что представляет размер пузыря на пузырчатой диаграмме."
type: docs
url: /ru/net/aspose.cells.charts/bubblesizerepresents/
---
## BubbleSizeRepresents enumeration

Определяет, что представляет размер пузыря на пузырьковой диаграмме.

```csharp
public enum BubbleSizeRepresents
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| SizeIsArea | `0` | Представляет значение [`BubbleSizes`](../series/bubblesizes/), которое является площадью пузыря. |
| SizeIsWidth | `1` | Представляет значение [`BubbleSizes`](../series/bubblesizes/), которое является шириной пузыря. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class BubbleSizeRepresentsDemo
    {
        public static void BubbleSizeRepresentsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные для пузырчатой диаграммы.
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["B2"].PutValue(3);
            worksheet.Cells["B3"].PutValue(4);
            worksheet.Cells["C1"].PutValue(5);
            worksheet.Cells["C2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(15);

            // Добавьте пузырчатую диаграмму на лист.
            int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Добавьте серию в пузырчатую диаграмму.
            int seriesIndex = chart.NSeries.Add("A1:C3", true);
            Series series = chart.NSeries[seriesIndex];

            // Установите значения X, значения Y и размеры пузырей.
            series.XValues = "A1:A3";
            series.Values = "B1:B3";
            series.BubbleSizes = "C1:C3";

            // Установите представление размера пузыря.
            series.SizeRepresents = BubbleSizeRepresents.SizeIsArea;

            // Сохраните книгу
            workbook.Save("BubbleSizeRepresentsExample.xlsx");
            workbook.Save("BubbleSizeRepresentsExample.pdf");

            // Установите представление размера пузыря.
            series.SizeRepresents = BubbleSizeRepresents.SizeIsWidth;

            // Сохраните книгу
            workbook.Save("BubbleSizeRepresentsExample2.xlsx");
            workbook.Save("BubbleSizeRepresentsExample2.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


