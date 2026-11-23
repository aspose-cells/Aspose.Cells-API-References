---
title: "Slicer.SlicerCache"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Slicer. Retourne l’objet SlicerCache associé au slicer. Lecture seule"
type: docs
url: /fr/net/aspose.cells.slicers/slicer/slicercache/
---
## Slicer.SlicerCache property

Renvoie l'objet SlicerCache associé au segmenteur. Lecture seule.

```csharp
public SlicerCache SlicerCache { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerPropertySlicerCacheDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["B4"].PutValue(20);

            // Créer un tableau à partir de la plage de données
            int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];

            // Ajouter un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Ajouter un segmenteur
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "Fruit", "Slicer1");
            Slicer slicer = worksheet.Slicers[slicerIndex];

            // Démontrer l'utilisation de SlicerCache
            SlicerCache slicerCache = slicer.SlicerCache;
            Console.WriteLine("Slicer Cache Name: " + slicerCache.Name);
            Console.WriteLine("Slicer Cache Source Name: " + slicerCache.SourceName);
            Console.WriteLine("Slicer Cache Items Count: " + slicerCache.SlicerCacheItems.Count);

            // Enregistrez le classeur
            workbook.Save("SlicerCacheDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SlicerCache](../../slicercache/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


