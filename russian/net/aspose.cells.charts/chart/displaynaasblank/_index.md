---
title: "Chart.DisplayNaAsBlank"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Указывает, отображать ли N/A как пустое значение"
type: docs
url: /ru/net/aspose.cells.charts/chart/displaynaasblank/
---
## Chart.DisplayNaAsBlank property

Указывает, следует ли отображать #N/A как пустое значение.

```csharp
public bool DisplayNaAsBlank { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyDisplayNaAsBlankDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные с некоторыми значениями NA
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(double.NaN); // NA value
            worksheet.Cells["B4"].PutValue(30);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Установите свойство DisplayNaAsBlank
            chart.DisplayNaAsBlank = true;

            // Сохраните книгу
            workbook.Save("output.xlsx");

            // Проверить свойство
            Console.WriteLine("DisplayNaAsBlank is set to: " + chart.DisplayNaAsBlank);
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


