---
title: "Cell.BoolValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Возвращает логическое значение, содержащееся в ячейке"
type: docs
url: /ru/net/aspose.cells/cell/boolvalue/
---
## Cell.BoolValue property

Получает логическое значение, содержащееся в ячейке.

```csharp
public bool BoolValue { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyBoolValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Cell cell = cells[0, 0];
            
            // Установить формулу, которая вычисляется в логическое значение
            cell.Formula = "=2.01>2";
            
            // Вычислить формулу, чтобы получить результат
            workbook.CalculateFormula();
            
            // Продемонстрировать свойство BoolValue
            Console.WriteLine("Cell BoolValue: " + cell.BoolValue);
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


