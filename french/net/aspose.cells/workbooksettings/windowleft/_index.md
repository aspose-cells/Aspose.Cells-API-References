---
title: "WorkbookSettings.WindowLeft"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. La distance du bord gauche de la zone client au bord gauche de la fenêtre, en points"
type: docs
url: /fr/net/aspose.cells/workbooksettings/windowleft/
---
## WorkbookSettings.WindowLeft property

La distance du bord gauche de la zone client au bord gauche de la fenêtre, en points.

```csharp
public double WindowLeft { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowLeftDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez aux WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Définir la propriété WindowLeft pour positionner la fenêtre à 100 pixels du bord gauche
            settings.WindowLeft = 100;

            // Définir d'autres propriétés de fenêtre à des fins de démonstration
            settings.WindowTop = 50;
            settings.WindowWidth = 800;
            settings.WindowHeight = 600;

            // Ajouter des données d'exemple à la feuille de calcul
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Window Position Demo");
            sheet.Cells["A2"].PutValue($"Left: {settings.WindowLeft}px");
            sheet.Cells["A3"].PutValue($"Top: {settings.WindowTop}px");

            // Enregistrez le classeur
            workbook.Save("WindowPositionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


