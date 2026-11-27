---
title: "WorkbookSettings.CheckCompatibility"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings-egenskap. Anger om kompatibilitetskontroll med tidigare versioner ska utföras när arbetsboken sparas"
type: docs
url: /sv/net/aspose.cells/workbooksettings/checkcompatibility/
---
## WorkbookSettings.CheckCompatibility property

Anger om kompatibilitet med tidigare versioner ska kontrolleras när arbetsboken sparas.

```csharp
public bool CheckCompatibility { get; set; }
```

### Anmärkningar

Standardvärdet är true. Endast för Excel97-2003 xls- eller xlt-filer.

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyCheckCompatibilityDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Ställ in CheckCompatibility till true och spara
            workbook.Settings.CheckCompatibility = true;
            workbook.Save("CheckCompatibilityDemo_true.xlsx");
            
            // Läs om och verifiera
            workbook = new Workbook("CheckCompatibilityDemo_true.xlsx");
            Console.WriteLine("CheckCompatibility (true): " + workbook.Settings.CheckCompatibility);
            
            // Ställ in CheckCompatibility till false och spara
            workbook.Settings.CheckCompatibility = false;
            workbook.Save("CheckCompatibilityDemo_false.xlsx");
            
            // Läs om och verifiera
            workbook = new Workbook("CheckCompatibilityDemo_false.xlsx");
            Console.WriteLine("CheckCompatibility (false): " + workbook.Settings.CheckCompatibility);
            
            // Demonstrera färgoperationer
            Console.WriteLine("Is Red in palette: " + workbook.IsColorInPalette(Color.Red));
            Color customColor = workbook.GetMatchingColor(Color.FromArgb(255, 123, 123, 123));
            Console.WriteLine("Matching color R value: " + customColor.R);
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


