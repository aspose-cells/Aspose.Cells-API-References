---
title: "WorkbookSettings.WindowHeightInch"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. La hauteur de la fenêtre en unités de pouce"
type: docs
url: /fr/net/aspose.cells/workbooksettings/windowheightinch/
---
## WorkbookSettings.WindowHeightInch property

La hauteur de la fenêtre, en pouces.

```csharp
public double WindowHeightInch { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowHeightInchDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder aux paramètres du classeur
            WorkbookSettings settings = workbook.Settings;

            // Définir la hauteur de la fenêtre en pouces
            settings.WindowHeightInch = 5.5;

            // Afficher la hauteur de la fenêtre en pouces
            Console.WriteLine("Window Height in Inches: " + settings.WindowHeightInch);

            // Enregistrez le classeur
            workbook.Save("WindowHeightInchDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


