---
title: "Перечисление PageLayoutAlignmentType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.PageLayoutAlignmentType перечисление. Перечисляет типы выравнивания макета страницы."
type: docs
url: /ru/net/aspose.cells/pagelayoutalignmenttype/
---
## PageLayoutAlignmentType enumeration

Перечисляет типы выравнивания макета страницы.

```csharp
public enum PageLayoutAlignmentType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Bottom | `0` | Представляет выравнивание нижней части макета страницы. |
| Center | `1` | Представляет выравнивание по центру макета страницы. |
| Left | `2` | Представляет выравнивание слева макета страницы. |
| Right | `3` | Представляет выравнивание справа макета страницы. |
| Top | `4` | Представляет выравнивание верхней части макета страницы. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PageLayoutAlignmentTypeDemo
    {
        public static void PageLayoutAlignmentTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые образцы данных в лист
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);
            worksheet.Cells["A4"].PutValue(789);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных для диаграммы
            chart.SetChartDataRange("A1:A4", true);

            // Установить заголовок диаграммы
            chart.Title.Text = "Sample Chart";

            // Сохранить книгу в файл
            workbook.Save("PageLayoutAlignmentTypeExample.xlsx");

            // Экспортировать диаграмму в PDF с определённым выравниванием макета страницы
            chart.ToPdf("ChartExample.pdf", 8.5f, 11f, PageLayoutAlignmentType.Center, PageLayoutAlignmentType.Center);

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


