---
title: "Slicer.StyleType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Slicer-Eigenschaft. Gibt den Typ des integrierten Slicer-Stils an. Der Standardtyp ist SlicerStyleLight1"
type: docs
url: /de/net/aspose.cells.slicers/slicer/styletype/
---
## Slicer.StyleType property

Gibt den Typ des integrierten Slicer-Stils an. Der Standardtyp ist SlicerStyleLight1.

```csharp
public SlicerStyleType StyleType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyStyleTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["B4"].PutValue(20);

            // Erstelle eine Pivot-Tabelle
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Zeilenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // Füge Slicer hinzu
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "A1", "FruitSlicer");
            Slicer slicer = worksheet.Slicers[slicerIndex];

            // Slicer-Eigenschaften einschließlich StyleType festlegen
            slicer.StyleType = SlicerStyleType.SlicerStyleDark2;
            slicer.Caption = "Fruit Selection";
            slicer.NumberOfColumns = 2;
            slicer.Width = 200;
            slicer.Height = 100;

            // Speichere die Arbeitsmappe
            workbook.Save("SlicerStyleTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [SlicerStyleType](../../slicerstyletype/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


