---
title: "SlicerCollection.Remove"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SlicerCollection yöntemi. Belirtilen Slicer'ı kaldır"
type: docs
url: /tr/net/aspose.cells.slicers/slicercollection/remove/
---
## SlicerCollection.Remove method

Belirtilen Slicer'ı kaldır

```csharp
public void Remove(Slicer slicer)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| slicer | Slicer | Slicer nesnesi |

### Örnekler

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

### Ayrıca Bakınız

* class [Slicer](../../slicer/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


