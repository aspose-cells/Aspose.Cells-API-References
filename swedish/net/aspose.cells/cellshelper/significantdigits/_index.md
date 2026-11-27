---
title: "CellsHelper.SignificantDigits"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsHelper-egenskap. Hämtar och anger antalet signifikanta siffror. Standardvärdet är 17"
type: docs
url: /sv/net/aspose.cells/cellshelper/significantdigits/
---
## CellsHelper.SignificantDigits property

Hämtar och anger antalet signifikanta siffror. Standardvärdet är 17.

```csharp
[Obsolete("Use SignificantDigitsType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static int SignificantDigits { get; set; }
```

### Anmärkningar

Kan nu bara vara 15 eller 17. OBS: Denna medlem är nu föråldrad. Använd istället [`SignificantDigitsType`](../significantdigitstype/). Denna egenskap kommer att tas bort 12 månader senare från och med juni 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertySignificantDigitsDemo
    {
        public static void Run()
        {
            // Ange signifikanta siffror
            CellsHelper.SignificantDigits = 15;
            
            // Demonstrera egenskapens användning
            Console.WriteLine("Significant Digits: " + CellsHelper.SignificantDigits);
            
            // Skapa en arbetsbok för att demonstrera signifikanta siffror i beräkningar
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange värden som kommer att påverkas av signifikanta siffror
            worksheet.Cells["A1"].PutValue(1.2345678912345678);
            worksheet.Cells["A2"].PutValue(1.2345678912345678);
            worksheet.Cells["A3"].Formula = "=A1+A2";
            
            // Beräkna formler med de angivna signifikanta siffrorna
            workbook.CalculateFormula();
            
            // Skriv ut resultaten
            Console.WriteLine("Value with significant digits: " + worksheet.Cells["A3"].Value);
        }
    }
}
```

### Se även

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


