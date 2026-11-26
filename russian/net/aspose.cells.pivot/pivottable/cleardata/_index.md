---
title: "PivotTable.ClearData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotTable. Очистить данные и форматирование представления PivotTable"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/cleardata/
---
## PivotTable.ClearData method

Очистить данные и форматирование представления PivotTable.

```csharp
public void ClearData()
```

### Примечания

Если этот метод не вызвать перед добавлением или удалением PivotField, возможно, данные PivotTable не будут корректными

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodClearDataDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Fruit");
            worksheet.Cells["A4"].PutValue("Vegetable");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(15);

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавить поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            Console.WriteLine("Pivot table with data:");
            Console.WriteLine(worksheet.Cells["D1"].StringValue);
            Console.WriteLine(worksheet.Cells["D2"].StringValue);
            Console.WriteLine(worksheet.Cells["D3"].StringValue);

            // Очистить данные сводной таблицы
            pivotTable.ClearData();
            Console.WriteLine("\nAfter ClearData():");
            Console.WriteLine("Pivot table row count: " + (pivotTable.DataBodyRange.EndRow - pivotTable.DataBodyRange.StartRow + 1));

            // Перестроить сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            Console.WriteLine("\nRebuilt pivot table:");
            Console.WriteLine(worksheet.Cells["D1"].StringValue);
            Console.WriteLine(worksheet.Cells["D2"].StringValue);
            Console.WriteLine(worksheet.Cells["D3"].StringValue);

            // Сохранить книгу
            workbook.Save("PivotTableClearDataDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


