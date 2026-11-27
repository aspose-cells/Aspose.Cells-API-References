---
title: "Workbook.Settings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-egenskap. Representerar arbetsbokens inställningar"
type: docs
url: /sv/net/aspose.cells/workbook/settings/
---
## Workbook.Settings property

Representerar arbetsbokens inställningar.

```csharp
public WorkbookSettings Settings { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertySettingsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Kom åt och ändra inställningar
            workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
            workbook.Settings.FormulaSettings.MaxIteration = 30;
            workbook.Settings.FormulaSettings.MaxChange = 0.1;

            // Verifiera inställningar
            Console.WriteLine("Iterative Calculation Enabled: " + 
                workbook.Settings.FormulaSettings.EnableIterativeCalculation);
            Console.WriteLine("Max Iterations: " + 
                workbook.Settings.FormulaSettings.MaxIteration);
            Console.WriteLine("Max Change: " + 
                workbook.Settings.FormulaSettings.MaxChange);

            // Spara arbetsboken
            workbook.Save("WorkbookSettingsDemo.xlsx");
        }
    }
}
```

### Se även

* class [WorkbookSettings](../../workbooksettings/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


