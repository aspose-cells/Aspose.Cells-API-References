---
title: "MsoFormatPicture.IsBiLevel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MsoFormatPicture. Indique si cette image doit s'afficher en noir et blanc"
type: docs
url: /fr/net/aspose.cells.drawing/msoformatpicture/isbilevel/
---
## MsoFormatPicture.IsBiLevel property

Indique si cette image doit être affichée en noir et blanc à deux couleurs.

```csharp
public bool IsBiLevel { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyIsBiLevelDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une image à la feuille de calcul
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[index];
            
            // Définir l'image en niveau binaire (noir et blanc)
            picture.FormatPicture.IsBiLevel = true;
            
            // Vérifier et afficher la valeur de la propriété IsBiLevel
            Console.WriteLine("Picture is bi-level: " + picture.FormatPicture.IsBiLevel);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


