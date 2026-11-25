---
title: "Slicer.Shape"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Slicer. Restituisce l'oggetto Shape associato allo slicer specificato. Solo lettura"
type: docs
url: /it/net/aspose.cells.slicers/slicer/shape/
---
## Slicer.Shape property

Restituisce l'oggetto Shape associato allo slicer specificato. Sola lettura.

```csharp
public SlicerShape Shape { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Crea una tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Aggiungi uno slicer
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "Fruit", "FruitSlicer");
            Slicer slicer = worksheet.Slicers[slicerIndex];

            try
            {
                // Accedi alla proprietà Shape (sola lettura)
                var slicerShape = slicer.Shape;

                // Visualizza le informazioni sullo Shape
                Console.WriteLine("Slicer Shape Type: " + slicerShape.GetType().Name);
                Console.WriteLine("Slicer Shape Name: " + slicerShape.Name);
                Console.WriteLine("Slicer Shape Width: " + slicerShape.Width);
                Console.WriteLine("Slicer Shape Height: " + slicerShape.Height);

                // Salva la cartella di lavoro
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

### Vedi anche

* class [SlicerShape](../../../aspose.cells.drawing/slicershape/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


