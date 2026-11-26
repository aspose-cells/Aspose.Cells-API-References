---
title: "Range.Worksheet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Range. Получает объект Worksheetobject, который содержит этот диапазон"
type: docs
url: /ru/net/aspose.cells/range/worksheet/
---
## Range.Worksheet property

Получает объект `Worksheet`, который содержит этот диапазон.

```csharp
public Worksheet Worksheet { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyWorksheetDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать именованный диапазон
            worksheet.Cells["A1"].PutValue("Test");
            worksheet.Cells["B1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            
            // Определите именованный диапазон
            int index = workbook.Worksheets.Names.Add("MyRange");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!$A$1:$B$2";
            
            // Получите диапазон по имени (полностью квалифицируйте Range, чтобы избежать неоднозначности)
            Aspose.Cells.Range range = workbook.Worksheets.GetRangeByName("MyRange");
            
            // Продемонстрировать использование свойства Worksheet
            Console.WriteLine("Range belongs to worksheet: " + range.Worksheet.Name);
            
            // Использовать свойство Worksheet для изменения ячеек
            range.Worksheet.Cells["A1"].PutValue("Updated");
            
            // Сохраните книгу
            workbook.Save("RangePropertyWorksheetDemo.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../../worksheet/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


