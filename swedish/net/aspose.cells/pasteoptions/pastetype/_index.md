---
title: "PasteOptions.PasteType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PasteOptions-egenskap. Typ av klistra-in-special"
type: docs
url: /sv/net/aspose.cells/pasteoptions/pastetype/
---
## PasteOptions.PasteType property

Specialklistringstypen.

```csharp
public PasteType PasteType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyPasteTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange källvärde
            worksheet.Cells["A1"].PutValue("SourceValue");

            // Skapa områden med fullständigt kvalificerade typnamn
            Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1");
            Aspose.Cells.Range targetRange = worksheet.Cells.CreateRange("B1:D3");

            // Kopiera med PasteType.All
            targetRange.Copy(sourceRange, new PasteOptions() { PasteType = PasteType.All });

            // Skriv ut resultat
            Console.WriteLine("A1: " + worksheet.Cells["A1"].StringValue);
            Console.WriteLine("B1: " + worksheet.Cells["B1"].StringValue);
            Console.WriteLine("C2: " + worksheet.Cells["C2"].StringValue);
            Console.WriteLine("D3: " + worksheet.Cells["D3"].StringValue);
        }
    }
}
```

### Se även

* enum [PasteType](../../pastetype/)
* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


