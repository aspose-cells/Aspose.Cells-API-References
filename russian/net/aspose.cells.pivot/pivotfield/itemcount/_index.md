---
title: "PivotField.ItemCount"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotField. Возвращает количество базовых элементов в этом сводном поле"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/itemcount/
---
## PivotField.ItemCount property

Возвращает количество базовых элементов в этом сводном поле.

```csharp
[Obsolete("Use PivotField.PivotItems.Count instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int ItemCount { get; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте свойство PivotField.PivotItems.Count. Этот метод будет удалён через 12 месяцев, начиная с августа 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyItemCountDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Fruit");
            worksheet.Cells["A4"].PutValue("Vegetable");
            worksheet.Cells["A5"].PutValue("Vegetable");
            worksheet.Cells["A6"].PutValue("Fruit");
            worksheet.Cells["A7"].PutValue("Vegetable");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(200);
            worksheet.Cells["B5"].PutValue(120);
            worksheet.Cells["B6"].PutValue(180);
            worksheet.Cells["B7"].PutValue(90);

            // Добавьте сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B7", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Вычислить данные
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Получите сводное поле и отобразите количество его элементов
            PivotField pivotField = pivotTable.RowFields[0];
            Console.WriteLine("Item count in pivot field: " + pivotField.ItemCount);
            
            // Сохраните книгу
            workbook.Save("PivotFieldItemCountDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


