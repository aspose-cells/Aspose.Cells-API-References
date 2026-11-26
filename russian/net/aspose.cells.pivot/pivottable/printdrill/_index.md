---
title: "PivotTable.PrintDrill"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Указывает логическое значение, определяющее, должны ли выводиться индикаторы drill. Печать кнопок развертывания/сворачивания при отображении в сводной таблице"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/printdrill/
---
## PivotTable.PrintDrill property

Задаёт логическое значение, указывающее, следует ли печатать индикаторы drill. Печать кнопок раскрытия/сворачивания при отображении в pivottable.

```csharp
public bool PrintDrill { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPrintDrillDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            var cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Bikes";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Cars";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Bikes";
            cells["B4"].Value = 1500;
            cells["A5"].Value = "Cars";
            cells["B5"].Value = 2500;

            // Добавить сводную таблицу
            int index = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Настройте сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Продемонстрировать свойство PrintDrill
            pivotTable.PrintDrill = false; // Disable printing drill indicators
            pivotTable.ShowDrill = true;   // Show drill indicators on screen
            
            // Обновить и вычислить сводную таблицу
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Сохраните книгу
            workbook.Save("PivotTablePrintDrillDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


