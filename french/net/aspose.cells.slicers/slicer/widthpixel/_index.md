---
title: "Slicer.WidthPixel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Slicer. Renvoie ou définit la largeur du slicer spécifié en pixels"
type: docs
url: /fr/net/aspose.cells.slicers/slicer/widthpixel/
---
## Slicer.WidthPixel property

Renvoie ou définit la largeur du slicer spécifié, en pixels.

```csharp
[Obsolete("Use Shape.Width property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int WidthPixel { get; set; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Shape.Width. Cette propriété sera supprimée 12 mois après mai 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerPropertyWidthPixelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(150);
            sheet.Cells["B3"].PutValue(200);
            
            int tableIndex = sheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = sheet.ListObjects[tableIndex];
            
            int slicerIndex = sheet.Slicers.Add(table, 0, "A5");
            Slicer slicer = sheet.Slicers[slicerIndex];
            slicer.LeftPixel = 50;
            slicer.TopPixel = 100;
            slicer.WidthPixel = 120;
            
            workbook.Save("SlicerWidthDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


