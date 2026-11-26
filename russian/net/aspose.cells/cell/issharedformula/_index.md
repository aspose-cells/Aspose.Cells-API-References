---
title: "Cell.IsSharedFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Указывает, является ли формула ячейки частью общей формулы"
type: docs
url: /ru/net/aspose.cells/cell/issharedformula/
---
## Cell.IsSharedFormula property

Указывает, является ли формула ячейки частью общей формулы.

```csharp
public bool IsSharedFormula { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsSharedFormulaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить общую формулу в диапазоне
            worksheet.Cells["B2"].Formula = "=A2*2";
            worksheet.Cells["B2"].Copy(worksheet.Cells["B3:B5"]);

            // Проверить, содержат ли ячейки общую формулу
            Cell cellB2 = worksheet.Cells["B2"];
            Cell cellB3 = worksheet.Cells["B3"];

            Console.WriteLine("Cell B2 IsSharedFormula: " + cellB2.IsSharedFormula);
            Console.WriteLine("Cell B3 IsSharedFormula: " + cellB3.IsSharedFormula);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


