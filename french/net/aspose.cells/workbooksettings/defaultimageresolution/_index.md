---
title: "WorkbookSettings.DefaultImageResolution"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Obtient et définit la résolution par défaut de l'image"
type: docs
url: /fr/net/aspose.cells/workbooksettings/defaultimageresolution/
---
## WorkbookSettings.DefaultImageResolution property

Obtient et définit la résolution par défaut de l'image.

```csharp
public int DefaultImageResolution { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDefaultImageResolutionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Définir la résolution d'image par défaut
            workbook.Settings.DefaultImageResolution = 300;
            
            // Ajouter une feuille de calcul et insérer une image
            Worksheet worksheet = workbook.Worksheets[0];
            int imgIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[imgIndex];
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
            
            // Vérifier la résolution d'image par défaut
            Console.WriteLine("Default Image Resolution: " + workbook.Settings.DefaultImageResolution);
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


