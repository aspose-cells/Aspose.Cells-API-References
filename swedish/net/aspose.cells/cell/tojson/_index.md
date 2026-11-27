---
title: "Cell.ToJson"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-metod. Konvertera Cell till JSON-strukturdata"
type: docs
url: /sv/net/aspose.cells/cell/tojson/
---
## Cell.ToJson method

Konvertera [`Cell`](../) till JSON-strukturdata.

```csharp
public string ToJson()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodToJsonDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ställ in exempeldata och stilar
            cells["A1"].PutValue(100);
            cells["B6"].Formula = "=A1";
            
            // Hämta cell och konvertera till JSON
            Cell cell = cells["B6"];
            string json = cell.ToJson();
            
            // Skriv ut JSON
            Console.WriteLine("Cell JSON:");
            Console.WriteLine(json);
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


