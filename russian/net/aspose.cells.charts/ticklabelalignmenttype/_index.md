---
title: "Перечисление TickLabelAlignmentType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Charts.TickLabelAlignmentType. Представляет тип выравнивания текста для меток делений на оси."
type: docs
url: /ru/net/aspose.cells.charts/ticklabelalignmenttype/
---
## TickLabelAlignmentType enumeration

Представляет тип выравнивания текста для меток делений на оси

```csharp
public enum TickLabelAlignmentType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Center | `0` | Указывает, что текст выровнен по центру. |
| Left | `1` | Указывает, что текст выровнен по левому краю. |
| Right | `2` | Указывает, что текст выровнен по правому краю.. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TickLabelAlignmentTypeDemo
    {
        public static void TickLabelAlignmentTypeExample()
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

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Добавить серию к диаграмме
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получить доступ к меткам делений оси категорий
            TickLabels tickLabels = chart.CategoryAxis.TickLabels;

            // Установить тип выравнивания для меток делений
            tickLabels.AlignmentType = TickLabelAlignmentType.Center;

            // Сохраните книгу
            workbook.Save("TickLabelAlignmentTypeExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


