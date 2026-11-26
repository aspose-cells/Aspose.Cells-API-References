---
title: "Worksheet.HasAutofilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Указывает, имеет ли лист автофильтр"
type: docs
url: /ru/net/aspose.cells/worksheet/hasautofilter/
---
## Worksheet.HasAutofilter property

Указывает, имеет ли этот лист автофильтр.

```csharp
public bool HasAutofilter { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyHasAutofilterDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            
            // Установить автофильтр
            worksheet.AutoFilter.Range = "A1:B3";
            
            // Проверьте, имеет ли лист автофильтр
            Console.WriteLine("Worksheet has autofilter: " + worksheet.HasAutofilter);
            
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


