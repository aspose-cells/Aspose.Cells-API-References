---
title: "Worksheet.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Representerar worksheet-typ"
type: docs
url: /sv/net/aspose.cells/worksheet/type/
---
## Worksheet.Type property

Representerar arbetsbladstyp.

```csharp
public SheetType Type { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in några grundläggande egenskaper
            worksheet.Name = "DemoSheet";
            worksheet.IsVisible = true;
            
            // Demonstrera användning av Type-egenskapen
            Console.WriteLine("Worksheet Type: " + worksheet.Type);
            
            // Lägg till ett diagramblad för att demonstrera olika worksheet-typ
            workbook.Worksheets.Add(SheetType.Chart);
            Worksheet chartSheet = workbook.Worksheets[1];
            
            // Jämför worksheet-typer
            Console.WriteLine("Regular Sheet Type: " + worksheet.Type);
            Console.WriteLine("Chart Sheet Type: " + chartSheet.Type);
            
            // Spara arbetsboken
            workbook.Save("WorksheetTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [SheetType](../../sheettype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


