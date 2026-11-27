---
title: "Worksheet.GridlineColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Hämtar och anger färgen på rutnätslinjen"
type: docs
url: /sv/net/aspose.cells/worksheet/gridlinecolor/
---
## Worksheet.GridlineColor property

Hämtar och anger färgen på rutnätslinjen

```csharp
public Color GridlineColor { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyGridlineColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in rutnätslinjens färg till röd
            worksheet.GridlineColor = Color.Red;
            
            // Spara arbetsboken
            string outputPath = "GridlineColorDemo.xlsx";
            workbook.Save(outputPath);
            
            Console.WriteLine("Gridline color set to red and saved to: " + outputPath);
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


