---
title: "DataLabels.Number"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataLabels. Получает и задает встроенный числовой формат"
type: docs
url: /ru/net/aspose.cells.charts/datalabels/number/
---
## DataLabels.Number property

Получает и задает встроенный числовой формат.

```csharp
public int Number { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyNumberDemo
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

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Bar, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получите первую серию и включите метки данных
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            
            // Получите доступ к свойствам меток данных
            DataLabels dataLabels = series.DataLabels;
            
            // Продемонстрируйте использование свойства Number
            Console.WriteLine("Original Number format: " + dataLabels.NumberFormat);
            Console.WriteLine("Original Number property value: " + dataLabels.Number);
            
            // Измените числовой формат
            dataLabels.Number = 2; // Currency format
            dataLabels.NumberFormat = "$#,##0.00";
            
            Console.WriteLine("Modified Number format: " + dataLabels.NumberFormat);
            Console.WriteLine("Modified Number property value: " + dataLabels.Number);

            // Сохраните книгу
            workbook.Save("DataLabelsNumberDemo.xlsx");
        }
    }
}
```

### См. также

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


