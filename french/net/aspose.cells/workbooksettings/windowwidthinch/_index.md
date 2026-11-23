---
title: "WorkbookSettings.WindowWidthInch"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. La largeur de la fenêtre en unité de pouce"
type: docs
url: /fr/net/aspose.cells/workbooksettings/windowwidthinch/
---
## WorkbookSettings.WindowWidthInch property

La largeur de la fenêtre, en pouces.

```csharp
public double WindowWidthInch { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowWidthInchDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder aux paramètres du classeur
            WorkbookSettings settings = workbook.Settings;

            // Définir la largeur de la fenêtre en pouces
            settings.WindowWidthInch = 10.5;

            // Afficher la largeur de la fenêtre en pouces
            Console.WriteLine("Window Width in Inches: " + settings.WindowWidthInch);

            // Enregistrez le classeur
            workbook.Save("WindowWidthInchDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


