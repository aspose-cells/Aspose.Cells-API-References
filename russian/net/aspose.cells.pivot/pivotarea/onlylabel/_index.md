---
title: "PivotArea.OnlyLabel"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotArea. Указывает, выбраны ли только подписи данных для выбранного элемента"
type: docs
url: /ru/net/aspose.cells.pivot/pivotarea/onlylabel/
---
## PivotArea.OnlyLabel property

Указывает, выбираются ли только метки данных для выбранного элемента.

```csharp
public bool OnlyLabel { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyOnlyLabelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Пример данных
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавить поля
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Настроить область сводной таблицы
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.OnlyLabel = true; // Key property demonstration
            
            // Применить выделение
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.LabelOnly);

            workbook.Save("PivotAreaOnlyLabelDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


