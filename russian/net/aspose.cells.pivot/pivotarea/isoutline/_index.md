---
title: "PivotArea.IsOutline"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotArea. Указывает, относится ли правило к области, находящейся в режиме контура"
type: docs
url: /ru/net/aspose.cells.pivot/pivotarea/isoutline/
---
## PivotArea.IsOutline property

Указывает, относится ли правило к области, находящейся в режиме структуры.

```csharp
public bool IsOutline { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyIsOutlineDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавить поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales

            // Создать и настроить PivotArea
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.IsOutline = false; // Disable outline style
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.DataAndLabel);

            // Сохраните книгу
            workbook.Save("PivotAreaIsOutlineDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


