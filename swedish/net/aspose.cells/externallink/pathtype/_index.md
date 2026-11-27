---
title: "ExternalLink.PathType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalLink egenskap. Hämta sökvägstypen för denna externa länk"
type: docs
url: /sv/net/aspose.cells/externallink/pathtype/
---
## ExternalLink.PathType property

Hämta sökvägstypen för denna externa länk

```csharp
public string PathType { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyPathTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad
            Worksheet sheet = workbook.Worksheets[0];
            
            // Skapa en extern länk till en annan arbetsbok
            sheet.Cells["A1"].Formula = "='C:\\Temp\\ExternalWorkbook.xlsx'!Sheet1!A1";
            
            // Hämta den externa länken
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];
            
            // Visa sökvägstypen för den externa länken
            Console.WriteLine("Path Type: " + externalLink.PathType);
            
            // Spara arbetsboken
            workbook.Save("ExternalLinkDemo.xlsx");
        }
    }
}
```

### Se även

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


