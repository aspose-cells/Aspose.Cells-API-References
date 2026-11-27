---
title: "SlicerCache.CrossFilterType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SlicerCache-egenskap. Anger hur objekt utan data för slicern ska visas"
type: docs
url: /sv/net/aspose.cells.slicers/slicercache/crossfiltertype/
---
## SlicerCache.CrossFilterType property

Anger hur objekt utan data för slicern ska visas.

```csharp
[Obsolete("Use Slicer.ShowTypeOfItemsWithNoData property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public SlicerCacheCrossFilterType CrossFilterType { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen [`ShowTypeOfItemsWithNoData`](../../slicer/showtypeofitemswithnodata/). Denna egenskap kommer att tas bort 12 månader senare från och med januari 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

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

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Lägg till skärmningskontrollen
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "A1", "Category");
            Slicer slicer = worksheet.Slicers[slicerIndex];

            // Ställ in och demonstrera CrossFilterType
            slicer.SlicerCache.CrossFilterType = SlicerCacheCrossFilterType.ShowItemsWithDataAtTop;
            Console.WriteLine("Slicer CrossFilterType: " + slicer.SlicerCache.CrossFilterType);

            workbook.Save("SlicerCacheCrossFilterTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [SlicerCacheCrossFilterType](../../slicercachecrossfiltertype/)
* class [SlicerCache](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


