---
title: "Cells.StandardHeightInch"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cells. Получает или задаёт высоту строки по умолчанию в этом листе в дюймах."
type: docs
url: /ru/net/aspose.cells/cells/standardheightinch/
---
## Cells.StandardHeightInch property

Получает или задает высоту строки по умолчанию в этом листе, в единицах дюймов.

```csharp
public double StandardHeightInch { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardHeightInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получите стандартную высоту в дюймах.
            double standardHeightInch = worksheet.Cells.StandardHeightInch;
            Console.WriteLine("Standard Height in Inches: " + standardHeightInch);
            
            // Установите новую стандартную высоту (1 дюйм).
            worksheet.Cells.StandardHeightInch = 1.0;
            Console.WriteLine("New Standard Height in Inches: " + worksheet.Cells.StandardHeightInch);
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


