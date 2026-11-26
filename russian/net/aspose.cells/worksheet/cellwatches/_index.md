---
title: "Worksheet.CellWatches"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Получает коллекцию ячеек этого листа, наблюдаемых в окне наблюдения"
type: docs
url: /ru/net/aspose.cells/worksheet/cellwatches/
---
## Worksheet.CellWatches property

Получает коллекцию ячеек этого листа, наблюдаемых в окне 'watch window'.

```csharp
public CellWatchCollection CellWatches { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCellWatchesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные в ячейку B2
            sheet.Cells["B2"].PutValue("Sample Data");

            // Добавить Cell Watch для B2
            int watchIndex = sheet.CellWatches.Add("B2");
            CellWatch cellWatch = sheet.CellWatches[watchIndex];

            // Отобразить информацию о наблюдении
            Console.WriteLine($"Cell Watch Added - Index: {watchIndex}");
            Console.WriteLine($"Cell Name: {cellWatch.CellName}");
            Console.WriteLine($"Row: {cellWatch.Row}, Column: {cellWatch.Column}");

            // Сохраните книгу
            workbook.Save("CellWatchDemo.xlsx");
        }
    }
}
```

### См. также

* class [CellWatchCollection](../../cellwatchcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


