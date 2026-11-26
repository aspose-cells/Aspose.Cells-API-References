---
title: "Cell.GetWidthOfValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Получает ширину значения в пикселях"
type: docs
url: /ru/net/aspose.cells/cell/getwidthofvalue/
---
## Cell.GetWidthOfValue method

Получает ширину значения в пикселях.

```csharp
public int GetWidthOfValue()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetWidthOfValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            cell.PutValue("CellsJava40307");
            int width = cell.GetWidthOfValue();
            
            Console.WriteLine("Width of the cell value: " + width);
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


