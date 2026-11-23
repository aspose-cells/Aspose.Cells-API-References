---
title: "Picture.IsAutoSize"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Picture. True indique que la taille de l'objet ole sera automatiquement modifiée en fonction de la taille de l'instantané du contenu intégré lorsque l'objet ole est activé"
type: docs
url: /fr/net/aspose.cells.drawing/picture/isautosize/
---
## Picture.IsAutoSize property

Vrai indique que la taille de l'objet OLE sera automatiquement modifiée en fonction de la taille de l'instantané du contenu intégré lorsque l'objet OLE est activé.

```csharp
public bool IsAutoSize { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyIsAutoSizeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une image à la feuille de calcul
            int pictureIndex = worksheet.Pictures.Add(1, 1, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Démontrer la propriété IsAutoSize
            Console.WriteLine("Original IsAutoSize value: " + picture.IsAutoSize);
            
            // Définir IsAutoSize sur true - l'image sera automatiquement redimensionnée pour s'adapter à son contenu
            picture.IsAutoSize = true;
            Console.WriteLine("After setting IsAutoSize to true: " + picture.IsAutoSize);
            
            // Définir IsAutoSize sur false - l'image conservera ses dimensions originales
            picture.IsAutoSize = false;
            Console.WriteLine("After setting IsAutoSize to false: " + picture.IsAutoSize);

            // Enregistrez le classeur
            workbook.Save("PicturePropertyIsAutoSizeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


