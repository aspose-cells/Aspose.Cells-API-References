---
title: "Chart.SwitchRowColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Chart. Переключает строки/столбцы"
type: docs
url: /ru/net/aspose.cells.charts/chart/switchrowcolumn/
---
## Chart.SwitchRowColumn method

Переключает строки/столбцы.

```csharp
public bool SwitchRowColumn()
```

### Возвращаемое значение

False означает, что переключение строк/столбцов не удалось.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodSwitchRowColumnDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["C2"].PutValue(150);
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["C3"].PutValue(250);
            worksheet.Cells["A4"].PutValue("Item 3");
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["C4"].PutValue(350);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.SetChartDataRange("A1:C4", true);
            
            // Показать оригинальные значения серий
            Console.WriteLine("Before SwitchRowColumn:");
            Console.WriteLine("Series 1 Values: " + chart.NSeries[0].Values);
            
            // Переключить строки/столбцы
            chart.SwitchRowColumn();
            
            // Показать значения рядов после переключения
            Console.WriteLine("\nAfter SwitchRowColumn:");
            Console.WriteLine("Series 1 Values: " + chart.NSeries[0].Values);
            
            // Сохраните книгу
            workbook.Save("SwitchRowColumnDemo.xlsx");
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


