---
title: "Enum ShapePathType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.ShapePathType enum. Rappresenta il tipo di segmento di percorso"
type: docs
url: /it/net/aspose.cells.drawing/shapepathtype/
---
## ShapePathType enumeration

Rappresenta il tipo di segmento di percorso.

```csharp
public enum ShapePathType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| LineTo | `1` | Segmento di linea retta |
| CubicBezierCurveTo | `3` | Curva Bézier cubica |
| MoveTo | `0` | Inizia un nuovo percorso |
| Close | `128` | Se il POINT di partenza e il POINT finale non sono gli stessi, viene disegnata una singola linea retta per collegare il POINT di partenza e il POINT finale del percorso. |
| End | `4` | La fine del percorso corrente |
| Escape | `5` | Esc |
| ArcTo | `6` | Un arco |
| Unknown | `7` | Sconosciuto |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapePathTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crea una forma per dimostrare i tipi di percorso
                Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 10, 10, 10, 10, 200, 200);

                // Crea un percorso di geometria personalizzato
                Geometry geometry = shape.Geometry;
                ShapePath path = new ShapePath();

                // Dimostra i diversi valori di ShapePathType
                Console.WriteLine("Available ShapePathType values:");
                Console.WriteLine($"LineTo: {ShapePathType.LineTo}");
                Console.WriteLine($"CubicBezierCurveTo: {ShapePathType.CubicBezierCurveTo}");
                Console.WriteLine($"MoveTo: {ShapePathType.MoveTo}");
                Console.WriteLine($"Close: {ShapePathType.Close}");
                Console.WriteLine($"End: {ShapePathType.End}");

                // Applica alcune operazioni di percorso
                path.MoveTo(10, 10);
                path.LineTo(100, 100);
                path.Close();

                // Salva la cartella di lavoro
                workbook.Save("ShapePathTypeDemo.xlsx");
                Console.WriteLine("Demo completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ShapePathType: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


