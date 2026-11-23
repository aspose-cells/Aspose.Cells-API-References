---
title: "WorkbookSettings.AutoCompressPictures"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Spécifie une valeur booléenne qui indique que l'application compresse automatiquement les images dans le classeur"
type: docs
url: /fr/net/aspose.cells/workbooksettings/autocompresspictures/
---
## WorkbookSettings.AutoCompressPictures property

Spécifie une valeur booléenne qui indique que l'application compresse automatiquement les images dans le classeur.

```csharp
public bool AutoCompressPictures { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyAutoCompressPicturesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Activer AutoCompressPictures
            workbook.Settings.AutoCompressPictures = true;
            
            // Ajouter une image d'exemple pour démontrer la compression
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Pictures.Add(0, 0, "example.jpg");
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
            
            // Charger le classeur enregistré pour vérifier le paramètre
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("AutoCompressPictures: " + loadedWorkbook.Settings.AutoCompressPictures);
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


