---
title: "Picture.IsSameSetting"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Picture. Retourne si la forme est identique"
type: docs
url: /fr/net/aspose.cells.drawing/picture/issamesetting/
---
## Picture.IsSameSetting method

Renvoie si la forme est identique.

```csharp
public override bool IsSameSetting(object obj)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| obj | Object |  |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureMethodIsSameSettingWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Insérer la première image (en utilisant un chemin d'image d'exemple)
            int imgIndex1 = worksheet.Pictures.Add(1, 1, "sample1.png");
            Picture pic1 = worksheet.Pictures[imgIndex1];
            
            // Insérer la deuxième image (en utilisant un chemin d'image d'exemple différent)
            int imgIndex2 = worksheet.Pictures.Add(1, 9, "sample2.jpg");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            
            // Comparer l'image avec elle-même
            if (pic1.IsSameSetting(pic1))
            {
                Console.WriteLine("pic1 and pic1 are the same");
            }
            
            // Comparer différentes images
            if (!pic1.IsSameSetting(pic2))
            {
                Console.WriteLine("pic1 and pic2 are different");
            }
        }
    }
}
```

### Voir aussi

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


