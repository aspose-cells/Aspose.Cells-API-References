---
title: "SlicerCollection.Remove"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SlicerCollection. Supprimer le segment spécifié"
type: docs
url: /fr/net/aspose.cells.slicers/slicercollection/remove/
---
## SlicerCollection.Remove method

Supprimer le Slicer spécifié

```csharp
public void Remove(Slicer slicer)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| segment | Segmentateur | L'objet Slicer |

### Exemples

```csharp
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodRemoveWithSlicerDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["A3"].PutValue("Item2");
            
            ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add("A1", "A3", true)];
            
            SlicerCollection slicers = worksheet.Slicers;
            slicers.Add(table, 0, "C1");
            slicers.Add(table, 0, "C5");
            
            Slicer delSlicer = slicers[0];
            slicers.Remove(delSlicer);
        }
    }
}
```

### Voir aussi

* class [Slicer](../../slicer/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


