---
title: "Перечисление Bar3DShapeType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Charts.Bar3DShapeType enum. Представляет форму, используемую в 3D столбчатой или колонковой диаграмме"
type: docs
url: /ru/net/aspose.cells.charts/bar3dshapetype/
---
## Bar3DShapeType enumeration

Представляет форму, используемую в 3‑D гистограмме или столбчатой диаграмме.

```csharp
public enum Bar3DShapeType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Box | `0` | Коробка |
| PyramidToPoint | `1` | PyramidToPoint |
| PyramidToMax | `2` | PyramidToMax |
| Cylinder | `3` | Цилиндр |
| ConeToPoint | `4` | ConeToPoint |
| ConeToMax | `5` | ConeToMax |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class Bar3DShapeTypeDemo
    {
        public static void Bar3DShapeTypeExample()
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
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Добавление диаграммы в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column3DClustered, 5, 0, 15, 5);
            // Получение экземпляра недавно добавленной диаграммы
            Chart chart = worksheet.Charts[chartIndex];
            // Добавление NSeries (источник данных диаграммы) к диаграмме, охватывающей ячейки от "A1" до "B4"
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            // Установка источника данных для категориальных данных NSeries
            chart.NSeries.CategoryData = "C1:C4";
            Series series = chart.NSeries[seriesIndex];
            // Установка значений серии
            series.Values = "=B1:B4";

            // Установка типа 3D‑формы для серии
            series.Bar3DShapeType = Bar3DShapeType.Cylinder;

            // Сохранение файла Excel
            workbook.Save("Bar3DShapeTypeExample.xlsx");
            workbook.Save("Bar3DShapeTypeExample.pdf");

            // Установка типа 3D‑формы для серии
            series.Bar3DShapeType = Bar3DShapeType.ConeToMax;

            // Сохранение файла Excel
            workbook.Save("Bar3DShapeTypeExample2.xlsx");
            workbook.Save("Bar3DShapeTypeExample2.pdf");
            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


