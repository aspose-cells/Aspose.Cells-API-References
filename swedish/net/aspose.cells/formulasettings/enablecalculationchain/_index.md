---
title: "FormulaSettings.EnableCalculationChain"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormulaSettings-egenskap. Anger om beräkningskedjan ska aktiveras för formler. Standard är falskt"
type: docs
url: /sv/net/aspose.cells/formulasettings/enablecalculationchain/
---
## FormulaSettings.EnableCalculationChain property

Anger om beräkningskedjan för formler ska aktiveras. Standard är falskt.

```csharp
public bool EnableCalculationChain { get; set; }
```

### Anmärkningar

När det finns många formler i arbetsboken och användaren behöver beräkna dem upprepade gånger genom att bara ändra en liten del av dem, kan det vara fördelaktigt för prestandan att aktivera beräkningskedjan. Å andra sidan, om kedjan är aktiverad kräver underhållet av kedjemodellen extra minne, och det kräver också lite mer CPU-tid för vissa andra operationer såsom att ändra en cells värde eller formler. Efter att denna egenskap har ändrats från falskt till sant kommer beräkningskedjan att analyseras och byggas vid den första beräkningen av arbetsboken, så den tid som krävs för den första beräkningen kan bli längre än en normal beräkning utan kedja.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyEnableCalculationChainDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempel på formler
            worksheet.Cells["A1"].Formula = "=1+2";
            worksheet.Cells["A2"].Formula = "=A1*3";
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";
            
            // Inaktivera beräkningskedja
            workbook.Settings.FormulaSettings.EnableCalculationChain = false;
            
            // Beräkna formler
            workbook.CalculateFormula();
            
            // Spara arbetsboken
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with calculation chain disabled.");
        }
    }
}
```

### Se även

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


