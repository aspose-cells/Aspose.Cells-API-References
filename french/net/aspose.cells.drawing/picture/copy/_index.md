---
title: "Picture.Copy"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Picture. Copie l'image"
type: docs
url: /fr/net/aspose.cells.drawing/picture/copy/
---
## Picture.Copy method

Copier l'image.

```csharp
public void Copy(Picture source, CopyOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| source | Image | L'image source. |
| options | CopyOptions | Les options de copie. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureMethodCopyWithPictureCopyOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Insérer la première image (en utilisant un chemin d'image d'exemple)
            int imgIndex1 = worksheet.Pictures.Add(1, 1, "sample1.png");
            Picture pic1 = worksheet.Pictures[imgIndex1];
            
            // Insérer une deuxième image (en utilisant un chemin d'image d'exemple)
            int imgIndex2 = worksheet.Pictures.Add(1, 9, "sample2.jpg");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            
            // Copier l'image 1 vers l'image 2 avec CopyOptions
            CopyOptions options = new CopyOptions();
            pic2.Copy(pic1, options);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [CopyOptions](../../../aspose.cells/copyoptions/)
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


