---
title: "GradientStopCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GradientStopCollection. Agregar una parada de degradado"
type: docs
url: /es/net/aspose.cells.drawing/gradientstopcollection/add/
---
## Add(double, CellsColor, int) {#add}

Agregar una parada de degradado.

```csharp
public void Add(double position, CellsColor color, int alpha)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| posición | Double | La posición de la parada, en unidades de porcentaje. |
| color | CellsColor | El color de la parada. |
| alpha | Int32 | El alfa del color. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientStopCollectionMethodAddWithDoubleCellsColorInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 0, 2, 0, 300, 100);
            shape.Fill.FillType = FillType.Gradient;
            
            GradientStopCollection gradientStops = shape.Fill.GradientFill.GradientStops;
            gradientStops.Clear();

            try
            {
                // Crear CellsColor usando el método de fábrica
                CellsColor gradientColor = workbook.CreateCellsColor();
                gradientColor.Color = Color.DarkOrange;

                gradientStops.Add(0.3, gradientColor, 192);

                Console.WriteLine("Gradient stop added successfully");
                workbook.Save("GradientStopAddDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding gradient stop: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [GradientStopCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(double, Color, int) {#add_1}

Agregar una parada de degradado.

```csharp
public void Add(double position, Color color, int alpha)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| posición | Double | La posición de la parada, en unidades de porcentaje. |
| color | Color | El color de la parada. |
| alpha | Int32 | El alfa del color. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientStopCollectionMethodAddWithDoubleColorInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una forma rectangular con relleno degradado
            var shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 0, 2, 0, 300, 100);
            shape.Fill.FillType = FillType.Gradient;
            shape.Fill.GradientFill.GradientStops.Clear();

            GradientStopCollection gradientStops = shape.Fill.GradientFill.GradientStops;

            try
            {
                // Agregar paradas de degradado usando parámetros (Double, Color, Int32)
                gradientStops.Add(0.0, Color.Red, 255);    // Opaque red at start position
                gradientStops.Add(1.0, Color.Blue, 128);    // Semi-transparent blue at end position

                Console.WriteLine("Added gradient stops with positions: 0.0 (Red) and 1.0 (Blue)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding gradient stops: {ex.Message}");
            }

            workbook.Save("GradientStopCollectionAddDemo.xlsx");
        }
    }
}
```

### Ver también

* class [GradientStopCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


