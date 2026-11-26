---
title: "Enum PrintSizeType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.PrintSizeType enum. Представляет размер печатной диаграммы"
type: docs
url: /ru/net/aspose.cells/printsizetype/
---
## PrintSizeType enumeration

Представляет размер печатного графика.

```csharp
public enum PrintSizeType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Full | `0` | Использовать полную страницу. |
| Fit | `1` | Масштабировать под страницу. |
| Custom | `2` | Пользовательский. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PrintSizeTypeDemo
    {
        public static void PrintSizeTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            // Получить первый лист
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells[0, 0].PutValue("Category");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);
            worksheet.Cells[3, 0].PutValue("C");
            worksheet.Cells[3, 1].PutValue(30);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных для диаграммы
            chart.SetChartDataRange("A1:B4", true);

            // Установить заголовок диаграммы
            chart.Title.Text = "Sample Chart";

            // Установить размер печати диаграммы
            chart.PrintSize = PrintSizeType.Fit;

            // Сохраните книгу
            workbook.Save("PrintSizeTypeExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


