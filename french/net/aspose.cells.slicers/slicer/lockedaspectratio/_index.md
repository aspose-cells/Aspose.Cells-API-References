---
title: "Slicer.LockedAspectRatio"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Slicer. Indique si le verrouillage du ratio d'aspect est activé"
type: docs
url: /fr/net/aspose.cells.slicers/slicer/lockedaspectratio/
---
## Slicer.LockedAspectRatio property

Indique si le verrouillage du ratio d'aspect est activé.

```csharp
[Obsolete("Use Shape.IsLockAspectRatio property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool LockedAspectRatio { get; set; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode [`IsAspectRatioLocked`](../../../aspose.cells.drawing/shape/isaspectratiolocked/). Cette propriété sera supprimée 12 mois plus tard, à compter de janvier 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class SlicerPropertyLockedAspectRatioDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(30);

            int tableIndex = worksheet.ListObjects.Add("A1", "B3", true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.DisplayName = "GroceryTable";

            int slicerIndex = worksheet.Slicers.Add(table, 0, "A5");
            Aspose.Cells.Slicers.Slicer slicer = worksheet.Slicers[slicerIndex];
            slicer.LockedAspectRatio = true;

            workbook.Save("SlicerLockedAspectRatioDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


