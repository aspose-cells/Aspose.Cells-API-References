---
title: "Protection.AllowUsingPivotTable"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Protection. Представляет, разрешено ли пользователю манипулировать сводными таблицами на защищённом листе"
type: docs
url: /ru/net/aspose.cells/protection/allowusingpivottable/
---
## Protection.AllowUsingPivotTable property

Представляет, разрешено ли пользователю манипулировать сводными таблицами на защищённом листе.

```csharp
public bool AllowUsingPivotTable { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowUsingPivotTableDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Включить защиту листа
            Protection protection = worksheet.Protection;
            protection.AllowUsingPivotTable = true;
            worksheet.Protect(ProtectionType.All);

            // Проверьте настройку
            Console.WriteLine("AllowUsingPivotTable is set to: " + protection.AllowUsingPivotTable);

            // Создайте сводную таблицу, чтобы продемонстрировать функциональность
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);

            // Создайте сводную таблицу с правильными параметрами
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "C1", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Сохраните книгу
            workbook.Save("ProtectionPropertyAllowUsingPivotTableDemo.xlsx");
        }
    }
}
```

### См. также

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


