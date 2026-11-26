---
title: "ChartFrame.Height"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartFrame. Возвращает или задает высоту кадра в единицах 1/4000 области диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chartframe/height/
---
## ChartFrame.Height property

Возвращает или задает высоту кадра в единицах 1/4000 области диаграммы.

```csharp
[Obsolete("Use ChartFrame.HeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int Height { get; set; }
```

### Примечания

Как преобразовать единицы 1/4000 в пиксели? Высота в пикселях = Y * Chart.ChartObject.Height / 4000d;

ПРИМЕЧАНИЕ: Этот элемент теперь устарел. Пожалуйста, используйте свойство ChartFrame.HeightRatioToChart. Height = HeightRatioToChart * 4000. Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyHeightDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
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
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получить доступ к меткам данных
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            
            // Установить свойство Height
            dataLabels.Height = 200; // Set height to 200 pixels
            
            // Отобразить значение высоты
            Console.WriteLine("DataLabels Height: " + dataLabels.Height);
            
            // Сохраните книгу
            workbook.Save("ChartFramePropertyHeightDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


