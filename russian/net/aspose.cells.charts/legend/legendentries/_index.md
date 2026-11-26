---
title: "Legend.LegendEntries"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Legend. Возвращает коллекцию всех объектов LegendEntry в указанной легенде диаграммы. Установка элементов легенды для поверхностной диаграммы не поддерживается. Поэтому будет возвращено null, если тип диаграммы — surface chart type"
type: docs
url: /ru/net/aspose.cells.charts/legend/legendentries/
---
## Legend.LegendEntries property

Получает коллекцию всех объектов LegendEntry в указанной легенде диаграммы. Установка записей легенды для поверхностной диаграммы не поддерживается. Поэтому будет возвращено null, если тип диаграммы — поверхностный.

```csharp
public LegendEntryCollection LegendEntries { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendPropertyLegendEntriesDemo
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

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.CategoryData = "B2:B4";

            // Получите доступ к элементам легенды
            Aspose.Cells.Charts.LegendEntryCollection legendEntries = chart.Legend.LegendEntries;
            
            // Удалить второй элемент легенды
            legendEntries[1].IsDeleted = true;
            
            // Сохраните книгу
            workbook.Save("LegendEntriesDemo.xlsx");
        }
    }
}
```

### См. также

* class [LegendEntryCollection](../../legendentrycollection/)
* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


