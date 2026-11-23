---
title: "WorkbookSettings.WindowLeftCM"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. La distance entre le bord gauche de la zone client et le bord gauche de la fenêtre. En centimètres"
type: docs
url: /fr/net/aspose.cells/workbooksettings/windowleftcm/
---
## WorkbookSettings.WindowLeftCM property

La distance du bord gauche de la zone client au bord gauche de la fenêtre, en centimètres.

```csharp
public double WindowLeftCM { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowLeftCMDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez aux WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Définir la propriété WindowLeftCM (distance du bord gauche de l'écran en centimètres)
            settings.WindowLeftCM = 2.54; // 1 inch = 2.54 cm

            // Vérifier le paramètre en l'affichant
            Console.WriteLine("WindowLeftCM: " + settings.WindowLeftCM);

            // Enregistrez le classeur
            workbook.Save("WindowLeftCMDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


