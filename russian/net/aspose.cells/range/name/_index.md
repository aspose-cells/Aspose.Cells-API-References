---
title: "Range.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Range. Получает или задает имя диапазона"
type: docs
url: /ru/net/aspose.cells/range/name/
---
## Range.Name property

Получает или задает имя диапазона.

```csharp
public string Name { get; set; }
```

### Примечания

Именованные диапазоны поддерживаются. Например,

range.Name = "Sheet1!MyRange";

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте диапазон (колонки от A до B)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 2, true);
            
            // Установите свойство имени для диапазона
            range.Name = "testRange";
            
            // Проверьте, что имя было установлено
            Console.WriteLine("Range name: " + range.Name);
            
            // Сохраните книгу
            workbook.Save("RangeWithName.xlsx");
            
            // Откройте сохранённый файл, чтобы продемонстрировать, что имя сохраняется
            Workbook loadedWorkbook = new Workbook("RangeWithName.xlsx");
            Aspose.Cells.Range loadedRange = loadedWorkbook.Worksheets[0].Cells.CreateRange(0, 2, true);
            Console.WriteLine("Loaded range name: " + loadedRange.Name);
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


