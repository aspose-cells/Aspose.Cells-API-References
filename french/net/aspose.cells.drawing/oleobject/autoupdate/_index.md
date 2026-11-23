---
title: "OleObject.AutoUpdate"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété OleObject. Spécifie si le lien vers l'OleObject est mis à jour automatiquement ou non"
type: docs
url: /fr/net/aspose.cells.drawing/oleobject/autoupdate/
---
## OleObject.AutoUpdate property

Spécifie si le lien vers l'OleObject est mis à jour automatiquement ou non.

```csharp
public bool AutoUpdate { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyAutoUpdateDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Créer des fichiers d'exemple pour la démonstration
            string imagePath = "OleObjectExample.jpg";
            string excelPath = "OleObjectExample.xls";
            
            // Créer un fichier image d'exemple s'il n'existe pas
            if (!File.Exists(imagePath))
            {
                using (File.Create(imagePath)) { }
            }

            // Créer un fichier Excel d'exemple s'il n'existe pas
            if (!File.Exists(excelPath))
            {
                new Workbook().Save(excelPath);
            }

            // Lire les données d'image
            byte[] imageData = File.ReadAllBytes(imagePath);
            
            // Ajouter OleObject à la feuille de calcul
            int oleIndex = sheet.OleObjects.Add(1, 1, 200, 200, imageData);
            Aspose.Cells.Drawing.OleObject oleObject = sheet.OleObjects[oleIndex];
            
            // Définir les propriétés OleObject
            oleObject.ObjectData = File.ReadAllBytes(excelPath);
            oleObject.ProgID = "Excel.Sheet.8";
            oleObject.DisplayAsIcon = true;
            
            // Démontrer la propriété AutoUpdate
            oleObject.AutoUpdate = false; // When false, the object won't update automatically when source changes
            
            // Enregistrez le classeur
            workbook.Save("OleObjectAutoUpdateDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


