---
title: "DataLabels.ShowLegendKey"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataLabels. Представляет поведение отображения ключа легенды подписи данных указанного графика. True, если ключ легенды подписи данных виден"
type: docs
url: /ru/net/aspose.cells.charts/datalabels/showlegendkey/
---
## DataLabels.ShowLegendKey property

Представляет поведение отображения ключа легенды метки данных указанной диаграммы. True, если ключ легенды метки данных видим.

```csharp
public bool ShowLegendKey { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowLegendKeyDemo
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
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получить подписи данных
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            
            // Установить ShowLegendKey в true
            dataLabels.ShowLegendKey = true;
            Console.WriteLine("ShowLegendKey set to: " + dataLabels.ShowLegendKey);

            // Сохраните книгу
            workbook.Save("DataLabelsShowLegendKeyDemo.xlsx");
        }
    }
}
```

### См. также

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


