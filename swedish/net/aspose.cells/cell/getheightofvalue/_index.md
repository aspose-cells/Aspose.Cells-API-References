---
title: "Cell.GetHeightOfValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-metod. Hämtar höjden på värdet i enheten pixlar"
type: docs
url: /sv/net/aspose.cells/cell/getheightofvalue/
---
## Cell.GetHeightOfValue method

Hämtar värdets höjd i pixelenheter.

```csharp
public int GetHeightOfValue()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetHeightOfValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Sätt värde och mät höjd
            worksheet.Cells["A1"].PutValue("Sample Text");
            double height = worksheet.Cells["A1"].GetHeightOfValue();
            
            Console.WriteLine("Height of value in A1: " + height);
            
            // Justera radhöjd och mät igen
            worksheet.Cells.Rows[0].Height = 30;
            height = worksheet.Cells["A1"].GetHeightOfValue();
            
            Console.WriteLine("Height after row adjustment: " + height);
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


