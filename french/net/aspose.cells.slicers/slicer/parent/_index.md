---
title: "Slicer.Parent"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Slicer. Retourne l’objet Worksheet qui contient ce segment. Lecture seule"
type: docs
url: /fr/net/aspose.cells.slicers/slicer/parent/
---
## Slicer.Parent property

Retourne l’objet [`Worksheet`](../worksheet/) qui contient ce segment. Lecture seule.

```csharp
[Obsolete("Use Slicer.Worksheet property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Worksheet Parent { get; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété [`Worksheet`](../worksheet/). Cette propriété sera supprimée 12 mois plus tard, à compter de janvier 2026. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerPropertyParentDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["A4"].Value = "Banana";

            int tableIndex = sheet.ListObjects.Add("A1", "A4", true);
            ListObject table = sheet.ListObjects[tableIndex];

            int slicerIndex = sheet.Slicers.Add(table, 0, "B1");
            Slicer slicer = sheet.Slicers[slicerIndex];
            Worksheet currSheet = slicer.Parent;

            currSheet.Cells["C1"].Value = "ParentWorksheetAccessed";
            workbook.Save("SlicerParentDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


