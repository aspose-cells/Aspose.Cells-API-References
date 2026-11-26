---
title: "ChartPoint.YValueType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartPoint. Возвращает тип значения Y точки диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chartpoint/yvaluetype/
---
## ChartPoint.YValueType property

Получает тип значения Y chartpoint.

```csharp
public CellValueType YValueType { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyYValueTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получить первую точку диаграммы в первой серии
            ChartPoint chartPoint = chart.NSeries[0].Points[0];

            // Отобразить текущий YValueType
            Console.WriteLine("Current YValueType: " + chartPoint.YValueType);

            // Отобразить YValue до изменения
            Console.WriteLine("Current YValue: " + chartPoint.YValue);

            // Изменить YValue на другой тип (string, чтобы продемонстрировать изменение типа)
            chartPoint.YValue = "15"; // This will change the YValueType to IsString

            // Отобразить YValueType после изменения
            Console.WriteLine("New YValueType: " + chartPoint.YValueType);
            Console.WriteLine("New YValue: " + chartPoint.YValue);

            // Сохраните книгу
            workbook.Save("ChartPointPropertyYValueTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [CellValueType](../../../aspose.cells/cellvaluetype/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


