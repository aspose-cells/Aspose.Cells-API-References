---
title: "PivotOptions.DropZoneFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotOptions. Указывает, отображается ли элемент управления для каждого поля PivotTable на оси страниц PivotTable исходной таблицы на диаграмме, когда параметр dropZonesVisible установлен в значение true"
type: docs
url: /ru/net/aspose.cells.charts/pivotoptions/dropzonefilter/
---
## PivotOptions.DropZoneFilter property

Указывает, отображается ли элемент управления для каждого поля сводной таблицы на оси страниц исходной сводной таблицы на диаграмме, когда параметр dropZonesVisible установлен в true.

```csharp
public bool DropZoneFilter { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PivotOptionsPropertyDropZoneFilterDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Пример данных
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

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("=A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Создать диаграмму, связанную с сводной таблицей
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.PivotSource = "PivotTable1";

            // Настроить параметры сводной таблицы с помощью DropZoneFilter
            PivotOptions pivotOptions = chart.PivotOptions;
            pivotOptions.DropZoneFilter = true;
            pivotOptions.DropZonesVisible = true;

            workbook.Save("PivotOptionsDropZoneFilterDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


