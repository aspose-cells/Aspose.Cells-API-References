---
title: "Перечисление TickLabelPositionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Charts.TickLabelPositionType. Представляет тип положения меток делений на указанной оси"
type: docs
url: /ru/net/aspose.cells.charts/ticklabelpositiontype/
---
## TickLabelPositionType enumeration

Представляет тип положения меток делений на указанной оси.

```csharp
public enum TickLabelPositionType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| High | `0` | Тип положения — высокий. |
| Low | `1` | Тип положения — низкий. |
| NextToAxis | `2` | Тип положения — рядом с осью. |
| None | `3` | Тип положения — отсутствует. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TickLabelPositionTypeDemo
    {
        public static void TickLabelPositionTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить некоторые образцы данных в лист
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);
            
            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Добавьте NSeries (источник данных диаграммы) к диаграмме, охватывающий ячейки от "A1" до "B3"
            chart.NSeries.Add("A1:B3", true);
            
            // Получите доступ к категориальной оси
            Axis categoryAxis = chart.CategoryAxis;
            
            // Установите положение метки деления в значение High
            categoryAxis.TickLabelPosition = TickLabelPositionType.High;
            
            // Сохраните книгу
            workbook.Save("TickLabelPositionTypeExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


