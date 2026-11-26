---
title: "Класс TickLabels"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Charts.TickLabels. Представляет подписи делений, связанные с делениями на оси диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/ticklabels/
---
## TickLabels class

Представляет подписи делений, связанные с делениями на оси диаграммы.

```csharp
public class TickLabels
```

## Свойства

| Имя | Описание |
| --- | --- |
| [AlignmentType](../../aspose.cells.charts/ticklabels/alignmenttype/) { get; set; } | Получает и задает выравнивание текста для подписей делений на оси. |
| [AutoScaleFont](../../aspose.cells.charts/ticklabels/autoscalefont/) { get; set; } | True, если текст в объекте изменяет размер шрифта при изменении размера объекта. Значение по умолчанию — True. |
| [BackgroundMode](../../aspose.cells.charts/ticklabels/backgroundmode/) { get; set; } | Получает и задает режим отображения фона |
| [DirectionType](../../aspose.cells.charts/ticklabels/directiontype/) { get; set; } | Получает и задает направление текста. |
| [DisplayNumberFormat](../../aspose.cells.charts/ticklabels/displaynumberformat/) { get; } | Получает и задает формат отображения чисел для подписей делений. |
| [Font](../../aspose.cells.charts/ticklabels/font/) { get; } | Возвращает объект [`Font`](./font/), который представляет шрифт указанного объекта TickLabels. |
| [IsAutomaticRotation](../../aspose.cells.charts/ticklabels/isautomaticrotation/) { get; set; } | Указывает, является ли угол поворота автоматическим |
| [Number](../../aspose.cells.charts/ticklabels/number/) { get; set; } | Представляет номер формата для объекта TickLabels. |
| [NumberFormat](../../aspose.cells.charts/ticklabels/numberformat/) { get; set; } | Представляет строку формата для объекта TickLabels. |
| [NumberFormatLinked](../../aspose.cells.charts/ticklabels/numberformatlinked/) { get; set; } | True, если числовой формат связан с ячейками (чтобы формат числа менялся в метках, когда он меняется в ячейках). |
| [Offset](../../aspose.cells.charts/ticklabels/offset/) { get; set; } | Получает и задает расстояние подписей от оси категорий. Это применимо только к оси категорий (x). |
| [ReadingOrder](../../aspose.cells.charts/ticklabels/readingorder/) { get; set; } | Представляет порядок чтения текста. |
| [RotationAngle](../../aspose.cells.charts/ticklabels/rotationangle/) { get; set; } | Представляет угол поворота текста по часовой стрелке. |
| [TextDirection](../../aspose.cells.charts/ticklabels/textdirection/) { get; set; } | (**Obsolete.**) Представляет порядок чтения текста. |
| [TickLabelItems](../../aspose.cells.charts/ticklabels/ticklabelitems/) { get; } | Получает отображаемые подписи делений оси. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TickLabelsDemo
    {
        public static void TickLabelsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
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

            // Доступ к оси значений
            Axis valueAxis = chart.ValueAxis;

            // Доступ к подписям делений оси значений
            TickLabels tickLabels = valueAxis.TickLabels;

            // Установить свойства подписей делений
            tickLabels.AutoScaleFont = true;
            tickLabels.BackgroundMode = BackgroundMode.Transparent;
            tickLabels.RotationAngle = 45;
            tickLabels.IsAutomaticRotation = false;
            tickLabels.NumberFormat = "0.00";
            tickLabels.Number = 2;
            tickLabels.NumberFormatLinked = true;
            tickLabels.Offset = 100;
            tickLabels.TextDirection = TextDirectionType.LeftToRight;
            tickLabels.ReadingOrder = TextDirectionType.LeftToRight;
            tickLabels.DirectionType = ChartTextDirectionType.Horizontal;
            tickLabels.AlignmentType = TickLabelAlignmentType.Center;

            // Сохраните книгу
            workbook.Save("TickLabelsExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


