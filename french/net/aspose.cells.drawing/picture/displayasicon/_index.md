---
title: "Picture.DisplayAsIcon"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Picture. Vrai si l'objet spécifié est affiché sous forme d'icône et que l'image ne sera pas modifiée automatiquement"
type: docs
url: /fr/net/aspose.cells.drawing/picture/displayasicon/
---
## Picture.DisplayAsIcon property

Vrai si l'objet spécifié est affiché sous forme d'icône et que l'image ne sera pas modifiée automatiquement.

```csharp
public bool DisplayAsIcon { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyDisplayAsIconDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une image à la feuille de calcul
            int pictureIndex = worksheet.Pictures.Add(1, 1, "example.ico");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Définir la propriété DisplayAsIcon sur vrai
            picture.DisplayAsIcon = true;
            
            // Définir d'autres propriétés de l'image
            picture.Name = "IconDisplay";
            picture.Height = 100;
            picture.Width = 100;

            // Enregistrez le classeur
            workbook.Save("DisplayAsIconDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Workbook saved with icon display picture.");
        }
    }
}
```

### Voir aussi

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


