---
title: "WorkbookSettings.FormulaSettings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings‑egenskap. Hämtar inställningarna för formelrelaterade funktioner"
type: docs
url: /sv/net/aspose.cells/workbooksettings/formulasettings/
---
## WorkbookSettings.FormulaSettings property

Hämtar inställningarna för formelrelaterade funktioner.

```csharp
public FormulaSettings FormulaSettings { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyFormulaSettingsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Kom åt och ändra FormulaSettings
            workbook.Settings.FormulaSettings.CalculationMode = CalcModeType.Manual;
            workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
            workbook.Settings.FormulaSettings.MaxIteration = 100;
            workbook.Settings.FormulaSettings.MaxChange = 0.001;

            // Visa inställningarna
            Console.WriteLine("Calculation Mode: " + workbook.Settings.FormulaSettings.CalculationMode);
            Console.WriteLine("Iterative Calculation Enabled: " + workbook.Settings.FormulaSettings.EnableIterativeCalculation);
            Console.WriteLine("Max Iterations: " + workbook.Settings.FormulaSettings.MaxIteration);
            Console.WriteLine("Max Change: " + workbook.Settings.FormulaSettings.MaxChange);
        }
    }
}
```

### Se även

* class [FormulaSettings](../../formulasettings/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


