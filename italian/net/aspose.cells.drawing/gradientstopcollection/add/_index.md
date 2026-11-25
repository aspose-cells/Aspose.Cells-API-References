---
title: "GradientStopCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GradientStopCollection. Aggiungi una fermata di gradiente"
type: docs
url: /it/net/aspose.cells.drawing/gradientstopcollection/add/
---
## Add(double, CellsColor, int) {#add}

Aggiungi una fermata del gradiente.

```csharp
public void Add(double position, CellsColor color, int alpha)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| posizione | Double | La posizione della fermata, in unità di percentuale. |
| colore | CellsColor | Il colore della fermata. |
| alpha | Int32 | L'alpha del colore. |

### Esempi

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
                // Crea CellsColor usando il metodo factory
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

### Vedi anche

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [GradientStopCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(double, Color, int) {#add_1}

Aggiungi una fermata del gradiente.

```csharp
public void Add(double position, Color color, int alpha)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| posizione | Double | La posizione della fermata, in unità di percentuale. |
| colore | Color | Il colore della fermata. |
| alpha | Int32 | L'alpha del colore. |

### Esempi

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

            // Crea una forma rettangolare con riempimento a gradiente
            var shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 0, 2, 0, 300, 100);
            shape.Fill.FillType = FillType.Gradient;
            shape.Fill.GradientFill.GradientStops.Clear();

            GradientStopCollection gradientStops = shape.Fill.GradientFill.GradientStops;

            try
            {
                // Aggiungi fermate di gradiente usando i parametri (Double, Color, Int32)
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

### Vedi anche

* class [GradientStopCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


