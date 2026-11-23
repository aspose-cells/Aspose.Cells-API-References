---
title: "Picture.OriginalHeightInch"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Picture. Obtient la hauteur originale de l'image en pouces"
type: docs
url: /fr/net/aspose.cells.drawing/picture/originalheightinch/
---
## Picture.OriginalHeightInch property

Obtient la hauteur originale de l'image, en pouces.

```csharp
public double OriginalHeightInch { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyOriginalHeightInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Picture pic = worksheet.Pictures[imgIndex];
            
            Console.WriteLine("Original picture height in inches: " + pic.OriginalHeightInch);
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### Voir aussi

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


