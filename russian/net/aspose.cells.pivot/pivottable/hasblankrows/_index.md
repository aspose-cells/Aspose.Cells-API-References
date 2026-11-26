---
title: "PivotTable.HasBlankRows"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Указывает, следует ли добавлять пустые строки. Это свойство применяется только к типам автоформатирования PivotTable, которым необходимо добавлять пустые строки."
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/hasblankrows/
---
## PivotTable.HasBlankRows property

Указывает, следует ли добавлять пустые строки. Это свойство применяется только к типам автоформатирования PivotTable, которым необходимо добавлять пустые строки.

```csharp
[Obsolete("Use PivotField.InsertBlankRow property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool HasBlankRows { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство PivotField.InsertBlankRow. Этот метод будет удалён через 12 месяцев, начиная с апреля 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyHasBlankRowsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet dataSheet = wb.Worksheets[0];
            
            // Создать примерные данные
            dataSheet.Cells[0, 0].PutValue("Category");
            dataSheet.Cells[0, 1].PutValue("Product");
            dataSheet.Cells[0, 2].PutValue("Sales");
            
            Random rnd = new Random();
            for (int i = 1; i <= 10; i++)
            {
                dataSheet.Cells[i, 0].PutValue(rnd.Next(2) == 0 ? "Electronics" : "Furniture");
                dataSheet.Cells[i, 1].PutValue("Product " + rnd.Next(1, 4));
                dataSheet.Cells[i, 2].PutValue(rnd.Next(100, 1000));
            }

            // Добавьте сводную таблицу
            Worksheet pivotSheet = wb.Worksheets.Add("PivotTable");
            int pivotIndex = pivotSheet.PivotTables.Add(
                "=Sheet1!A1:C11", "A1", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];

            // Настройте сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Row, 1); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales
            
            // Продемонстрировать свойство HasBlankRows
            pivotTable.HasBlankRows = false; // Remove blank lines between items
            
            // Сохраните книгу
            wb.Save("PivotTableHasBlankRowsDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


