---
title: "Worksheet.RemoveAutoFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Worksheet. Удаляет автофильтр листа"
type: docs
url: /ru/net/aspose.cells/worksheet/removeautofilter/
---
## Worksheet.RemoveAutoFilter method

Удаляет автофильтр листа.

```csharp
public void RemoveAutoFilter()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodRemoveAutoFilterDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            
            // Применить автофильтр
            worksheet.AutoFilter.Range = "A1:A3";
            
            Console.WriteLine("AutoFilter applied: " + worksheet.HasAutofilter);
            
            // Удалить автофильтр
            worksheet.RemoveAutoFilter();
            
            Console.WriteLine("AutoFilter after removal: " + worksheet.HasAutofilter);
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


