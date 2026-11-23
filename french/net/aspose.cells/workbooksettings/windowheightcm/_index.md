---
title: "WorkbookSettings.WindowHeightCM"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. La hauteur de la fenêtre en unité de centimètre"
type: docs
url: /fr/net/aspose.cells/workbooksettings/windowheightcm/
---
## WorkbookSettings.WindowHeightCM property

La hauteur de la fenêtre, en centimètres.

```csharp
public double WindowHeightCM { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowHeightCMDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder aux paramètres du classeur
            WorkbookSettings settings = workbook.Settings;

            // Définir la propriété WindowHeightCM
            settings.WindowHeightCM = 15.5;

            // Afficher la valeur définie
            Console.WriteLine("Window Height in Centimeters: " + settings.WindowHeightCM);

            // Enregistrez le classeur
            workbook.Save("WindowHeightDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


