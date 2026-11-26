---
title: "Title.X"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Title. Возвращает или задает координату X верхнего левого угла в единицах 1/4000 области диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/title/x/
---
## Title.X property

Возвращает или задает координату X верхнего левого угла в единицах 1/4000 области диаграммы.

```csharp
[Obsolete("Use Title.XRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int X { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот элемент теперь устарел. Пожалуйста, используйте свойство Title.XRatioToChart вместо него. X = XRatioToChart * 4000; Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TitlePropertyXDemo
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
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);

            // Добавить диаграмму и задать данные
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Установить свойства заголовка диаграммы с позицией X
            chart.Title.Text = "Sample Chart";
            chart.Title.X = 200; // Demonstrating X property usage
            chart.Title.Y = 50;

            // Сохраните книгу
            workbook.Save("TitlePropertyXDemo.xlsx");
        }
    }
}
```

### См. также

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


