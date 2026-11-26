---
title: "Cell.Formula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Получает или задает формулу ячейки"
type: docs
url: /ru/net/aspose.cells/cell/formula/
---
## Cell.Formula property

Получает или задает формулу [`Cell`](../).

```csharp
public string Formula { get; set; }
```

### Примечания

Строка формулы всегда начинается со знака равенства (=). И, пожалуйста, всегда используйте запятую (,) в качестве разделителя параметров, например "=SUM(A1, E1, H2)".

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyFormulaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите значения в ячейках, которые будут использоваться в формуле
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);
            worksheet.Cells["E1"].PutValue(5);
            worksheet.Cells["A1"].PutValue(100);

            // Установите формулу в ячейку B6
            worksheet.Cells["B6"].Formula = "=SUM(B2:B5, E1) + A1";

            // Вычислить формулу
            workbook.CalculateFormula();

            // Отобразить результат
            Console.WriteLine("Formula result in B6: " + worksheet.Cells["B6"].Value);
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


