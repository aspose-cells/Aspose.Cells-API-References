---
title: "CopyOptions.CopyInvalidFormulasAsValues"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CopyOptions-egenskap. Om formeln inte är giltig för destinationsarbetsboken kopieras endast värden"
type: docs
url: /sv/net/aspose.cells/copyoptions/copyinvalidformulasasvalues/
---
## CopyOptions.CopyInvalidFormulasAsValues property

Om formeln inte är giltig för destinationsmålet, kopieras endast värden.

```csharp
public bool CopyInvalidFormulasAsValues { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyCopyInvalidFormulasAsValuesDemo
    {
        public static void Run()
        {
            // Skapa en källarbetsbok med ett exempelarbetsblad
            Workbook srcWorkbook = new Workbook();
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            
            // Lägg till en formel som kan vara ogiltig i vissa sammanhang
            srcSheet.Cells["A1"].Formula = "=1/0"; // Division by zero - invalid formula
            srcSheet.Cells["A2"].Value = "Valid Data";

            // Skapa en målarbetsbok
            Workbook destWorkbook = new Workbook();
            
            // Ställ in kopieringsalternativ för att konvertera ogiltiga formler till värden
            CopyOptions copyOptions = new CopyOptions();
            copyOptions.CopyInvalidFormulasAsValues = true;

            // Kopiera kalkylbladet med alternativen
            destWorkbook.Worksheets[0].Copy(srcSheet, copyOptions);

            // Verifiera resultaten
            Console.WriteLine("A1 (invalid formula copied as value): " + 
                destWorkbook.Worksheets[0].Cells["A1"].Value); // Should show #DIV/0! as value
            Console.WriteLine("A2 (valid data): " + 
                destWorkbook.Worksheets[0].Cells["A2"].Value); // Should show "Valid Data"
        }
    }
}
```

### Se även

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


