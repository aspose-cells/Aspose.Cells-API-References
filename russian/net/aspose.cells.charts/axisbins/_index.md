---
title: "Класс AxisBins"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Charts.AxisBins. Представляет интервалы оси"
type: docs
url: /ru/net/aspose.cells.charts/axisbins/
---
## AxisBins class

Представляет интервалы оси

```csharp
public class AxisBins
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.cells.charts/axisbins/count/) { get; set; } | Получает или задает количество интервалов оси |
| [IsAutomatic](../../aspose.cells.charts/axisbins/isautomatic/) { get; set; } | Указывает, являются ли интервалы оси автоматическими. |
| [IsByCategory](../../aspose.cells.charts/axisbins/isbycategory/) { get; set; } | Указывает, включено ли группирование данных по категории. |
| [Overflow](../../aspose.cells.charts/axisbins/overflow/) { get; set; } | Получает или задает переполнение интервалов оси |
| [Underflow](../../aspose.cells.charts/axisbins/underflow/) { get; set; } | Получает или задает недополнение интервалов оси |
| [Width](../../aspose.cells.charts/axisbins/width/) { get; set; } | Получает или задает ширину интервала оси. |

## Методы

| Имя | Описание |
| --- | --- |
| [ResetOverflow](../../aspose.cells.charts/axisbins/resetoverflow/)() | (**Obsolete.**) Сбросить переполнение |
| [ResetUnderflow](../../aspose.cells.charts/axisbins/resetunderflow/)() | (**Obsolete.**) Сбросить недополнение |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisBinsDemo
    {
        public static void AxisBinsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            // Добавить новый лист
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Histogram, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Добавьте серию данных в диаграмму
            chart.NSeries.Add("A1:A5", true);

            // Доступ к оси значений
            Axis valueAxis = chart.ValueAxis;

            // Доступ к интервалам оси значений
            AxisBins bins = valueAxis.Bins;

            // Установить свойства для интервалов
            bins.IsByCategory = false;
            bins.IsAutomatic = true;
            bins.Width = 10.0;
            bins.Count = 5;
            bins.Overflow = 60.0;
            bins.Underflow = 0.0;

            // Сбросить переполнение и недополнение
            //bins.ResetOverflow();
            //bins.ResetUnderflow();

            // Сохраните книгу
            workbook.Save("AxisBinsExample.xlsx");
            workbook.Save("AxisBinsExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


