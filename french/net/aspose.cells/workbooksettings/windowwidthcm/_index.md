---
title: "WorkbookSettings.WindowWidthCM"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. La largeur de la fenêtre en unité de centimètre"
type: docs
url: /fr/net/aspose.cells/workbooksettings/windowwidthcm/
---
## WorkbookSettings.WindowWidthCM property

La largeur de la fenêtre, en centimètres.

```csharp
public double WindowWidthCM { get; set; }
```

### Exemples

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowWidthCMDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez aux WorkbookSettings
            WorkbookSettings settings = workbook.Settings;
            
            // Définir la propriété WindowWidthCM (20,32 cm = ~8 pouces)
            settings.WindowWidthCM = 20.32;
            
            // Vérifier le paramètre en l'affichant
            Console.WriteLine("Window Width in Centimeters: " + settings.WindowWidthCM);
            
            // Enregistrez le classeur
            workbook.Save("WindowWidthCMDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


