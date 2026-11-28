---
title: "Slicer.RemovePivotConnection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Slicer yöntemi. PivotTable bağlantısını kaldırır"
type: docs
url: /tr/net/aspose.cells.slicers/slicer/removepivotconnection/
---
## Slicer.RemovePivotConnection method

PivotTable bağlantısını kaldırır.

```csharp
public void RemovePivotConnection(PivotTable pivot)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivot | PivotTable | PivotTable nesnesi |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerMethodRemovePivotConnectionWithPivotTableDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            
            dataSheet.Cells["A1"].PutValue("Product");
            dataSheet.Cells["A2"].PutValue("Apple");
            dataSheet.Cells["A3"].PutValue("Banana");
            dataSheet.Cells["B1"].PutValue("Sales");
            dataSheet.Cells["B2"].PutValue(100);
            dataSheet.Cells["B3"].PutValue(200);

            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            int index = pivotTables.Add("=Data!A1:B3", "A3", "TestPivotTable");
            PivotTable pivotTable = pivotTables[index];
            
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            int slicerIndex = pivotSheet.Slicers.Add(pivotTable, "E3", 0);
            Slicer slicer = pivotSheet.Slicers[slicerIndex];
            slicer.RemovePivotConnection(pivotTable);

            workbook.Save("SlicerRemovePivotConnection_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


