---
title: "Класс PivotOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Charts.PivotOptions. Представляет сложный тип, который определяет элементы управления сводкой, отображаемые на диаграмме"
type: docs
url: /ru/net/aspose.cells.charts/pivotoptions/
---
## PivotOptions class

Представляет сложный тип, определяющий элементы управления сводной таблицы, отображаемые на диаграмме

```csharp
public class PivotOptions
```

## Свойства

| Имя | Описание |
| --- | --- |
| [DropZoneCategories](../../aspose.cells.charts/pivotoptions/dropzonecategories/) { get; set; } | Указывает, отображается ли элемент управления для каждого поля сводной таблицы на оси строк исходной сводной таблицы на диаграмме, когда параметр dropZonesVisible установлен в true. |
| [DropZoneData](../../aspose.cells.charts/pivotoptions/dropzonedata/) { get; set; } | Указывает, отображается ли элемент управления для каждого поля сводной таблицы на оси данных исходной сводной таблицы на диаграмме, когда параметр dropZonesVisible установлен в true. |
| [DropZoneFilter](../../aspose.cells.charts/pivotoptions/dropzonefilter/) { get; set; } | Указывает, отображается ли элемент управления для каждого поля сводной таблицы на оси страниц исходной сводной таблицы на диаграмме, когда параметр dropZonesVisible установлен в true. |
| [DropZoneSeries](../../aspose.cells.charts/pivotoptions/dropzoneseries/) { get; set; } | Указывает, отображается ли элемент управления для каждого поля сводной таблицы на оси столбцов исходной сводной таблицы на диаграмме, когда параметр dropZonesVisible установлен в true. |
| [DropZonesVisible](../../aspose.cells.charts/pivotoptions/dropzonesvisible/) { get; set; } | Указывает, могут ли какие-либо элементы управления сводкой появляться на сводной диаграмме. |
| [ShowExpandCollapseFieldButtons](../../aspose.cells.charts/pivotoptions/showexpandcollapsefieldbuttons/) { get; set; } | Получает или задает значение, указывающее, показывать ли кнопки раскрытия или сворачивания полей |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotOptionsDemo
    {
        public static void PivotOptionsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B5"].PutValue(40);

            // Добавить сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("=A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.PivotSource = "PivotTable1";

            // Получите доступ к PivotOptions диаграммы
            PivotOptions pivotOptions = chart.PivotOptions;

            // Установите свойства PivotOptions
            pivotOptions.DropZoneFilter = true;
            pivotOptions.DropZoneCategories = true;
            pivotOptions.DropZoneData = true;
            pivotOptions.DropZoneSeries = true;
            pivotOptions.DropZonesVisible = true;

            // Сохраните книгу
            workbook.Save("PivotOptionsExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


