---
title: "WorkbookSettings.WindowTop"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. La distance entre le bord supérieur de la zone client et le bord supérieur de la fenêtre, en points"
type: docs
url: /fr/net/aspose.cells/workbooksettings/windowtop/
---
## WorkbookSettings.WindowTop property

La distance du bord supérieur de la zone client au bord supérieur de la fenêtre, en points.

```csharp
public double WindowTop { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowTopDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez aux WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Définir la propriété WindowTop pour positionner la fenêtre à 100 pixels du haut
            settings.WindowTop = 100;
            
            // Vérifier la valeur de WindowTop
            Console.WriteLine("Window top position set to: " + settings.WindowTop);

            // Enregistrez le classeur
            workbook.Save("WindowTopDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


