---
title: "Перечисление DisplayUnitType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Charts.DisplayUnitType enum. Представляет тип единицы отображения оси диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/displayunittype/
---
## DisplayUnitType enumeration

Представляет тип единицы отображения оси диаграммы.

```csharp
public enum DisplayUnitType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Единица отображения — None. |
| Hundreds | `1` | Указывает, что значения на диаграмме должны быть разделены на 100. |
| Thousands | `2` | Указывает, что значения на диаграмме должны быть разделены на 1,000. |
| TenThousands | `3` | Указывает, что значения на диаграмме должны быть разделены на 10,000. |
| HundredThousands | `4` | Указывает, что значения на диаграмме должны быть разделены на 100,000. |
| Millions | `5` | Указывает, что значения на диаграмме должны быть разделены на 1,000,000. |
| TenMillions | `6` | Указывает, что значения на диаграмме должны быть разделены на 10,000,000. |
| HundredMillions | `7` | Указывает, что значения на диаграмме должны быть разделены на 100,000,000. |
| Billions | `8` | Указывает, что значения на диаграмме должны быть разделены на 1,000,000,000. |
| Trillions | `9` | Указывает, что значения на диаграмме должны быть разделены на 1,000,000,000,000. |
| Percentage | `10` | Значения на диаграмме должны быть разделены на 0.01. |
| Cust | `11` | указывает пользовательское значение для единицы отображения. |
| Custom | `12` | указывает пользовательское значение для единицы отображения. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class DisplayUnitTypeDemo
    {
        public static void DisplayUnitTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить новый лист в книгу
            int sheetIndex = workbook.Worksheets.Add();
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Добавить некоторые образцы данных в лист
            worksheet.Cells["A1"].PutValue(500000);
            worksheet.Cells["A2"].PutValue(1000000);
            worksheet.Cells["A3"].PutValue(1500000);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);
            
            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Добавьте NSeries (источник данных диаграммы) к диаграмме, охватывающий ячейки от "A1" до "B3"
            chart.NSeries.Add("A1:B3", true);
            
            // Установите единицу отображения оси значений в миллионы
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Millions;
            
            // Опционально показывайте метку единицы отображения
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            
            // Сохраните книгу
            workbook.Save("DisplayUnitTypeExample.xlsx");
            workbook.Save("DisplayUnitTypeExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


