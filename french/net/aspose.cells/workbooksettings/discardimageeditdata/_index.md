---
title: "WorkbookSettings.DiscardImageEditData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Indique si les données d'édition d'image sont supprimées"
type: docs
url: /fr/net/aspose.cells/workbooksettings/discardimageeditdata/
---
## WorkbookSettings.DiscardImageEditData property

Indique si les données d'image en cours d'édition sont abandonnées.

```csharp
public bool DiscardImageEditData { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDiscardImageEditDataDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une image à la feuille de calcul
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[index];
            
            // Définir DiscardImageEditData sur true (false par défaut)
            workbook.Settings.DiscardImageEditData = true;
            
            // Enregistrez le classeur
            workbook.Save("output_with_discarded_image_data.xlsx", SaveFormat.Xlsx);
            
            // Vérifier que le paramètre a été appliqué
            Console.WriteLine("DiscardImageEditData is set to: " + workbook.Settings.DiscardImageEditData);
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


