---
title: "Перечисление TextAlignmentType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.TextAlignmentType. Перечисляет типы выравнивания текста"
type: docs
url: /ru/net/aspose.cells/textalignmenttype/
---
## TextAlignmentType enumeration

Перечисляет типы выравнивания текста.

```csharp
public enum TextAlignmentType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| General | `1792` | Представляет общее выравнивание текста. |
| Bottom | `528` | Представляет выравнивание текста по нижнему краю. |
| Center | `1802` | Представляет выравнивание текста по центру. |
| CenterAcross | `1286` | Представляет выравнивание текста по центру по ширине. |
| Distributed | `807` | Представляет распределённое выравнивание текста. |
| Fill | `1284` | Представляет выравнивание текста заполнением. |
| Justify | `1821` | Представляет выравнивание текста по ширине. |
| Left | `257` | Представляет выравнивание текста по левому краю |
| Right | `259` | Представляет выравнивание текста по правому краю. |
| Top | `512` | Представляет выравнивание текста по верхнему краю. |
| JustifiedLow | `832` | Выравнивает текст с отрегулированной длиной кашиды для арабского текста. |
| ThaiDistributed | `896` | Особым образом распределяет тайский текст, поскольку каждый символ рассматривается как слово. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TextAlignmentTypeDemo
    {
        public static void TextAlignmentTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["B3"].PutValue(90);
            worksheet.Cells["B4"].PutValue(78);

            // Добавить комментарий к ячейке
            Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
            comment.Note = "This is a comment.";
            comment.TextHorizontalAlignment = TextAlignmentType.Center;
            comment.TextVerticalAlignment = TextAlignmentType.Top;

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.SetChartDataRange("A1:B4", true);

            // Настроить заголовок диаграммы
            chart.Title.Text = "Scores Chart";
            chart.Title.TextHorizontalAlignment = TextAlignmentType.Center;
            chart.Title.TextVerticalAlignment = TextAlignmentType.Top;

            // Сохраните книгу
            workbook.Save("TextAlignmentTypeExample.xlsx");

            // Выведите результаты
            Console.WriteLine("Workbook saved successfully with text alignment settings.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


