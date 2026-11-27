---
title: "FormulaParseOptions.CheckAddIn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormulaParseOptions egenskap. Anger om tillägg ska kontrolleras i befintliga externa länkar i aktuell arbetsbok för användardefinierade funktioner utan extern länk. Standard är sant om användardefinierad funktion matchar ett tillägg i befintliga externa länkar, så tas det som tillägget"
type: docs
url: /sv/net/aspose.cells/formulaparseoptions/checkaddin/
---
## FormulaParseOptions.CheckAddIn property

Om tillägg ska kontrolleras i befintliga externa länkar i den aktuella arbetsboken för användardefinierade funktioner utan extern länk. Standard är true (om en användardefinierad funktion matchar ett tillägg i befintliga externa länkar, tas det som tillägget).

```csharp
public bool CheckAddIn { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaParseOptionsPropertyCheckAddInDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Registrera tilläggsfunktion
            wb.Worksheets.RegisterAddInFunction("Test.xlam", "TEST_UDF", false);

            // Utan CheckAddIn=false - formeln kommer att konverteras till tilläggsformat
            cells["A1"].SetFormula("=TEST_UDF()", new FormulaParseOptions());
            Console.WriteLine("A1 Formula (CheckAddIn=true): " + cells["A1"].Formula);

            // Med CheckAddIn=false - formeln förblir oförändrad
            cells["A2"].SetFormula("=TEST_UDF()", new FormulaParseOptions() { CheckAddIn = false });
            Console.WriteLine("A2 Formula (CheckAddIn=false): " + cells["A2"].Formula);
        }
    }
}
```

### Se även

* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


