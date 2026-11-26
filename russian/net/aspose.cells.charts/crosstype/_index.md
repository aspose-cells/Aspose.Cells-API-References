---
title: "Перечисление CrossType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Charts.CrossType. Представляет тип пересечения оси"
type: docs
url: /ru/net/aspose.cells.charts/crosstype/
---
## CrossType enumeration

Представляет тип пересечения осей.

```csharp
public enum CrossType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Automatic | `0` | Microsoft Excel задает точку пересечения оси. |
| Maximum | `1` | Ось пересекается в максимальном значении. |
| Minimum | `2` | Ось пересекает минимальное значение. |
| Custom | `3` | Ось пересекает пользовательское значение. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class CrossTypeDemo
    {
        public static void CrossTypeExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();
            // Добавление нового листа к объекту Excel
            int sheetIndex = workbook.Worksheets.Add();
            // Получение ссылки на только что добавленный лист путем передачи его индекса листа
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Добавление образцовых значений в ячейки
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Добавление диаграммы в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            // Получение экземпляра недавно добавленной диаграммы
            Chart chart = worksheet.Charts[chartIndex];
            // Добавление NSeries (источника данных диаграммы) к диаграмме в диапазоне от ячейки "A1" до "B3"
            chart.NSeries.Add("A1:B3", true);

            // Установите максимальное значение оси значений
            chart.ValueAxis.MaxValue = 200;
            // Установите минимальное значение оси значений
            chart.ValueAxis.MinValue = 0;
            // Установите основной интервал
            chart.ValueAxis.MajorUnit = 25;

            // Ось Category(X) пересекает максимальное значение
            chart.ValueAxis.CrossType = CrossType.Maximum;

            // Установите количество категорий или рядов между метками делений
            chart.CategoryAxis.TickLabelSpacing = 2;

            // Сохранение файла Excel
            workbook.Save("CrossTypeExample.xlsx");
            workbook.Save("CrossTypeExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


