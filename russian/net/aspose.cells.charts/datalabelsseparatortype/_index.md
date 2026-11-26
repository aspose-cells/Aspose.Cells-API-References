---
title: "Перечисление DataLabelsSeparatorType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Charts.DataLabelsSeparatorType. Представляет тип разделителя для DataLabels"
type: docs
url: /ru/net/aspose.cells.charts/datalabelsseparatortype/
---
## DataLabelsSeparatorType enumeration

Представляет тип разделителя для подписей данных.

```csharp
public enum DataLabelsSeparatorType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Auto | `0` | Представляет автоматический разделитель |
| Space | `1` | Представляет пробел(" ") |
| Comma | `2` | Представляет запятую(",") |
| Semicolon | `3` | Представляет точку с запятой(";") |
| Period | `4` | Представляет точку(".") |
| NewLine | `5` | Представляет перевод строки("\n") |
| Custom | `6` | Представляет пользовательский разделитель |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class DataLabelsSeparatorTypeDemo
    {
        public static void DataLabelsSeparatorTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные для диаграммы
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

            // Добавьте серию данных к диаграмме
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получите доступ к меткам данных первой серии
            DataLabels dataLabels = chart.NSeries[0].DataLabels;

            // Установите тип разделителя в запятую
            dataLabels.SeparatorType = DataLabelsSeparatorType.Comma;

            // Включите подписи данных и задайте некоторые свойства
            dataLabels.ShowCategoryName = true;
            dataLabels.ShowValue = true;
            dataLabels.Position = LabelPositionType.InsideBase;

            // Установите свойства шрифта
            dataLabels.Font.Color = Color.Blue;
            dataLabels.Font.IsBold = true;

            // Сохраните книгу
            workbook.Save("DataLabelsSeparatorTypeExample.xlsx");
            workbook.Save("DataLabelsSeparatorTypeExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


