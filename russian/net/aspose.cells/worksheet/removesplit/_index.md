---
title: "Worksheet.RemoveSplit"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Worksheet. Удаляет разделённое окно"
type: docs
url: /ru/net/aspose.cells/worksheet/removesplit/
---
## Worksheet.RemoveSplit method

Удаляет разделённое окно.

```csharp
public void RemoveSplit()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodRemoveSplitDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Разделить лист
            worksheet.Split();
            Console.WriteLine("Worksheet split state: " + worksheet.PaneState);
            
            // Удалить разделение
            worksheet.RemoveSplit();
            Console.WriteLine("Worksheet split state after RemoveSplit: " + worksheet.PaneState);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


