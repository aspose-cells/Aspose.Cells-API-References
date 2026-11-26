---
title: "PivotItemCollection.ChangeitemsOrder"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotItemCollection. Непосредственно изменяет порядок двух элементов"
type: docs
url: /ru/net/aspose.cells.pivot/pivotitemcollection/changeitemsorder/
---
## PivotItemCollection.ChangeitemsOrder method

Непосредственно изменяет порядок двух элементов.

```csharp
[Obsolete("Use PivotItemCollection.SwapItem() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ChangeitemsOrder(int sourceIndex, int destIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceIndex | Int32 | Текущий индекс |
| destIndex | Int32 | Индекс назначения |

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод PivotItemCollection.SwapItem(). Этот метод будет удалён через 12 месяцев, начиная с июля 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemCollectionMethodChangeitemsOrderWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells[0, 0].Value = "Category";
            worksheet.Cells[1, 0].Value = "A";
            worksheet.Cells[2, 0].Value = "B";
            worksheet.Cells[3, 0].Value = "C";

            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:A4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = pivotField.PivotItems;

            Console.WriteLine("Original Order:");
            foreach (PivotItem item in pivotItems)
            {
                Console.WriteLine(item.Name);
            }

            pivotItems.ChangeitemsOrder(0, 2);

            Console.WriteLine("\nAfter Changing Order:");
            foreach (PivotItem item in pivotItems)
            {
                Console.WriteLine(item.Name);
            }

            workbook.Save("PivotItemOrderChange.xlsx");
        }
    }
}
```

### См. также

* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


