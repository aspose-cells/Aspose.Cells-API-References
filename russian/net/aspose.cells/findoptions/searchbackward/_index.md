---
title: "FindOptions.SearchBackward"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FindOptions. Выполнять ли поиск назад по ячейкам"
type: docs
url: /ru/net/aspose.cells/findoptions/searchbackward/
---
## FindOptions.SearchBackward property

Искать ли в обратном направлении ячейки.

```csharp
public bool SearchBackward { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertySearchBackwardDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Настройте примерные данные
            worksheet.Cells["A1"].PutValue("abc");
            worksheet.Cells["B2"].PutValue("abc");
            worksheet.Cells["C3"].PutValue("abc");

            FindOptions options = new FindOptions();
            options.LookInType = LookInType.Values;
            options.LookAtType = LookAtType.Contains;
            
            // Поиск вперёд (поведение по умолчанию)
            options.SearchBackward = false;
            Cell foundForward = worksheet.Cells.Find("abc", null, options);
            Console.WriteLine($"Forward search found at: {foundForward.Name}");

            // Поиск назад
            options.SearchBackward = true;
            Cell foundBackward = worksheet.Cells.Find("abc", null, options);
            Console.WriteLine($"Backward search found at: {foundBackward.Name}");
        }
    }
}
```

### См. также

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


