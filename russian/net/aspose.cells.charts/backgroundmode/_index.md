---
title: "Перечисление BackgroundMode"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Charts.BackgroundMode. Представляет режим отображения фона"
type: docs
url: /ru/net/aspose.cells.charts/backgroundmode/
---
## BackgroundMode enumeration

Представляет режим отображения фона.

```csharp
public enum BackgroundMode
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Automatic | `0` | Автоматически |
| Opaque | `1` | Непрозрачный |
| Transparent | `2` | Прозрачный |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class BackgroundModeDemo
    {
        public static void BackgroundModeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить ссылку на первый лист
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные в ячейки
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            
            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Добавьте NSeries (источник данных диаграммы) к диаграмме, охватывающий ячейки от "A1" до "B3"
            chart.NSeries.Add("A1:B3", true);
            
            // Получите доступ к области диаграммы
            ChartArea chartArea = chart.ChartArea;

            // Установите цвет переднего плана области диаграммы
            chartArea.Area.ForegroundColor = Color.Yellow;

            // Установите режим фона области диаграммы
            chartArea.BackgroundMode = BackgroundMode.Opaque;
            chartArea.Area.Transparency = 0.8;           
            
            
            // Установите тень области диаграммы
            chartArea.Shadow = true;
            
            // Сохраните книгу
            workbook.Save("BackgroundModeExample.xlsx");
            workbook.Save("BackgroundModeExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


