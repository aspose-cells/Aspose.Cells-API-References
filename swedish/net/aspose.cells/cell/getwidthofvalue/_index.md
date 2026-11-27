---
title: "Cell.GetWidthOfValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell‑metod. Hämtar värdets bredd i enheten pixlar"
type: docs
url: /sv/net/aspose.cells/cell/getwidthofvalue/
---
## Cell.GetWidthOfValue method

Hämtar bredden på värdet i enheten pixlar.

```csharp
public int GetWidthOfValue()
```

### Exempel

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

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


