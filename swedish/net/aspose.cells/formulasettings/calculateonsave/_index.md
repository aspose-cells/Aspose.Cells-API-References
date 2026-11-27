---
title: "FormulaSettings.CalculateOnSave"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormulaSettings-egenskapen. Anger om arbetsboken ska beräknas om innan dokumentet sparas när man är i manuellt beräkningsläge"
type: docs
url: /sv/net/aspose.cells/formulasettings/calculateonsave/
---
## FormulaSettings.CalculateOnSave property

Anger om arbetsboken ska omberäknas innan dokumentet sparas, när man är i manuellt beräkningsläge.

```csharp
public bool CalculateOnSave { get; set; }
```

### Anmärkningar

Denna egenskap är endast för att spara inställningarna till den resulterande kalkylbladsfilen så att andra program (såsom MS Excel) kan agera därefter när de laddar och manipulerar den resulterande filen. Av prestandaskäl för de flesta användares applikationer beräknar vi inte någon formel i arbetsboken automatiskt, oavsett vilket värde som har satts för denna egenskap.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculateOnSaveDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till kalkylbladet och lägg till lite data
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Inaktivera CalculateOnSave (standard är falskt)
            workbook.Settings.FormulaSettings.CalculateOnSave = false;
            
            // Spara utan att beräkna formler
            workbook.Save("output_without_calculation.xlsx");

            // Aktivera CalculateOnSave
            workbook.Settings.FormulaSettings.CalculateOnSave = true;
            
            // Spara med formelberäkning
            workbook.Save("output_with_calculation.xlsx");
        }
    }
}
```

### Se även

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


