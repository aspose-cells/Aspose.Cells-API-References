---
title: "WorkbookSettings.WindowTopInch"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. La distance entre le bord supérieur de la zone client et le bord supérieur de la fenêtre, exprimée en pouces"
type: docs
url: /fr/net/aspose.cells/workbooksettings/windowtopinch/
---
## WorkbookSettings.WindowTopInch property

La distance du bord supérieur de la zone client au bord supérieur de la fenêtre, en pouces.

```csharp
public double WindowTopInch { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowTopInchDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez aux WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Définir la propriété WindowTopInch pour positionner la fenêtre à 2 pouces du haut
            settings.WindowTopInch = 2.0;

            // Vérifier le paramètre en l'affichant
            Console.WriteLine("Window top position (inches): " + settings.WindowTopInch);

            // Enregistrez le classeur
            workbook.Save("WindowTopInchDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


