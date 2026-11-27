---
title: "Style.IsDateTime"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-egenskap. Anger om talformatet är ett datumformat"
type: docs
url: /sv/net/aspose.cells/style/isdatetime/
---
## Style.IsDateTime property

Anger om talformatet är ett datumformat.

```csharp
public bool IsDateTime { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsDateTimeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Ange ett numeriskt värde
            cells["A1"].PutValue(1230);
            
            // Hämta och ändra cellens stil
            Style style = cells["A1"].GetStyle();
            
            // Ställ in till datumformat (15 är det inbyggda datumformatet)
            style.Number = 15;
            Console.WriteLine("IsDateTime after setting Number=15: " + style.IsDateTime);
            
            // Ställ in anpassat datumformat
            style.Custom = "yyyy-mm-dd";
            Console.WriteLine("IsDateTime after setting custom date format: " + style.IsDateTime);
            
            // Applicera den ändrade stilen tillbaka till cellen
            cells["A1"].SetStyle(style);
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


