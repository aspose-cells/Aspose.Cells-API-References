---
title: "FormulaSettings.PreservePaddingSpaces"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormulaSettings-egenskapen. Anger om de mellanslag och radbrytningar som är utfyllda mellan formel‑token ska bevaras vid hämtning och inställning av formler. Standardvärdet är falskt"
type: docs
url: /sv/net/aspose.cells/formulasettings/preservepaddingspaces/
---
## FormulaSettings.PreservePaddingSpaces property

Anger om mellanslag och radbrytningar som är insatta mellan formeltoken ska bevaras vid hämtning och inställning av formler. Standardvärdet är falskt.

```csharp
public bool PreservePaddingSpaces { get; set; }
```

### Anmärkningar

Generellt är dessa mellanslag och radbrytningar bara för visuellt ändamål, att bevara dem eller inte påverkar inte det beräknade resultatet. Av prestandaskäl, om det inte finns något särskilt krav, är det bättre att inte bevara dem vid bearbetning av formler.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyPreservePaddingSpacesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange formel med utfyllda mellanslag
            string formulaWithSpaces = "=SUM( IF( A1:A5 > 10, B1:B5, 0 ) )";
            worksheet.Cells["C1"].Formula = formulaWithSpaces;
            
            // Standardbeteende (PreservePaddingSpaces är sant)
            Console.WriteLine("Formula with spaces preserved: " + worksheet.Cells["C1"].Formula);
            
            // Ändra inställning för att ta bort utfyllda mellanslag
            workbook.Settings.FormulaSettings.PreservePaddingSpaces = false;
            worksheet.Cells["C2"].Formula = formulaWithSpaces;
            
            Console.WriteLine("Formula with spaces removed: " + worksheet.Cells["C2"].Formula);
            
            // Spara arbetsboken
            workbook.Save("FormulaSpacesDemo.xlsx");
        }
    }
}
```

### Se även

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


