---
title: "Slicer.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Slicer-Eigenschaft. Gibt den Namen des angegebenen Slicers zurück oder legt ihn fest."
type: docs
url: /de/net/aspose.cells.slicers/slicer/name/
---
## Slicer.Name property

Gibt den Namen des angegebenen Slicers zurück oder legt ihn fest

```csharp
public string Name { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerPropertyNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Vegetable");
            
            int tableIndex = worksheet.ListObjects.Add("A1", "A3", true);
            ListObject table = worksheet.ListObjects[tableIndex];

            int slicerIndex = worksheet.Slicers.Add(table, 0, "B1");
            Slicer slicer = worksheet.Slicers[slicerIndex];
            slicer.Name = "slicer name";

            workbook.Save("SlicerPropertyNameDemoOutput.xlsx");
        }
    }
}
```

### Siehe auch

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


