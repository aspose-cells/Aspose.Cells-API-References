---
title: "SlicerCollection.RemoveAt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SlicerCollection. Удаляет срез по указанному индексу"
type: docs
url: /ru/net/aspose.cells.slicers/slicercollection/removeat/
---
## SlicerCollection.RemoveAt method

Удаляет срез по указанному индексу

```csharp
public void RemoveAt(int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | Индекс позиции в коллекции срезов |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Добавить лист
            Worksheet worksheet = workbook.Worksheets.Add("Sheet1");
            
            // Добавьте некоторые данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["B4"].Value = 8;

            // Добавить сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Добавить срезы
            Aspose.Cells.Slicers.SlicerCollection slicers = worksheet.Slicers;
            slicers.Add(pivotTable, "Fruit", "FruitSlicer1");
            slicers.Add(pivotTable, "Fruit", "FruitSlicer2");

            // Удалить второй срез по индексу 1
            slicers.RemoveAt(1);
            
            // Сохраните книгу
            workbook.Save("SlicerCollectionMethodRemoveAtWithInt32Demo.xlsx");
        }
    }
}
```

### См. также

* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


