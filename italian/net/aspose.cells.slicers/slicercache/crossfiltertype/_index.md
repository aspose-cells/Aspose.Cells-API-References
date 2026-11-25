---
title: "SlicerCache.CrossFilterType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SlicerCache. Indica come mostrare gli elementi senza dati dello slicer"
type: docs
url: /it/net/aspose.cells.slicers/slicercache/crossfiltertype/
---
## SlicerCache.CrossFilterType property

Indica come mostrare gli elementi senza dati dello slicer.

```csharp
[Obsolete("Use Slicer.ShowTypeOfItemsWithNoData property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public SlicerCacheCrossFilterType CrossFilterType { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà [`ShowTypeOfItemsWithNoData`](../../slicer/showtypeofitemswithnodata/). Questa proprietà sarà rimossa tra 12 mesi a partire da gennaio 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

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

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Aggiungi slicer
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "A1", "Category");
            Slicer slicer = worksheet.Slicers[slicerIndex];

            // Imposta e dimostra CrossFilterType
            slicer.SlicerCache.CrossFilterType = SlicerCacheCrossFilterType.ShowItemsWithDataAtTop;
            Console.WriteLine("Slicer CrossFilterType: " + slicer.SlicerCache.CrossFilterType);

            workbook.Save("SlicerCacheCrossFilterTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [SlicerCacheCrossFilterType](../../slicercachecrossfiltertype/)
* class [SlicerCache](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


