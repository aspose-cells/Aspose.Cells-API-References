---
title: "Chart.SetChartDataRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Chart. Указывает диапазон данных для диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chart/setchartdatarange/
---
## Chart.SetChartDataRange method

Указывает диапазон данных для диаграммы.

```csharp
public void SetChartDataRange(string area, bool isVertical)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| область | String | Указывает значения, из которых строится серия данных |
| isVertical | Boolean | Указывает, строить ли серию из диапазона ячеек по строкам или по столбцам. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodSetChartDataRangeWithStringBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["A2"].PutValue("Cat1");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Cat2");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("Cat3");
            worksheet.Cells["B4"].PutValue(30);
            
            // Добавить диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.SetChartDataRange("A1:B4", true);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


