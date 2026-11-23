---
title: "Picture.BorderWeight"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Picture. Obtient ou définit le poids de la ligne de bordure d'une image en unités de pt"
type: docs
url: /fr/net/aspose.cells.drawing/picture/borderweight/
---
## Picture.BorderWeight property

Obtient ou définit l'épaisseur de la ligne de bordure d'une image en unités de pt.

```csharp
public double BorderWeight { get; set; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyBorderWeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Aspose.Cells.Drawing.Picture pic = worksheet.Pictures[imgIndex];
            
            pic.BorderLineColor = Color.Red;
            pic.BorderWeight = 3;
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### Voir aussi

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


