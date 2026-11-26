---
title: "Класс LegendEntry"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Charts.LegendEntry. Представляет запись легенды в легенде диаграммы."
type: docs
url: /ru/net/aspose.cells.charts/legendentry/
---
## LegendEntry class

Представляет элемент легенды в легенде диаграммы.

```csharp
public class LegendEntry
```

## Свойства

| Имя | Описание |
| --- | --- |
| [AutoScaleFont](../../aspose.cells.charts/legendentry/autoscalefont/) { get; set; } | True, если текст в объекте изменяет размер шрифта при изменении размера объекта. Значение по умолчанию — True. |
| [Background](../../aspose.cells.charts/legendentry/background/) { get; set; } | (**Obsolete.**) Получает и задает режим отображения фона |
| [BackgroundMode](../../aspose.cells.charts/legendentry/backgroundmode/) { get; set; } | Получает и задает режим отображения фона |
| [Font](../../aspose.cells.charts/legendentry/font/) { get; } | Получает объект [`Font`](./font/) указанного объекта ChartFrame. |
| [IsDeleted](../../aspose.cells.charts/legendentry/isdeleted/) { get; set; } | Получает и задает, удалена ли запись легенды. |
| [IsTextNoFill](../../aspose.cells.charts/legendentry/istextnofill/) { get; set; } | Получает или задает отсутствие заливки текста. |
| virtual [TextFont](../../aspose.cells.charts/legendentry/textfont/) { get; } | (**Obsolete.**) Получает объект [`Font`](./font/) указанного объекта LegendEntry. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LegendEntryDemo
    {
        public static void LegendEntryExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Добавить NSeries (источник данных диаграммы) к диаграмме, охватывающей ячейки от "A1" до "B4"
            chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";

            // Получить запись легенды первой серии
            LegendEntry legendEntry = chart.NSeries[0].LegendEntry;

            // Установить свойства записи легенды
            legendEntry.IsDeleted = false;
            legendEntry.IsTextNoFill = false;
            legendEntry.AutoScaleFont = true;
            legendEntry.Background = BackgroundMode.Transparent;
            legendEntry.BackgroundMode = BackgroundMode.Opaque;

            // Получить доступ и изменить шрифт записи легенды
            Font font = legendEntry.Font;
            font.Name = "Arial";
            font.Size = 12;
            font.IsBold = true;
            font.Color = System.Drawing.Color.Blue;

            // Сохраните книгу
            workbook.Save("LegendEntryExample.xlsx");
            workbook.Save("LegendEntryExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


