---
title: "WorkbookSettings.WindowTopCM"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. La distance entre le bord supérieur de la zone client et le bord supérieur de la fenêtre, exprimée en centimètres"
type: docs
url: /fr/net/aspose.cells/workbooksettings/windowtopcm/
---
## WorkbookSettings.WindowTopCM property

La distance du bord supérieur de la zone client au bord supérieur de la fenêtre, en centimètres.

```csharp
public double WindowTopCM { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowTopCMDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder aux paramètres du classeur
            WorkbookSettings settings = workbook.Settings;

            // Définir la propriété WindowTopCM (position depuis le haut en centimètres)
            settings.WindowTopCM = 2.5;

            // Afficher la valeur actuelle de WindowTopCM
            Console.WriteLine("Window Top Position (cm): " + settings.WindowTopCM);

            // Enregistrez le classeur
            workbook.Save("WindowTopCMDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


