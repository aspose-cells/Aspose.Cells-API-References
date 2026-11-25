---
title: "Classe SlicerCache"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Slicers.SlicerCache. Rappresenta la descrizione sommaria della cache dello slicer"
type: docs
url: /it/net/aspose.cells.slicers/slicercache/
---
## SlicerCache class

Rappresenta la descrizione sommaria della cache dello slicer

```csharp
public class SlicerCache
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CrossFilterType](../../aspose.cells.slicers/slicercache/crossfiltertype/) { get; set; } | (**Obsolete.**) Indica come mostrare gli elementi senza dati dello slicer. |
| [List](../../aspose.cells.slicers/slicercache/list/) { get; } | Indica se lo slicer associato alla cache dello slicer specificata è basato su una fonte dati non OLAP. |
| [Name](../../aspose.cells.slicers/slicercache/name/) { get; } | Restituisce il nome della cache dello slicer. |
| [SlicerCacheItems](../../aspose.cells.slicers/slicercache/slicercacheitems/) { get; } | Restituisce una raccolta SlicerCacheItem che contiene la collezione di tutti gli elementi nella cache dello slicer. Sola lettura |
| [SourceName](../../aspose.cells.slicers/slicercache/sourcename/) { get; } | Restituisce il nome di questa cache dello slicer. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicersClassSlicerCacheDemo
    {
        public static void Run()
        {
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Crea dati di esempio
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";
            cells[5, 0].Value = "grape";
            cells[6, 0].Value = "blueberry";
            cells[7, 0].Value = "kiwi";
            cells[8, 0].Value = "cherry";
            
            cells[0, 1].Value = "year";
            cells[1, 1].Value = 2020;
            cells[2, 1].Value = 2020;
            cells[3, 1].Value = 2020;
            cells[4, 1].Value = 2020;
            cells[5, 1].Value = 2021;
            cells[6, 1].Value = 2021;
            cells[7, 1].Value = 2021;
            cells[8, 1].Value = 2021;
            
            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;
            cells[5, 2].Value = 90;
            cells[6, 2].Value = 100;
            cells[7, 2].Value = 110;
            cells[8, 2].Value = 120;
            
            // Crea tabella pivot
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            pivot.RefreshData();
            pivot.CalculateData();
            
            // Aggiungi lo slicer e ottieni la sua cache
            SlicerCollection slicers = sheet.Slicers;
            int slicerIndex = slicers.Add(pivot, "E12", "fruit");
            Slicer slicer = slicers[slicerIndex];
            slicer.StyleType = SlicerStyleType.SlicerStyleLight2;
            
            // Dimostrare l'utilizzo di SlicerCache
            SlicerCache slicerCache = slicer.SlicerCache;
            Console.WriteLine("Slicer Cache Items:");
            foreach (SlicerCacheItem item in slicerCache.SlicerCacheItems)
            {
                Console.WriteLine(item.Value);
            }
            
            book.Save("out.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)


