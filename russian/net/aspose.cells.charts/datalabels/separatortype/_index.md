---
title: "DataLabels.SeparatorType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataLabels. Получает или задает тип разделителя, используемого для подписей данных на диаграмме"
type: docs
url: /ru/net/aspose.cells.charts/datalabels/separatortype/
---
## DataLabels.SeparatorType property

Получает или задает тип разделителя, используемого для меток данных на диаграмме.

```csharp
public DataLabelsSeparatorType SeparatorType { get; set; }
```

### Примечания

Чтобы задать пользовательский разделитель, пожалуйста, установите свойство `SeparatorType` в значение Custom, а затем укажите ожидаемое значение для [`SeparatorValue`](../separatorvalue/).

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertySeparatorTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Добавьте диаграмму
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Включить подписи данных
            chart.NSeries[0].DataLabels.ShowValue = true;
            chart.NSeries[0].DataLabels.ShowCategoryName = true;
            
            // Задать тип разделителя
            chart.NSeries[0].DataLabels.SeparatorType = DataLabelsSeparatorType.Space;

            // Сохраните книгу
            workbook.Save("DataLabelsSeparatorTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [DataLabelsSeparatorType](../../datalabelsseparatortype/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


