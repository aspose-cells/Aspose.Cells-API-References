---
title: "FormulaSettings.ForceFullCalculation"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormulaSettings-egenskap. Anger om alla formler beräknas varje gång en beräkning utlöses"
type: docs
url: /sv/net/aspose.cells/formulasettings/forcefullcalculation/
---
## FormulaSettings.ForceFullCalculation property

Anger om alla formler beräknas varje gång en beräkning utlöses.

```csharp
public bool ForceFullCalculation { get; set; }
```

### Anmärkningar

Denna egenskap är endast för att spara inställningarna till den resulterande kalkylbladsfilen så att andra program (såsom MS Excel) kan agera därefter när de laddar och manipulerar den resulterande filen. Av prestandaskäl för de flesta användares applikationer beräknar vi inte någon formel i arbetsboken automatiskt, oavsett vilket värde som har satts för denna egenskap.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyForceFullCalculationDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till formelinställningarna
            FormulaSettings formulaSettings = workbook.Settings.FormulaSettings;

            // Demonstrera ForceFullCalculation-egenskapen
            formulaSettings.ForceFullCalculation = true;
            Console.WriteLine($"ForceFullCalculation is set to: {formulaSettings.ForceFullCalculation}");

            // Lägg till exempeldata och formel
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Beräkna formler med ForceFullCalculation-inställning
            workbook.CalculateFormula();

            // Skriv ut resultatet
            Console.WriteLine($"Calculation result: {worksheet.Cells["A3"].Value}");

            // Spara arbetsboken
            workbook.Save("ForceFullCalculationDemo.xlsx");
        }
    }
}
```

### Se även

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


