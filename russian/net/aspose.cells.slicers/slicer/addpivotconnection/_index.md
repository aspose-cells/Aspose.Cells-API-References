---
title: "Slicer.AddPivotConnection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Slicer. Добавляет соединение с PivotTable"
type: docs
url: /ru/net/aspose.cells.slicers/slicer/addpivotconnection/
---
## Slicer.AddPivotConnection method

Добавляет соединение PivotTable.

```csharp
public void AddPivotConnection(PivotTable pivot)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| свод | PivotTable | Объект PivotTable |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerMethodAddPivotConnectionWithPivotTableDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B2"].Value = 10;
            cells["B3"].Value = 15;
            cells["B4"].Value = 5;

            // Создать сводную таблицу
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Добавить срез — исправленные параметры
            int slicerIndex = sheet.Slicers.Add(pivotTable, 0, 0, "Slicer1");
            Slicer slicer = sheet.Slicers[slicerIndex];

            // Добавить соединение сводной таблицы к срезу
            slicer.AddPivotConnection(pivotTable);

            // Сохраните книгу
            workbook.Save("SlicerAddPivotConnectionDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


