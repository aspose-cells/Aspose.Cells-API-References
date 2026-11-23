---
title: "Shape.FormatPicture"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient et définit les options du format d'image"
type: docs
url: /fr/net/aspose.cells.drawing/shape/formatpicture/
---
## Shape.FormatPicture property

Obtient et définit les options du format d'image.

```csharp
public MsoFormatPicture FormatPicture { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyFormatPictureDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une image à la feuille de calcul
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[index];
            
            // Accéder à la propriété FormatPicture de la forme
            MsoFormatPicture msoFormatPicture = picture.FormatPicture;
            
            // Modifier les propriétés du format d'image
            msoFormatPicture.Brightness = 0.5f;
            msoFormatPicture.Contrast = 0.7f;
            msoFormatPicture.Transparency = 0.3f;
            
            // Enregistrez le classeur
            workbook.Save("ShapePropertyFormatPictureDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [MsoFormatPicture](../../msoformatpicture/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


