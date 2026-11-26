---
title: "PivotFieldCollection.Move"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotFieldCollection. Перемещает PivotField из текущей позиции в целевую позицию"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfieldcollection/move/
---
## PivotFieldCollection.Move method

Перемещает PivotField из текущей позиции в целевую позицию

```csharp
public void Move(int currPos, int destPos)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| currPos | Int32 | Текущая позиция PivotField, начиная с нуля |
| destPos | Int32 | Позиция назначения PivotField, основанная на нуле |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldCollectionMethodMoveWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Создать примерные данные
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B1"].Value = "Quantity";
            cells["B2"].Value = 10;
            cells["B3"].Value = 15;
            cells["B4"].Value = 20;

            // Создать сводную таблицу
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Добавить поля в область строк
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Row, 1);
            
            Console.WriteLine("Before move:");
            for (int i = 0; i < pivotTable.RowFields.Count; i++)
            {
                Console.WriteLine($"Field {i}: {pivotTable.RowFields[i].Name}");
            }
            
            // Переместить первое поле в позицию 1
            pivotTable.RowFields.Move(0, 1);
            
            Console.WriteLine("\nAfter move:");
            for (int i = 0; i < pivotTable.RowFields.Count; i++)
            {
                Console.WriteLine($"Field {i}: {pivotTable.RowFields[i].Name}");
            }
        }
    }
}
```

### См. также

* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


