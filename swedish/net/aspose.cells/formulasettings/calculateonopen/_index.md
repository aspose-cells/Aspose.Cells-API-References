---
title: "FormulaSettings.CalculateOnOpen"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormulaSettings-egenskap. Anger om programmet är tvunget att utföra en fullständig beräkning när arbetsboken öppnas"
type: docs
url: /sv/net/aspose.cells/formulasettings/calculateonopen/
---
## FormulaSettings.CalculateOnOpen property

Anger om applikationen måste utföra en fullständig beräkning när arbetsboken öppnas.

```csharp
public bool CalculateOnOpen { get; set; }
```

### Anmärkningar

Denna egenskap är endast för att spara inställningarna till den resulterande kalkylbladsfilen så att andra program (såsom MS Excel) kan agera därefter när de laddar den resulterande filen. Med hänsyn till prestanda för de flesta användares program beräknar vi inte någon formel i arbetsboken automatiskt, oavsett vilket värde som har satts för denna egenskap.

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculateOnOpenDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in formel i cell A1 som refererar till B1
            worksheet.Cells["A1"].Formula = "=B1";
            
            // Ställ in värde i cell B1
            worksheet.Cells["B1"].PutValue(10);
            
            // Inaktivera automatisk formelberäkning vid öppning
            workbook.Settings.FormulaSettings.CalculateOnOpen = false;
            
            // Spara arbetsboken
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            // Öppna den sparade arbetsboken igen
            Workbook reopenedWorkbook = new Workbook("output.xlsx");
            
            // Verifiera att formeln inte beräknades vid öppning
            Console.WriteLine("A1 value (should be 0 before calculation): " + reopenedWorkbook.Worksheets[0].Cells["A1"].IntValue);
            
            // Beräkna formler manuellt
            reopenedWorkbook.CalculateFormula();
            
            // Verifiera att formeln beräknades
            Console.WriteLine("A1 value (should be 10 after calculation): " + reopenedWorkbook.Worksheets[0].Cells["A1"].IntValue);
        }
    }
}
```

### Se även

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


