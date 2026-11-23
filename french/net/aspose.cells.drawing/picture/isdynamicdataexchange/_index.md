---
title: "Picture.IsDynamicDataExchange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Picture. Obtient ou définit si l'échange dynamique de données est activé"
type: docs
url: /fr/net/aspose.cells.drawing/picture/isdynamicdataexchange/
---
## Picture.IsDynamicDataExchange property

Obtient ou définit si l'échange de données dynamique est activé.

```csharp
public bool IsDynamicDataExchange { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyIsDynamicDataExchangeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une image à la feuille de calcul
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Démontrer la propriété IsDynamicDataExchange
            Console.WriteLine("Original IsDynamicDataExchange value: " + picture.IsDynamicDataExchange);
            
            // Définir IsDynamicDataExchange sur true
            picture.IsDynamicDataExchange = true;
            Console.WriteLine("After setting IsDynamicDataExchange to true: " + picture.IsDynamicDataExchange);

            // Enregistrez le classeur
            workbook.Save("PicturePropertyIsDynamicDataExchangeDemo.xlsx", SaveFormat.Xlsx);

            // Chargez le classeur enregistré pour vérifier la propriété
            Workbook loadedWorkbook = new Workbook("PicturePropertyIsDynamicDataExchangeDemo.xlsx");
            Picture loadedPicture = loadedWorkbook.Worksheets[0].Pictures[0];
            Console.WriteLine("Loaded IsDynamicDataExchange value: " + loadedPicture.IsDynamicDataExchange);
        }
    }
}
```

### Voir aussi

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


