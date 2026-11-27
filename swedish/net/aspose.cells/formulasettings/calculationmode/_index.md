---
title: "FormulaSettings.CalculationMode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormulaSettings-egenskap. Hämtar eller anger läget för arbetsboksberäkning i MS Excel"
type: docs
url: /sv/net/aspose.cells/formulasettings/calculationmode/
---
## FormulaSettings.CalculationMode property

Hämtar eller anger läget för arbetsboksberäkning i MS Excel.

```csharp
public CalcModeType CalculationMode { get; set; }
```

### Anmärkningar

Denna egenskap är endast för att spara inställningarna till den resulterande kalkylbladsfilen så att andra program (såsom MS Excel) kan agera därefter när de laddar och manipulerar den resulterande filen. Med hänsyn till prestanda för de flesta användarapplikationer beräknar vi inte någon formel i arbetsboken automatiskt, oavsett vilket läge som har satts för denna egenskap. Om användaren behöver beräkna formler, vänligen anropa alltid metoder på olika objekt enligt krav: [`CalculateFormula`](../../workbook/calculateformula/), [`CalculateFormula`](../../worksheet/calculateformula/), [`Calculate`](../../cell/calculate/), ...etc.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculationModeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Ställ in beräkningsläge till AutomaticExceptTable
            workbook.Settings.FormulaSettings.CalculationMode = CalcModeType.AutomaticExceptTable;
            Console.WriteLine("Calculation Mode: " + workbook.Settings.FormulaSettings.CalculationMode);

            // Ändra beräkningsläge till Manuell
            workbook.Settings.FormulaSettings.CalculationMode = CalcModeType.Manual;
            Console.WriteLine("Calculation Mode: " + workbook.Settings.FormulaSettings.CalculationMode);

            // Återställ till standardläget Automatic
            workbook.Settings.FormulaSettings.CalculationMode = CalcModeType.Automatic;
            Console.WriteLine("Calculation Mode: " + workbook.Settings.FormulaSettings.CalculationMode);
        }
    }
}
```

### Se även

* enum [CalcModeType](../../calcmodetype/)
* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


