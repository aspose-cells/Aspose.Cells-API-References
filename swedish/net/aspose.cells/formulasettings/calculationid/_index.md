---
title: "FormulaSettings.CalculationId"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormulaSettings-egenskap. Anger versionen av beräkningsmotorn som används för att beräkna värden i arbetsboken"
type: docs
url: /sv/net/aspose.cells/formulasettings/calculationid/
---
## FormulaSettings.CalculationId property

Anger versionen av beräkningsmotorn som används för att beräkna värden i arbetsboken.

```csharp
public string CalculationId { get; set; }
```

### Anmärkningar

Denna egenskap är endast för att spara inställningarna till den resulterande kalkylbladsfilen så att andra program (såsom MS Excel) kan agera därefter när de laddar och manipulerar den resulterande filen. I fallet med MS Excel, om värdet på denna egenskap är mindre än identifieraren för omberäkningsmotorn som är associerad med programmet som öppnar den resulterande filen, kommer programmet att omberäkna resultaten av alla formler i arbetsboken omedelbart efter att filen har laddats. Med hänsyn till prestanda för de flesta användares program beräknar vi inte någon formel i arbetsboken automatiskt, oavsett vilket värde som har satts för denna egenskap.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculationIdDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Ställ in formel som beter sig olika baserat på CalculationId
            Cell cell = sheet.Cells["A1"];
            cell.Formula = "=AND(\"a\",true)";
            
            // Beräkna utan CalculationId (standardbeteende)
            wb.CalculateFormula();
            Console.WriteLine("Without CalculationId: " + cell.Value);
            
            // Ställ in CalculationId och beräkna om
            wb.Settings.FormulaSettings.CalculationId = "181029";
            wb.CalculateFormula();
            Console.WriteLine("With CalculationId 181029: " + cell.BoolValue);
        }
    }
}
```

### Se även

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


