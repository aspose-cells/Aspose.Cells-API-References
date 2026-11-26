---
title: "ChartFrame.Background"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartFrame. Получает и задает режим отображения фона. Это свойство действительно только в Excel 2003 и более ранних версиях."
type: docs
url: /ru/net/aspose.cells.charts/chartframe/background/
---
## ChartFrame.Background property

Получает и задает режим отображения фона. Это свойство действительно только в Excel 2003 и более ранних версиях.

```csharp
[Obsolete("Use ChartFrame.Area.FillFormat.FillType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public BackgroundMode Background { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство ChartFrame.Area.FillFormat.FillType. Например, если вам нужно установить BackgroundMode в Opaque, вы можете использовать следующий код: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Это свойство будет удалено через 12 месяцев, начиная с ЯНВАРЯ 2012. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyBackgroundDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Настройте данные диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Настройте подписи данных с параметрами фона
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;
            dataLabels.Background = BackgroundMode.Transparent;

            // Сохраните книгу
            workbook.Save("ChartBackgroundDemo.xlsx");
        }
    }
}
```

### См. также

* enum [BackgroundMode](../../backgroundmode/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


