---
title: "Перечисление FormattingType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Charts.FormattingType. Представляет тип форматирования, применяемый к объекту Area или объекту Line."
type: docs
url: /ru/net/aspose.cells.charts/formattingtype/
---
## FormattingType enumeration

Представляет тип форматирования, применяемый к объекту [`Area`](../../aspose.cells.drawing/area/) или объекту [`Line`](../../aspose.cells.drawing/line/).

```csharp
public enum FormattingType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Automatic | `0` | Представляет тип автоматического форматирования. |
| Custom | `2` | Представляет пользовательский тип форматирования. |
| None | `1` | Представляет тип отсутствующего форматирования. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class FormattingTypeDemo
    {
        public static void FormattingTypeExample()
        {
            // Создайте объект Workbook
            Workbook workbook = new Workbook();
            
            // Добавление нового листа в объект Workbook
            int sheetIndex = workbook.Worksheets.Add();
            
            // Получение ссылки на только что добавленный лист путем передачи его индекса листа
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Добавление образцовых значений в ячейки
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            
            // Добавление диаграммы в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            
            // Получение экземпляра недавно добавленной диаграммы
            Chart chart = worksheet.Charts[chartIndex];
            
            // Добавление NSeries (источника данных диаграммы) к диаграмме в диапазоне от ячейки "A1" до "B3"
            chart.NSeries.Add("A1:B3", true);
            
            // Установка цвета переднего плана области построения
            chart.PlotArea.Area.ForegroundColor = Color.Blue;
            chart.PlotArea.Area.Formatting = FormattingType.Custom;
            
            // Установка цвета переднего плана области диаграммы
            chart.ChartArea.Area.ForegroundColor = Color.Yellow;
            chart.ChartArea.Area.Formatting = FormattingType.Automatic;
            
            // Установка цвета переднего плана области первой серии NSeries
            chart.NSeries[0].Area.ForegroundColor = Color.Red;
            chart.NSeries[0].Area.Formatting = FormattingType.None;
            
            // Установка цвета переднего плана области первой точки серии NSeries
            chart.NSeries[0].Points[0].Area.ForegroundColor = Color.Cyan;
            chart.NSeries[0].Points[0].Area.Formatting = FormattingType.Custom;
            
            // Сохранение файла Excel
            workbook.Save("FormattingTypeExample.xlsx");
            workbook.Save("FormattingTypeExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


