---
title: "Cell.IntValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Получает целочисленное значение, содержащееся в ячейке"
type: docs
url: /ru/net/aspose.cells/cell/intvalue/
---
## Cell.IntValue property

Получает целочисленное значение, содержащееся в ячейке.

```csharp
public int IntValue { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIntValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Установите числовое значение и получите IntValue
            Cell cell1 = cells[0, 0];
            cell1.PutValue(42);
            Console.WriteLine("IntValue of numeric cell: " + cell1.IntValue);

            // Установите формулу, вычисляющую число, и получите IntValue
            Cell cell2 = cells[0, 1];
            cell2.Formula = "=10+5";
            workbook.CalculateFormula();
            Console.WriteLine("IntValue of formula cell: " + cell2.IntValue);

            // Установите логическое значение и получите IntValue
            Cell cell3 = cells[0, 2];
            cell3.PutValue(true);
            Console.WriteLine("IntValue of boolean cell: " + cell3.IntValue);

            // Установите текстовое значение и получите IntValue (будет 0, если не преобразуемо)
            Cell cell4 = cells[0, 3];
            cell4.PutValue("Hello");
            Console.WriteLine("IntValue of text cell: " + cell4.IntValue);
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


