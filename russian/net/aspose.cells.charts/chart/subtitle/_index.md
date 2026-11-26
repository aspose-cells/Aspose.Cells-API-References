---
title: "Chart.SubTitle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Получает подзаголовок диаграммы. Применяется только к файлам ODS"
type: docs
url: /ru/net/aspose.cells.charts/chart/subtitle/
---
## Chart.SubTitle property

Получает подзаголовок диаграммы. Применяется только к файлам ODS.

```csharp
public Title SubTitle { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertySubTitleDemo
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

            // Добавьте диаграмму и задайте её диапазон данных
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Установите основной заголовок
            chart.Title.Text = "Main Chart Title";

            // Установите подзаголовок
            chart.SubTitle.Text = "Chart Subtitle";
            chart.SubTitle.Font.Size = 12;
            chart.SubTitle.Font.IsBold = true;

            // Сохраните книгу
            workbook.Save("ChartWithSubtitle.xlsx");
        }
    }
}
```

### См. также

* class [Title](../../title/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


