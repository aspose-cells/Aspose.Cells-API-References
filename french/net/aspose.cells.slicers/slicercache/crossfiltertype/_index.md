---
title: "SlicerCache.CrossFilterType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SlicerCache. Indique comment afficher les éléments sans données du segment"
type: docs
url: /fr/net/aspose.cells.slicers/slicercache/crossfiltertype/
---
## SlicerCache.CrossFilterType property

Indique comment afficher les éléments sans données du segment.

```csharp
[Obsolete("Use Slicer.ShowTypeOfItemsWithNoData property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public SlicerCacheCrossFilterType CrossFilterType { get; set; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété [`ShowTypeOfItemsWithNoData`](../../slicer/showtypeofitemswithnodata/). Cette propriété sera supprimée 12 mois plus tard, à compter de janvier 2026. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCachePropertyCrossFilterTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Ajouter un slicer
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "A1", "Category");
            Slicer slicer = worksheet.Slicers[slicerIndex];

            // Définir et démontrer CrossFilterType
            slicer.SlicerCache.CrossFilterType = SlicerCacheCrossFilterType.ShowItemsWithDataAtTop;
            Console.WriteLine("Slicer CrossFilterType: " + slicer.SlicerCache.CrossFilterType);

            workbook.Save("SlicerCacheCrossFilterTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [SlicerCacheCrossFilterType](../../slicercachecrossfiltertype/)
* class [SlicerCache](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


