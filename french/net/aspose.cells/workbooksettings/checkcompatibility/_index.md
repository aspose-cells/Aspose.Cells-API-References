---
title: "WorkbookSettings.CheckCompatibility"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Indique si la vérification de compatibilité avec les versions antérieures doit être effectuée lors de l'enregistrement du classeur"
type: docs
url: /fr/net/aspose.cells/workbooksettings/checkcompatibility/
---
## WorkbookSettings.CheckCompatibility property

Indique si la compatibilité avec les versions antérieures est vérifiée lors de l'enregistrement du workbook.

```csharp
public bool CheckCompatibility { get; set; }
```

### Remarques

La valeur par défaut est true. Seulement pour les fichiers Excel97-2003 xls ou xlt.

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyCheckCompatibilityDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Définir CheckCompatibility sur true et enregistrer
            workbook.Settings.CheckCompatibility = true;
            workbook.Save("CheckCompatibilityDemo_true.xlsx");
            
            // Recharger et vérifier
            workbook = new Workbook("CheckCompatibilityDemo_true.xlsx");
            Console.WriteLine("CheckCompatibility (true): " + workbook.Settings.CheckCompatibility);
            
            // Définir CheckCompatibility sur false et enregistrer
            workbook.Settings.CheckCompatibility = false;
            workbook.Save("CheckCompatibilityDemo_false.xlsx");
            
            // Recharger et vérifier
            workbook = new Workbook("CheckCompatibilityDemo_false.xlsx");
            Console.WriteLine("CheckCompatibility (false): " + workbook.Settings.CheckCompatibility);
            
            // Démontrer les opérations de couleur
            Console.WriteLine("Is Red in palette: " + workbook.IsColorInPalette(Color.Red));
            Color customColor = workbook.GetMatchingColor(Color.FromArgb(255, 123, 123, 123));
            Console.WriteLine("Matching color R value: " + customColor.R);
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


