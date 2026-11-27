---
title: "CalculationOptions.CharacterEncoding"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CalculationOptions-egenskapen. Anger den kodning som används för kodning/avkodning av tecken vid beräkning av formler. För funktioner såsom CHAR CODE beror det beräknade resultatet på regionsinställningarna och standardteckenuppsättningen i miljön. Med denna egenskap kan användaren specificera rätt kodning som används för dessa funktioner för att få det förväntade resultatet"
type: docs
url: /sv/net/aspose.cells/calculationoptions/characterencoding/
---
## CalculationOptions.CharacterEncoding property

Anger den kodning som används för kodning/avkodning av tecken vid beräkning av formler. För funktioner såsom CHAR, CODE beror det beräknade resultatet på regioninställningarna och standardteckenuppsättningen i miljön. Med den här egenskapen kan användaren ange rätt kodning som används för dessa funktioner för att få det förväntade resultatet.

```csharp
public Encoding CharacterEncoding { get; set; }
```

### Exempel

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyCharacterEncodingDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            wb.Settings.Region = CountryCode.Japan;
            
            CalculationOptions copts = new CalculationOptions();
            copts.CharacterEncoding = Encoding.GetEncoding("iso-2022-jp");
            
            string formula = "=TRIM(1)";
            string result = (string)sheet.CalculateFormula(formula, copts);
            
            Console.WriteLine("Calculation result: " + result);
        }
    }
}
```

### Se även

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


