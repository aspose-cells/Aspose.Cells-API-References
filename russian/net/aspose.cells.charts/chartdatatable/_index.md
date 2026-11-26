---
title: "Класс ChartDataTable"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Charts.ChartDataTable. Представляет таблицу данных диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chartdatatable/
---
## ChartDataTable class

Представляет таблицу данных диаграммы.

```csharp
public class ChartDataTable
```

## Свойства

| Имя | Описание |
| --- | --- |
| [AutoScaleFont](../../aspose.cells.charts/chartdatatable/autoscalefont/) { get; set; } | True, если текст в объекте изменяет размер шрифта при изменении размера объекта. Значение по умолчанию — True. |
| [BackgroundMode](../../aspose.cells.charts/chartdatatable/backgroundmode/) { get; set; } | Получает и задает режим отображения фона |
| [Border](../../aspose.cells.charts/chartdatatable/border/) { get; } | Возвращает объект Border, который представляет границу объекта |
| [Font](../../aspose.cells.charts/chartdatatable/font/) { get; } | Получает объект [`Font`](./font/), который представляет настройки шрифта указанной таблицы данных диаграммы. |
| [HasBorderHorizontal](../../aspose.cells.charts/chartdatatable/hasborderhorizontal/) { get; set; } | (**Устарело.**) Истина, если у таблицы данных диаграммы есть горизонтальные границы ячеек |
| [HasBorderOutline](../../aspose.cells.charts/chartdatatable/hasborderoutline/) { get; set; } | (**Obsolete.**) Истина, если у таблицы данных диаграммы есть границы контура |
| [HasBorderVertical](../../aspose.cells.charts/chartdatatable/hasbordervertical/) { get; set; } | (**Obsolete.**) Истина, если у таблицы данных диаграммы есть вертикальные границы ячеек |
| [HasHorizontalBorder](../../aspose.cells.charts/chartdatatable/hashorizontalborder/) { get; set; } | Истина, если у таблицы данных диаграммы есть горизонтальные границы ячеек |
| [HasOutlineBorder](../../aspose.cells.charts/chartdatatable/hasoutlineborder/) { get; set; } | Истина, если у таблицы данных диаграммы есть границы контура |
| [HasVerticalBorder](../../aspose.cells.charts/chartdatatable/hasverticalborder/) { get; set; } | Истина, если у таблицы данных диаграммы есть вертикальные границы ячеек |
| [ShowLegendKey](../../aspose.cells.charts/chartdatatable/showlegendkey/) { get; set; } | Истина, если ключ легенды подписи данных виден. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartDataTableDemo
    {
        public static void ChartDataTableExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();

            // Получение ссылки на первый лист
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавление образцовых значений в ячейки
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Добавление диаграммы в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);

            // Получение экземпляра недавно добавленной диаграммы
            Chart chart = worksheet.Charts[chartIndex];

            // Добавление NSeries (источника данных диаграммы) к диаграмме в диапазоне от ячейки "A1" до "B3"
            chart.NSeries.Add("A1:B3", true);

            // Отображение таблицы данных
            chart.ShowDataTable = true;

            // Получение таблицы данных диаграммы
            ChartDataTable chartTable = chart.ChartDataTable;

            // Установка свойств таблицы данных диаграммы
            chartTable.Font.Color = Color.Red;
            chartTable.AutoScaleFont = true;
            chartTable.BackgroundMode = BackgroundMode.Transparent;
            chartTable.HasBorderHorizontal = true;
            chartTable.HasBorderVertical = true;
            chartTable.HasBorderOutline = true;
            chartTable.ShowLegendKey = false;

            // Сохранение файла Excel
            workbook.Save("ChartDataTableExample.xlsx");
            workbook.Save("ChartDataTableExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


