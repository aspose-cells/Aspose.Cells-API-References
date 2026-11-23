---
title: "Picture.OriginalHeightCM"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Picture. Obtient la hauteur originale de l'image en centimètres"
type: docs
url: /fr/net/aspose.cells.drawing/picture/originalheightcm/
---
## Picture.OriginalHeightCM property

Obtient la hauteur originale de l'image, en centimètres.

```csharp
public double OriginalHeightCM { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyOriginalHeightCMDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Picture pic = worksheet.Pictures[imgIndex];
            
            Console.WriteLine("Original height of the picture (cm): " + pic.OriginalHeightCM);
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### Voir aussi

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


