---
title: "Worksheet.BackgroundImage"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Obtient et définit l'image d'arrière-plan de la feuille de calcul"
type: docs
url: /fr/net/aspose.cells/worksheet/backgroundimage/
---
## Worksheet.BackgroundImage property

Obtient et définit l'image d'arrière-plan de la feuille de calcul.

```csharp
public byte[] BackgroundImage { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyBackgroundImageDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Obtenir la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Chemin du fichier image
            string imagePath = "background.jpg";
            
            // Lire le fichier image dans un tableau d'octets
            byte[] imageData = File.ReadAllBytes(imagePath);
            
            // Définir l'image d'arrière-plan pour la feuille de calcul
            worksheet.BackgroundImage = imageData;
            
            // Enregistrez le classeur
            workbook.Save("WorksheetWithBackground.xlsx");
            
            Console.WriteLine("Worksheet background image set successfully.");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


