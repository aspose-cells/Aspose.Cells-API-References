---
title: "Перечисление CategoryType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Charts.CategoryType. Представляет тип оси категорий"
type: docs
url: /ru/net/aspose.cells.charts/categorytype/
---
## CategoryType enumeration

Представляет тип категориальной оси.

```csharp
public enum CategoryType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| AutomaticScale | `0` | AutomaticScale |
| CategoryScale | `1` | CategoryScale |
| TimeScale | `2` | TimeScale |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class CategoryTypeDemo
    {
        public static void CategoryTypeExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();
            // Добавление нового листа к объекту Excel
            int sheetIndex = workbook.Worksheets.Add();
            // Получение ссылки на только что добавленный лист путем передачи его индекса листа
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Добавление образцовых значений в ячейки
            worksheet.Cells["A1"].PutValue("Dates");
            worksheet.Cells["A2"].PutValue(new DateOnly(2024, 01, 01));
            worksheet.Cells["A3"].PutValue(new DateOnly(2024, 03, 01));
            worksheet.Cells["A4"].PutValue(new DateOnly(2024, 05, 01));
            worksheet.Cells["B1"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(50);
            worksheet.Cells["C1"].PutValue("Data2");
            worksheet.Cells["C2"].PutValue(8);
            worksheet.Cells["C3"].PutValue(15);
            worksheet.Cells["C4"].PutValue(30);

            // Добавление диаграммы в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            // Получение экземпляра недавно добавленной диаграммы
            Chart chart = worksheet.Charts[chartIndex];
            // Добавление NSeries (источника данных диаграммы) к диаграмме в диапазоне от ячейки "A1" до "B3"
            chart.NSeries.Add("B2:C4", true);

            // Установка имен категорий для оси X из диапазона "A2:A5"
            chart.NSeries[0].XValues = "A2:A4";

            // Установка типа оси категорий в TimeScale
            chart.CategoryAxis.CategoryType = CategoryType.CategoryScale;

            // Установка масштаба основной единицы для оси категорий
            chart.CategoryAxis.MajorUnitScale = TimeUnit.Months;
            chart.CategoryAxis.MajorUnit = 2;

            // Установка масштаба вспомогательной единицы для оси категорий
            chart.CategoryAxis.MinorUnitScale = TimeUnit.Months;
            chart.CategoryAxis.MinorUnit = 2;

            // Сохранение файла Excel
            workbook.Save("CategoryTypeExample.xlsx");
            workbook.Save("CategoryTypeExample.pdf");

        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


