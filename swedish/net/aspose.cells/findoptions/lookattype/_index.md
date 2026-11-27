---
title: "FindOptions.LookAtType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FindOptions‑egenskap. Titta på typ"
type: docs
url: /sv/net/aspose.cells/findoptions/lookattype/
---
## FindOptions.LookAtType property

Titta på typen.

```csharp
public LookAtType LookAtType { get; set; }
```

### Anmärkningar

När ``[`RegexKey`](../regexkey/)`` är true och användaren har angett den exakta regeln för regexen, bör denna egenskap av prestandaskäl sättas till EntireContent. Annars kommer vi att omstrukturera söknyckeln för att säkerställa att den kan matchas enligt den specifika typen. Till exempel, när typen är Contains (detta är standardvärdet för denna egenskap), kommer vi automatiskt att lägga till jokertecken i början och slutet av söknyckeln. I detta fall blir reguljära uttryck mer komplexa och prestandan minskar också.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyLookAtTypeDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok och lägg till lite data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Hello World");
            worksheet.Cells["A2"].PutValue("=1+2"); // Formula
            worksheet.Cells["A3"].PutValue("Partial match test");
            worksheet.Cells["A4"].PutValue("=A1&A3"); // Formula concatenating cells

            // Skapa sökalternativ med LookAtType.EntireContent
            FindOptions options = new FindOptions
            {
                LookInType = LookInType.OnlyFormulas,
                LookAtType = LookAtType.EntireContent
            };

            // Sök efter formel som exakt matchar "=A1&A3"
            Cell cell = worksheet.Cells.Find("=A1&A3", null, options);
            Console.WriteLine("Found cell with exact formula match: " + (cell != null ? cell.Name : "null"));

            // Ändra till partiell matchning
            options.LookAtType = LookAtType.Contains;
            cell = worksheet.Cells.Find("A3", null, options);
            Console.WriteLine("Found cell containing 'A3' in formula: " + (cell != null ? cell.Name : "null"));
        }
    }
}
```

### Se även

* enum [LookAtType](../../lookattype/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


