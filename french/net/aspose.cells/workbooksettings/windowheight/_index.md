---
title: "WorkbookSettings.WindowHeight"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. La hauteur de la fenêtre en unité de point"
type: docs
url: /fr/net/aspose.cells/workbooksettings/windowheight/
---
## WorkbookSettings.WindowHeight property

La hauteur de la fenêtre, en points.

```csharp
public double WindowHeight { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowHeightDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez aux WorkbookSettings
            WorkbookSettings settings = workbook.Settings;
            
            // Définir la propriété WindowHeight
            settings.WindowHeight = 600;
            
            // Vérifier la valeur de WindowHeight
            Console.WriteLine("Window Height set to: " + settings.WindowHeight);
            
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


