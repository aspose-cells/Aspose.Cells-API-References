---
title: "Chart.PrintSize"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Получает и задает размер печатной диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chart/printsize/
---
## Chart.PrintSize property

Получает и задает размер печатной диаграммы.

```csharp
public PrintSizeType PrintSize { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPrintSizeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Настроить параметры печати
            chart.PrintSize = PrintSizeType.Full;
            chart.SizeWithWindow = false;
            chart.AutoScaling = false;

            // Сохраните книгу
            workbook.Save("ChartPrintSizeDemo.pdf", SaveFormat.Pdf);
        }
    }
}
```

### См. также

* enum [PrintSizeType](../../../aspose.cells/printsizetype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


