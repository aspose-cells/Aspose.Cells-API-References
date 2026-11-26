---
title: "Класс Area"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.Area. Инкапсулирует объект, представляющий формат области"
type: docs
url: /ru/net/aspose.cells.drawing/area/
---
## Area class

Инкапсулирует объект, представляющий формат области.

```csharp
public class Area
```

## Свойства

| Имя | Описание |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor/) { get; set; } | Получает или задает фоновый цвет `Area`. |
| [FillFormat](../../aspose.cells.drawing/area/fillformat/) { get; } | Представляет объект [`FillFormat`](./fillformat/), содержащий свойства форматирования заливки для указанной диаграммы или фигуры. |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor/) { get; set; } | Получает или задает цвет переднего плана. |
| [Formatting](../../aspose.cells.drawing/area/formatting/) { get; set; } | Представляет форматирование области. |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative/) { get; set; } | Если свойство истинно и значение точки диаграммы отрицательное, цвета переднего плана и фона будут обменены. |
| [Transparency](../../aspose.cells.drawing/area/transparency/) { get; set; } | Возвращает или задает степень прозрачности области значением от 0.0 (непрозрачный) до 1.0 (прозрачный). |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class AreaDemo
    {
        public static void AreaExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();
            // Добавление нового листа в объект Workbook
            int sheetIndex = workbook.Worksheets.Add();
            // Получение ссылки на только что добавленный лист путем передачи его индекса листа
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Добавление образцовых значений в ячейки
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(-100);
            worksheet.Cells["A3"].PutValue(150);
            // Добавление диаграммы в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Area, 5, 0, 15, 5);
            // Получение экземпляра недавно добавленной диаграммы
            Chart chart = worksheet.Charts[chartIndex];
            // Добавление NSeries (источник данных диаграммы) к диаграмме в диапазоне от ячейки "A1" до "A3"
            chart.NSeries.Add("A1:A3", true);

            // Доступ к области первого NSeries
            Area area = chart.NSeries[0].Area;

            // Установка свойств
            area.InvertIfNegative = true;
            area.ForegroundColor = Color.Red;
            area.BackgroundColor = Color.Yellow;
            area.Formatting = Aspose.Cells.Charts.FormattingType.Custom;
            area.Transparency = 0.5;

            // Сохранение файла Excel
            workbook.Save("AreaExample.xlsx");
            workbook.Save("AreaExample.pdf");

        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


