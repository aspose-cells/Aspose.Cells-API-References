---
title: "PivotTable.ShowRowGrandTotals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Указывает, показывать ли общие итоги для строк сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/showrowgrandtotals/
---
## PivotTable.ShowRowGrandTotals property

Указывает, показывать ли общие итоги для строк сводной таблицы.

```csharp
public bool ShowRowGrandTotals { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowRowGrandTotalsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить лист
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Product A";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            
            cells["A3"].Value = "Product B";
            cells["B3"].Value = "South";
            cells["C3"].Value = 1500;
            
            cells["A4"].Value = "Product A";
            cells["B4"].Value = "South";
            cells["C4"].Value = 2000;
            
            cells["A5"].Value = "Product B";
            cells["B5"].Value = "North";
            cells["C5"].Value = 1200;

            // Добавить сводную таблицу
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Настройте сводную таблицу
            pivotTable.ShowRowGrandTotals = true; // Demonstrate ShowRowGrandTotals property
            pivotTable.ShowColumnGrandTotals = true;
            
            // Добавить поля в области
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product as row
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Region as column
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales as data
            
            // Сохраните книгу
            workbook.Save("PivotTableShowRowGrandTotalsDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


