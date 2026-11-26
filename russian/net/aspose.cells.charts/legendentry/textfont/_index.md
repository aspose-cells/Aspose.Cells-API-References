---
title: "LegendEntry.TextFont"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LegendEntry. Возвращает объект Font указанного объекта LegendEntry"
type: docs
url: /ru/net/aspose.cells.charts/legendentry/textfont/
---
## LegendEntry.TextFont property

Возвращает объект [`Font`](../font/) указанного объекта LegendEntry.

```csharp
[Obsolete("Use LegendEntry.Font property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual Font TextFont { get; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство LegendEntry.Font. Это свойство будет удалено через 12 месяцев, начиная с ЯНВАРЯ 2012. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LegendEntryPropertyTextFontDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["B1"].PutValue("Series 2");
            worksheet.Cells["B2"].PutValue(25);
            worksheet.Cells["B3"].PutValue(35);
            worksheet.Cells["B4"].PutValue(45);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A1:B1";

            // Включить легенду
            chart.ShowLegend = true;
            Legend legend = chart.Legend;

            // Получите доступ к первой записи легенды и измените её свойства TextFont
            LegendEntry legendEntry = legend.LegendEntries[0];
            Aspose.Cells.Font font = legendEntry.TextFont;
            
            // Установите различные свойства шрифта
            font.Name = "Arial";
            font.Size = 12;
            font.Color = Color.Red;
            font.IsBold = true;
            font.IsItalic = true;
            font.Underline = FontUnderlineType.Single;

            // Сохраните книгу
            workbook.Save("LegendEntryTextFontDemo.xlsx");
        }
    }
}
```

### См. также

* class [Font](../../../aspose.cells/font/)
* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


