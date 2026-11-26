---
title: "ChartCollection.AddFloatingChart"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ChartCollection. Добавляет диаграмму в коллекцию"
type: docs
url: /ru/net/aspose.cells.charts/chartcollection/addfloatingchart/
---
## ChartCollection.AddFloatingChart method

Добавляет диаграмму в коллекцию.

```csharp
public int AddFloatingChart(ChartType type, int left, int top, int width, int height)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | ChartType | Тип диаграммы |
| влево | Int32 | Смещение по оси x к углу |
| верх | Int32 | Смещение по оси y к углу |
| ширина | Int32 | Ширина диаграммы |
| высота | Int32 | Высота диаграммы |

### Возвращаемое значение

[`Chart`](../../chart/) object index.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionMethodAddFloatingChartWithChartTypeInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавить плавающую диаграмму с указанными размерами
            int chartIndex = sheet.Charts.AddFloatingChart(ChartType.Column, 100, 100, 600, 400);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Добавить примерные данные в диаграмму
            chart.NSeries.Add("{1,3,2,5}", false);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


