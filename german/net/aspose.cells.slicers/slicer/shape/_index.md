---
title: "Slicer.Shape"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Slicer-Eigenschaft. Gibt das mit dem angegebenen Slicer verbundene Shape-Objekt zurück. Nur lesbar"
type: docs
url: /de/net/aspose.cells.slicers/slicer/shape/
---
## Slicer.Shape property

Gibt das Shape‑Objekt zurück, das dem angegebenen Slicer zugeordnet ist. Nur lesbar.

```csharp
public SlicerShape Shape { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Slicers;
    using Aspose.Cells.Pivot;
    using System;

    public class SlicerPropertyShapeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Erstelle eine Pivot-Tabelle
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Einen Slicer hinzufügen
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "Fruit", "FruitSlicer");
            Slicer slicer = worksheet.Slicers[slicerIndex];

            try
            {
                // Zugriff auf die Shape-Eigenschaft (nur lesbar)
                var slicerShape = slicer.Shape;

                // Informationen über das Shape anzeigen
                Console.WriteLine("Slicer Shape Type: " + slicerShape.GetType().Name);
                Console.WriteLine("Slicer Shape Name: " + slicerShape.Name);
                Console.WriteLine("Slicer Shape Width: " + slicerShape.Width);
                Console.WriteLine("Slicer Shape Height: " + slicerShape.Height);

                // Speichere die Arbeitsmappe
                workbook.Save("SlicerShapeDemo.xlsx");
                Console.WriteLine("Slicer Shape has been demonstrated and saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [SlicerShape](../../../aspose.cells.drawing/slicershape/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


