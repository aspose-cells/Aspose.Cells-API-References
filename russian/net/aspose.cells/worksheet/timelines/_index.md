---
title: "Worksheet.Timelines"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Получает коллекцию Timeline на листе"
type: docs
url: /ru/net/aspose.cells/worksheet/timelines/
---
## Worksheet.Timelines property

Получить коллекцию Timeline в листе

```csharp
public TimelineCollection Timelines { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTimelinesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            sheet.Cells["A1"].Value = "Ship Date";
            sheet.Cells["A2"].Value = new DateTime(2023, 1, 1);
            sheet.Cells["A3"].Value = new DateTime(2023, 1, 15);
            sheet.Cells["A4"].Value = new DateTime(2023, 2, 1);
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 1000;
            sheet.Cells["B3"].Value = 2000;
            sheet.Cells["B4"].Value = 3000;

            // Создать сводную таблицу
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Ship Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Добавить элемент управления Timeline для сводной таблицы
            sheet.Timelines.Add(pivotTable, 0, 0, "Ship Date");

            // Сохраните книгу
            workbook.Save("TimelineDemo.xlsx");
        }
    }
}
```

### См. также

* class [TimelineCollection](../../../aspose.cells.timelines/timelinecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


