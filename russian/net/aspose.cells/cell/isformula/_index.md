---
title: "Cell.IsFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Указывает, содержит ли указанная ячейка формулу"
type: docs
url: /ru/net/aspose.cells/cell/isformula/
---
## Cell.IsFormula property

Представляет, содержит ли указанная ячейка формулу.

```csharp
public bool IsFormula { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsFormulaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить формулу в ячейку A1
            worksheet.Cells["A1"].Formula = "=1+2";
            
            // Добавить простое значение в ячейку A2
            worksheet.Cells["A2"].PutValue("Test");
            
            // Проверить, содержат ли ячейки формулы
            Console.WriteLine("A1 is formula: " + worksheet.Cells["A1"].IsFormula);
            Console.WriteLine("A2 is formula: " + worksheet.Cells["A2"].IsFormula);
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


