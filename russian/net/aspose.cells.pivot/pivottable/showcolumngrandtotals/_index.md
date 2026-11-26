---
title: "PivotTable.ShowColumnGrandTotals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Указывает, следует ли показывать общие итоги для столбцов этой сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/showcolumngrandtotals/
---
## PivotTable.ShowColumnGrandTotals property

Указывает, следует ли показывать общие итоги для столбцов этой сводной таблицы.

```csharp
public bool ShowColumnGrandTotals { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowColumnGrandTotalsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            var cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["A5"].Value = "Apple";
            cells["B2"].Value = 5;
            cells["B3"].Value = 3;
            cells["B4"].Value = 6;
            cells["B5"].Value = 2;

            // Добавьте сводную таблицу
            int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Настройте сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit as rows
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sum of Quantity

            // Продемонстрировать свойство ShowColumnGrandTotals
            pivotTable.ShowColumnGrandTotals = false; // Disable column grand totals
            Console.WriteLine("Column Grand Totals Visible: " + pivotTable.ShowColumnGrandTotals);

            // Сохраните книгу
            workbook.Save("PivotTableShowColumnGrandTotalsDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


