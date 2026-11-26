---
title: "CellWatch.CellName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "CellWatch свойство. Получает и задает имя ячейки"
type: docs
url: /ru/net/aspose.cells/cellwatch/cellname/
---
## CellWatch.CellName property

Получает и задает имя ячейки.

```csharp
public string CellName { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellWatchPropertyCellNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте несколько наблюдений за ячейками
            worksheet.CellWatches.Add("B5");
            worksheet.CellWatches.Add("C10");
            
            // Отобразите имена ячеек всех наблюдателей
            Console.WriteLine("Cell Watches:");
            foreach (CellWatch watch in worksheet.CellWatches)
            {
                Console.WriteLine(watch.CellName);
            }
            
            // Добавьте новое наблюдение и отобразите его имя
            worksheet.CellWatches.Add("A1");
            Console.WriteLine("Added new watch: " + 
                worksheet.CellWatches[worksheet.CellWatches.Count - 1].CellName);
            
            // Сохраните книгу
            workbook.Save("CellWatchDemo.xlsx");
        }
    }
}
```

### См. также

* class [CellWatch](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


