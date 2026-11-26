---
title: "Series.XValuesFormatCode"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Series property. Представляет код формата X Values NumberList"
type: docs
url: /ru/net/aspose.cells.charts/series/xvaluesformatcode/
---
## Series.XValuesFormatCode property

Представляет код формата списка чисел X Values.

```csharp
public string XValuesFormatCode { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyXValuesFormatCodeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
            worksheet.Cells["B3"].PutValue(200);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Установите код формата XValues
            chart.NSeries[0].XValuesFormatCode = "M/d/yyyy";

            // Сохраните книгу
            workbook.Save("SeriesPropertyXValuesFormatCodeDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


