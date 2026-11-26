---
title: "Chart.Worksheet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Получает лист, содержащий эту диаграмму"
type: docs
url: /ru/net/aspose.cells.charts/chart/worksheet/
---
## Chart.Worksheet property

Получает лист, содержащий эту диаграмму.

```csharp
public Worksheet Worksheet { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyWorksheetDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
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
            
            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Продемонстрировать использование свойства Worksheet
            Console.WriteLine("Chart's worksheet index: " + chart.Worksheet.Index);
            Console.WriteLine("Chart's worksheet name: " + chart.Worksheet.Name);
            
            // Сохраните книгу
            workbook.Save("ChartPropertyWorksheetDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


