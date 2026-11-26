---
title: "Cell.IsArrayHeader"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Указывает, что формула ячейки является формулой массива и что это первая ячейка массива"
type: docs
url: /ru/net/aspose.cells/cell/isarrayheader/
---
## Cell.IsArrayHeader property

Указывает, что формула ячейки является массивной формулой и эта ячейка является первой ячейкой массива.

```csharp
public bool IsArrayHeader { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsArrayHeaderDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте формулу массива в диапазоне B2:D4
            worksheet.Cells["B2"].SetArrayFormula("=A1:A3*B1:B3", 3, 3);
            
            // Проверьте и выведите свойство IsArrayHeader
            // Примечание: IsArrayHeader только для чтения и автоматически устанавливается для заголовков формул массива
            Console.WriteLine("B2 IsArrayHeader: " + worksheet.Cells["B2"].IsArrayHeader);
            Console.WriteLine("B3 IsArrayHeader: " + worksheet.Cells["B3"].IsArrayHeader);
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


