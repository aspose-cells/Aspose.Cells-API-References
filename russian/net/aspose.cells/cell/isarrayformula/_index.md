---
title: "Cell.IsArrayFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Указывает, является ли формула ячейки массивной формулой."
type: docs
url: /ru/net/aspose.cells/cell/isarrayformula/
---
## Cell.IsArrayFormula property

Указывает, является ли формула ячейки массивной формулой.

```csharp
public bool IsArrayFormula { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsArrayFormulaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать массивную формулу в ячейке B2
            worksheet.Cells["B2"].SetArrayFormula("SUM(A1:A10*B1:B10)", 1, 1);
            
            // Проверить, содержит ли ячейка массивную формулу
            bool isArrayFormula = worksheet.Cells["B2"].IsArrayFormula;
            
            // Вывести результат.
            Console.WriteLine("Cell B2 is an array formula: " + isArrayFormula);
            
            // Сохраните книгу
            workbook.Save("IsArrayFormulaDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


