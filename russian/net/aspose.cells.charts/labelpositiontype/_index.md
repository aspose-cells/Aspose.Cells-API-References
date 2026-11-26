---
title: "Перечисление LabelPositionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Charts.LabelPositionType. Представляет тип положения подписи данных"
type: docs
url: /ru/net/aspose.cells.charts/labelpositiontype/
---
## LabelPositionType enumeration

Представляет тип положения подписи данных.

```csharp
public enum LabelPositionType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Center | `0` | Применяется только к столбчатым, 2D/3D круговым диаграммам |
| InsideBase | `1` | Применяется только к столбчатым, 2D/3D круговым диаграммам |
| InsideEnd | `2` | Применяется только к столбчатым диаграммам |
| OutsideEnd | `3` | Применяется только к столбчатым, 2d/3d круговым диаграммам |
| Above | `4` | Применяется только к линейным диаграммам |
| Below | `5` | Применяется только к линейным диаграммам |
| Left | `6` | Применяется только к линейным диаграммам |
| Right | `7` | Применяется только к линейным диаграммам |
| BestFit | `8` | Применяется только к 2D/3D круговым диаграммам |
| Moved | `9` | Пользователь переместил подписи данных. Это только для чтения диаграммы из файла шаблона. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LabelPositionTypeDemo
    {
        public static void LabelPositionTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые примерные данные для диаграммы
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

            // Добавьте серию данных к диаграмме
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получите доступ к меткам данных первой серии
            DataLabels dataLabels = chart.NSeries[0].DataLabels;

            // Установить положение подписей данных
            dataLabels.Position = LabelPositionType.InsideBase;

            // Отображать название категории в подписях данных
            dataLabels.ShowCategoryName = true;

            // Отображать значение в подписях данных
            dataLabels.ShowValue = true;

            // Сохраните книгу
            workbook.Save("LabelPositionTypeExample.xlsx");
            workbook.Save("LabelPositionTypeExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


