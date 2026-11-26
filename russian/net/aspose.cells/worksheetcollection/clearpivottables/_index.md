---
title: "WorksheetCollection.ClearPivottables"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод WorksheetCollection. Очищает сводные таблицы из электронной таблицы"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/clearpivottables/
---
## WorksheetCollection.ClearPivottables method

Удаляет сводные таблицы из электронной таблицы.

```csharp
public void ClearPivottables()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodClearPivottablesDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать примерные данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // Добавить сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            Console.WriteLine("Pivot tables count before clearing: " + worksheet.PivotTables.Count);

            // Очистить все сводные таблицы во всех листах
            workbook.Worksheets.ClearPivottables();

            Console.WriteLine("Pivot tables count after clearing: " + worksheet.PivotTables.Count);
        }
    }
}
```

### См. также

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


