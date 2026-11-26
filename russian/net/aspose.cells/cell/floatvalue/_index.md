---
title: "Cell.FloatValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Возвращает числовое значение с плавающей точкой, содержащееся в ячейке"
type: docs
url: /ru/net/aspose.cells/cell/floatvalue/
---
## Cell.FloatValue property

Получает значение float, содержащееся в ячейке.

```csharp
public float FloatValue { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyFloatValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите числовое значение напрямую
            worksheet.Cells["A1"].PutValue(3.14f);
            Console.WriteLine("FloatValue of A1: " + worksheet.Cells["A1"].FloatValue);
            
            // Установите формулу, возвращающую число с плавающей точкой
            worksheet.Cells["A2"].Formula = "=3.5*2";
            workbook.CalculateFormula();
            Console.WriteLine("FloatValue of A2: " + worksheet.Cells["A2"].FloatValue);
            
            // Продемонстрируйте FloatValue с общей формулой
            worksheet.Cells["B1"].Formula = "=5-2";
            workbook.CalculateFormula();
            worksheet.Cells["B1"].SetSharedFormula("=5-2", 3, 1);
            workbook.CalculateFormula();
            Console.WriteLine("FloatValue of B3: " + worksheet.Cells["B3"].FloatValue);
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


