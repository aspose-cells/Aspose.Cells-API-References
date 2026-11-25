---
title: "Slicer.AlternativeText"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Slicer. Restituisce o imposta la stringa di testo alternativo descrittivo dell'oggetto Slicer"
type: docs
url: /it/net/aspose.cells.slicers/slicer/alternativetext/
---
## Slicer.AlternativeText property

Restituisce o imposta la stringa di testo descrittivo (alternativo) dell'oggetto Slicer.

```csharp
[Obsolete("Use Shape.AlternativeText property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string AlternativeText { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, utilizza la proprietà [`AlternativeText`](../../../aspose.cells.drawing/shape/alternativetext/). Questa proprietà sarà rimossa 12 mesi dopo, a partire da gennaio 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class SlicerPropertyAlternativeTextDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            
            ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add("A1:A3", "", true)];
            table.DisplayName = "Table1";

            int slicerIndex = worksheet.Slicers.Add(table, 0, "C1");
            Slicer slicer = worksheet.Slicers[slicerIndex];
            slicer.AlternativeText = "AlternativeText test";

            workbook.Save("SlicerAlternativeTextDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


