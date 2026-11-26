---
title: "DataLabels.NumberFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataLabels. Представляет строку формата для объекта DataLabels"
type: docs
url: /ru/net/aspose.cells.charts/datalabels/numberformat/
---
## DataLabels.NumberFormat property

Представляет строку формата для объекта DataLabels.

```csharp
public string NumberFormat { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyNumberFormatDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Включить подписи данных
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            
            // Установить пользовательский числовой формат для подписей данных
            series.DataLabels.NumberFormat = "_(* #,##0_);_(* \\(#,##0\\);_(* \"-\"??_);_(@_)";
            
            // Сохраните книгу
            workbook.Save("DataLabelsNumberFormatDemo.xlsx");
        }
    }
}
```

### См. также

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


