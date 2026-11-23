---
title: "Picture.BorderLineColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Picture. Représente la couleur de la ligne de bordure d'une image"
type: docs
url: /fr/net/aspose.cells.drawing/picture/borderlinecolor/
---
## Picture.BorderLineColor property

Représente la couleur de la ligne de bordure d'une image.

```csharp
public Color BorderLineColor { get; set; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyBorderLineColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Picture pic = worksheet.Pictures[imgIndex];
            
            pic.BorderLineColor = Color.Red;
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### Voir aussi

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


