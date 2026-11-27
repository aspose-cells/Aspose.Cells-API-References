---
title: "Style.ShrinkToFit"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-egenskap. Representerar om text automatiskt krymper för att passa den tillgängliga kolumnbredden"
type: docs
url: /sv/net/aspose.cells/style/shrinktofit/
---
## Style.ShrinkToFit property

Representerar om text automatiskt krymper för att passa i den tillgängliga kolumnbredden.

```csharp
public bool ShrinkToFit { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyShrinkToFitDemo
    {
        public static void Run()
        {
            // Skapa ett arbetsbok-objekt
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till cells-samlingen
            Cells cells = worksheet.Cells;
            
            // Sätt in lite text i cell A1 som är längre än kolumnbredden
            cells["A1"].PutValue("This is a long text that needs shrinking to fit");
            
            // Ställ in kolumnbredden så att den är mindre än textlängden
            cells.SetColumnWidth(0, 10);
            
            // Hämta stilen för cell A1
            Style style = cells["A1"].GetStyle();
            
            // Ställ in ShrinkToFit till true
            style.ShrinkToFit = true;
            
            // Applicera stilen på cell A1
            cells["A1"].SetStyle(style);
            
            // Spara arbetsboken
            workbook.Save("ShrinkToFitDemo.xlsx");
            
            Console.WriteLine("ShrinkToFit demo completed successfully.");
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


