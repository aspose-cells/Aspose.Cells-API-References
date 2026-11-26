---
title: "Slicer.Shape"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Slicer. Devuelve el objeto Shape asociado con el slicer especificado. Solo lectura"
type: docs
url: /es/net/aspose.cells.slicers/slicer/shape/
---
## Slicer.Shape property

Devuelve el objeto Shape asociado al segmentador especificado. Solo lectura.

```csharp
public SlicerShape Shape { get; }
```

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Crear una tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Agregar un segmentador
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "Fruit", "FruitSlicer");
            Slicer slicer = worksheet.Slicers[slicerIndex];

            try
            {
                // Acceda a la propiedad Shape (solo lectura)
                var slicerShape = slicer.Shape;

                // Muestra información sobre el Shape
                Console.WriteLine("Slicer Shape Type: " + slicerShape.GetType().Name);
                Console.WriteLine("Slicer Shape Name: " + slicerShape.Name);
                Console.WriteLine("Slicer Shape Width: " + slicerShape.Width);
                Console.WriteLine("Slicer Shape Height: " + slicerShape.Height);

                // Guarda el libro de trabajo
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

### Ver también

* class [SlicerShape](../../../aspose.cells.drawing/slicershape/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


