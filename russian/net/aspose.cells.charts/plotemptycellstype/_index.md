---
title: "Перечисление PlotEmptyCellsType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Charts.PlotEmptyCellsType. Представляет все типы пустых ячеек диаграммы."
type: docs
url: /ru/net/aspose.cells.charts/plotemptycellstype/
---
## PlotEmptyCellsType enumeration

Представляет все типы пустых ячеек построения диаграммы.

```csharp
public enum PlotEmptyCellsType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| NotPlotted | `0` | Не отображается (оставить пробел) |
| Zero | `1` | Ноль |
| Interpolated | `2` | Интерполировано |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotEmptyCellsTypeDemo
    {
        public static void PlotEmptyCellsTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(null); // Empty cell
            worksheet.Cells["A5"].PutValue("D");
            worksheet.Cells["B5"].PutValue(40);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных для диаграммы
            chart.SetChartDataRange("A1:B5", true);

            // Установить заголовок диаграммы
            chart.Title.Text = "Plot Empty Cells Example";

            // Установите, как отображать пустые ячейки
            chart.PlotEmptyCellsType = PlotEmptyCellsType.Interpolated;

            // Сохраните книгу
            workbook.Save("PlotEmptyCellsTypeExample.xlsx");

            Console.WriteLine("Workbook saved successfully.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


