---
title: "Workbook.Settings"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Workbook. Représente les paramètres du classeur"
type: docs
url: /fr/net/aspose.cells/workbook/settings/
---
## Workbook.Settings property

Représente les paramètres du classeur.

```csharp
public WorkbookSettings Settings { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertySettingsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder et modifier les paramètres
            workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
            workbook.Settings.FormulaSettings.MaxIteration = 30;
            workbook.Settings.FormulaSettings.MaxChange = 0.1;

            // Vérifier les paramètres
            Console.WriteLine("Iterative Calculation Enabled: " + 
                workbook.Settings.FormulaSettings.EnableIterativeCalculation);
            Console.WriteLine("Max Iterations: " + 
                workbook.Settings.FormulaSettings.MaxIteration);
            Console.WriteLine("Max Change: " + 
                workbook.Settings.FormulaSettings.MaxChange);

            // Enregistrez le classeur
            workbook.Save("WorkbookSettingsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../../workbooksettings/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


