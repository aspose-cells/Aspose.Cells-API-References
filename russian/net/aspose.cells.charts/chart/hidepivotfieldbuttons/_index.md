---
title: "Chart.HidePivotFieldButtons"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Указывает, скрывать ли кнопки полей сводной диаграммы только когда диаграмма является PivotChart"
type: docs
url: /ru/net/aspose.cells.charts/chart/hidepivotfieldbuttons/
---
## Chart.HidePivotFieldButtons property

Указывает, скрывать ли кнопки полей сводной диаграммы только когда диаграмма является PivotChart.

```csharp
public bool HidePivotFieldButtons { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class ChartPropertyHidePivotFieldButtonsDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["B4"].Value = 200;

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Создать диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column3DClustered, 9, 6, 24, 14);
            Chart chart = worksheet.Charts[chartIndex];
            chart.PivotSource = "Sheet1!PivotTable1";
            
            // Продемонстрировать свойство HidePivotFieldButtons
            chart.HidePivotFieldButtons = false; // Show pivot field buttons
            chart.RefreshPivotData();

            // Сохраните книгу
            workbook.Save("HidePivotFieldButtonsDemo.xlsx");
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


