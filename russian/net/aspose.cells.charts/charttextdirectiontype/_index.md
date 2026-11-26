---
title: "Перечисление ChartTextDirectionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Charts.ChartTextDirectionType. Представляет тип направления текста диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/charttextdirectiontype/
---
## ChartTextDirectionType enumeration

Представляет тип направления текста в диаграмме.

```csharp
public enum ChartTextDirectionType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Horizontal | `0` | Тип горизонтального направления. |
| Vertical | `1` | Тип вертикального направления. |
| Rotate90 | `2` | Поверните на девяносто градусов. |
| Rotate270 | `3` | Поверните на 270 градусов. |
| Stacked | `4` | Сложенный текст. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartTextDirectionTypeDemo
    {
        public static void ChartTextDirectionTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в лист
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
            
            // Добавьте серию данных в диаграмму
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Установить заголовок диаграммы
            chart.Title.Text = "Sample Chart";
            chart.Title.Font.Color = Color.Blue;
            
            // Установите направление текста заголовка диаграммы
            chart.Title.DirectionType = ChartTextDirectionType.Rotate90;
            
            // Установите направление текста заголовка оси категорий
            chart.CategoryAxis.Title.Text = "Categories";
            chart.CategoryAxis.Title.DirectionType = ChartTextDirectionType.Vertical;
            
            // Установите направление текста заголовка оси значений
            chart.ValueAxis.Title.Text = "Values";
            chart.ValueAxis.Title.DirectionType = ChartTextDirectionType.Horizontal;
            
            // Сохраните книгу
            workbook.Save("ChartTextDirectionTypeExample.xlsx");
            workbook.Save("ChartTextDirectionTypeExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


