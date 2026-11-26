---
title: "SeriesLayoutProperties.ShowMeanLine"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SeriesLayoutProperties. Указывает, показывать ли линию, соединяющую все средние точки"
type: docs
url: /ru/net/aspose.cells.charts/serieslayoutproperties/showmeanline/
---
## SeriesLayoutProperties.ShowMeanLine property

Указывает, следует ли отображать линию, соединяющую все средние точки.

```csharp
public bool ShowMeanLine { get; set; }
```

### Примечания

Работает только для диаграммы BoxWhisker.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyShowMeanLineDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы box and whisker
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(40);
            worksheet.Cells["A4"].PutValue(25);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["A6"].PutValue(115);
            worksheet.Cells["A7"].PutValue(65.666);

            // Добавить диаграмму box and whisker
            int chartIndex = worksheet.Charts.Add(ChartType.BoxWhisker, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Добавить серию к диаграмме
            chart.NSeries.Add("A1:A7", true);

            // Получить первую серию
            Series series = chart.NSeries[0];

            // Получить доступ к свойствам макета
            SeriesLayoutProperties layout = series.LayoutProperties;

            // Продемонстрировать свойство ShowMeanLine
            Console.WriteLine("Default ShowMeanLine value: " + layout.ShowMeanLine);
            
            // Установить ShowMeanLine в true
            layout.ShowMeanLine = true;
            Console.WriteLine("After setting ShowMeanLine to true: " + layout.ShowMeanLine);

            // Сохраните книгу
            workbook.Save("BoxWhiskerChart_ShowMeanLineDemo.xlsx");
        }
    }
}
```

### См. также

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


