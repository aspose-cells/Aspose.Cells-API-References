---
title: "WorkbookSettings.WindowLeftInch"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. La distance entre le bord gauche de la zone client et le bord gauche de la fenêtre. En unité de pouce"
type: docs
url: /fr/net/aspose.cells/workbooksettings/windowleftinch/
---
## WorkbookSettings.WindowLeftInch property

La distance du bord gauche de la zone client au bord gauche de la fenêtre, en pouces.

```csharp
public double WindowLeftInch { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowLeftInchDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez aux WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Définir la propriété WindowLeftInch
            settings.WindowLeftInch = 1.5; // Position window 1.5 inches from left edge of screen

            // Ajoutez des données d'exemple pour démontrer que le classeur fonctionne
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Window Position Demo");
            sheet.Cells["A2"].PutValue($"Window left position: {settings.WindowLeftInch} inches");

            // Enregistrez le classeur
            workbook.Save("WindowLeftInchDemo.xlsx");

            Console.WriteLine("Workbook saved with WindowLeftInch = " + settings.WindowLeftInch);
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


