---
title: "WorkbookSettings.WindowWidth"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. La largeur de la fenêtre en unité de point"
type: docs
url: /fr/net/aspose.cells/workbooksettings/windowwidth/
---
## WorkbookSettings.WindowWidth property

La largeur de la fenêtre, en points.

```csharp
public double WindowWidth { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowWidthDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez aux WorkbookSettings
            WorkbookSettings settings = workbook.Settings;
            
            // Définir la propriété WindowWidth
            settings.WindowWidth = 800;
            
            // Vérifier la valeur de WindowWidth
            Console.WriteLine("Window Width set to: " + settings.WindowWidth);
            
            // Enregistrez le classeur
            workbook.Save("WindowWidthDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


