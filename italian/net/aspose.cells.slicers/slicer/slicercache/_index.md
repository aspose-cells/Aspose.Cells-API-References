---
title: "Slicer.SlicerCache"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Slicer. Restituisce l'oggetto SlicerCache associato allo slicer. Sola lettura"
type: docs
url: /it/net/aspose.cells.slicers/slicer/slicercache/
---
## Slicer.SlicerCache property

Restituisce l'oggetto SlicerCache associato allo slicer. Sola lettura.

```csharp
public SlicerCache SlicerCache { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["B4"].PutValue(20);

            // Crea una tabella dall'intervallo di dati
            int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];

            // Aggiungi una tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Aggiungi uno slicer
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "Fruit", "Slicer1");
            Slicer slicer = worksheet.Slicers[slicerIndex];

            // Dimostrare l'utilizzo di SlicerCache
            SlicerCache slicerCache = slicer.SlicerCache;
            Console.WriteLine("Slicer Cache Name: " + slicerCache.Name);
            Console.WriteLine("Slicer Cache Source Name: " + slicerCache.SourceName);
            Console.WriteLine("Slicer Cache Items Count: " + slicerCache.SlicerCacheItems.Count);

            // Salva la cartella di lavoro
            workbook.Save("SlicerCacheDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SlicerCache](../../slicercache/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


