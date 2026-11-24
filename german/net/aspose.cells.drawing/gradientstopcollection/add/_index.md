---
title: "GradientStopCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GradientStopCollection‑Methode. Einen Gradient‑Stopp hinzufügen"
type: docs
url: /de/net/aspose.cells.drawing/gradientstopcollection/add/
---
## Add(double, CellsColor, int) {#add}

Fügen Sie einen Gradient-Stop hinzu.

```csharp
public void Add(double position, CellsColor color, int alpha)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Position | Double | Die Position des Stops in Prozent. |
| Farbe | CellsColor | Die Farbe des Stops. |
| Alpha | Int32 | Der Alpha‑Wert der Farbe. |

### Beispiele

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
                // CellsColor mit Fabrikmethode erstellen
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

### Siehe auch

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [GradientStopCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(double, Color, int) {#add_1}

Fügen Sie einen Gradient-Stop hinzu.

```csharp
public void Add(double position, Color color, int alpha)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Position | Double | Die Position des Stops in Prozent. |
| Farbe | Farbe | Die Farbe des Stops. |
| Alpha | Int32 | Der Alpha‑Wert der Farbe. |

### Beispiele

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

            // Erstellen Sie eine Rechteckform mit Farbverlauffüllung
            var shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 0, 2, 0, 300, 100);
            shape.Fill.FillType = FillType.Gradient;
            shape.Fill.GradientFill.GradientStops.Clear();

            GradientStopCollection gradientStops = shape.Fill.GradientFill.GradientStops;

            try
            {
                // Gradient‑Stops mit den Parametern (Double, Color, Int32) hinzufügen
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

### Siehe auch

* class [GradientStopCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


