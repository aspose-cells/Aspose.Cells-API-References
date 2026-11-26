---
title: "PivotOptions.DropZoneData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotOptions. Указывает, отображается ли элемент управления для каждого поля PivotTable на оси данных PivotTable исходной таблицы на диаграмме, когда параметр dropZonesVisible установлен в значение true"
type: docs
url: /ru/net/aspose.cells.charts/pivotoptions/dropzonedata/
---
## PivotOptions.DropZoneData property

Указывает, отображается ли элемент управления для каждого поля сводной таблицы на оси данных исходной сводной таблицы на диаграмме, когда параметр dropZonesVisible установлен в true.

```csharp
public bool DropZoneData { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PivotOptionsPropertyDropZoneDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Пример данных для сводной таблицы
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Books");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Electronics");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Books");
            worksheet.Cells["B4"].PutValue(1500);

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "SalesPivot");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Создать диаграмму, связанную со сводной таблицей
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.PivotSource = "SalesPivot";

            // Настроить параметры сводной таблицы с включённым DropZoneData
            PivotOptions pivotOptions = chart.PivotOptions;
            pivotOptions.DropZoneData = true;
            pivotOptions.DropZonesVisible = true;

            // Сохранить результат
            workbook.Save("PivotOptionsDropZoneDataDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


