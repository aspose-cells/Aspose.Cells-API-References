---
title: "WorkbookSettings.FormulaSettings"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Obtient les paramètres des fonctionnalités liées aux formules"
type: docs
url: /fr/net/aspose.cells/workbooksettings/formulasettings/
---
## WorkbookSettings.FormulaSettings property

Obtient les paramètres des fonctionnalités liées aux formules.

```csharp
public FormulaSettings FormulaSettings { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyFormulaSettingsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder et modifier FormulaSettings
            workbook.Settings.FormulaSettings.CalculationMode = CalcModeType.Manual;
            workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
            workbook.Settings.FormulaSettings.MaxIteration = 100;
            workbook.Settings.FormulaSettings.MaxChange = 0.001;

            // Afficher les paramètres
            Console.WriteLine("Calculation Mode: " + workbook.Settings.FormulaSettings.CalculationMode);
            Console.WriteLine("Iterative Calculation Enabled: " + workbook.Settings.FormulaSettings.EnableIterativeCalculation);
            Console.WriteLine("Max Iterations: " + workbook.Settings.FormulaSettings.MaxIteration);
            Console.WriteLine("Max Change: " + workbook.Settings.FormulaSettings.MaxChange);
        }
    }
}
```

### Voir aussi

* class [FormulaSettings](../../formulasettings/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


