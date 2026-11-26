---
title: "DataLabels.IsNeverOverlap"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataLabels. Указывает, никогда ли подписи данных не перекрываются при преобразовании круговой диаграммы в изображение. Обратите внимание, что это свойство имеет смысл только при преобразовании круговой диаграммы в изображение."
type: docs
url: /ru/net/aspose.cells.charts/datalabels/isneveroverlap/
---
## DataLabels.IsNeverOverlap property

Указывает, будет ли Datalabels никогда не перекрываться при преобразовании круговой диаграммы в изображение. Примечание: это свойство имеет смысл только при преобразовании круговой диаграммы в изображение.

```csharp
public bool IsNeverOverlap { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyIsNeverOverlapDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавить столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Включить подписи данных
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;

            // Получить подписи данных и установить свойство IsNeverOverlap
            DataLabels dataLabels = series.DataLabels;
            Console.WriteLine("Default IsNeverOverlap value: " + dataLabels.IsNeverOverlap);
            
            // Установить IsNeverOverlap в значение true
            dataLabels.IsNeverOverlap = true;
            Console.WriteLine("After setting IsNeverOverlap: " + dataLabels.IsNeverOverlap);

            // Сохраните книгу
            workbook.Save("DataLabelsIsNeverOverlapDemo.xlsx");
        }
    }
}
```

### См. также

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


