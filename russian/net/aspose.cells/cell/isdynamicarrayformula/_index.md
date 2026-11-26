---
title: "Cell.IsDynamicArrayFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Указывает, является ли формула ячейки динамической массивной формулой (true) или устаревшей массивной формулой (false)"
type: docs
url: /ru/net/aspose.cells/cell/isdynamicarrayformula/
---
## Cell.IsDynamicArrayFormula property

Указывает, является ли формула ячейки динамической массивной формулой (true) или устаревшей массивной формулой (false).

```csharp
public bool IsDynamicArrayFormula { get; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsDynamicArrayFormulaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установите динамическую массивную формулу в ячейку A1
            worksheet.Cells["A1"].SetDynamicArrayFormula("=B1:B3", new FormulaParseOptions(), false);
            
            // Проверьте, содержит ли ячейка динамическую массивную формулу
            Console.WriteLine("Is A1 a dynamic array formula? " + worksheet.Cells["A1"].IsDynamicArrayFormula);

            // Сохраните книгу
            string outputPath = "DynamicArrayFormulaDemo.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);

            Console.WriteLine("Workbook saved with dynamic array formula at: " + outputPath);
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


