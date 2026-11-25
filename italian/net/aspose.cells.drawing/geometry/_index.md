---
title: "Classe Geometry"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.Geometry. Rappresenta una forma geometrica"
type: docs
url: /it/net/aspose.cells.drawing/geometry/
---
## Geometry class

Rappresenta una forma geometrica.

```csharp
public abstract class Geometry
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ShapeAdjustValues](../../aspose.cells.drawing/geometry/shapeadjustvalues/) { get; } | Ottiene una collezione di valori di regolazione della forma |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    
    public class DrawingClassGeometryDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare al foglio di lavoro
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);

            // Accedi alla geometria della forma
            Geometry geometry = rectangle.Geometry;

            // Aggiungi guide di regolazione della forma direttamente alla collezione
            geometry.ShapeAdjustValues.Add("Roundness", 0.3);
            geometry.ShapeAdjustValues.Add("Angle", 45.0);

            // Salva la cartella di lavoro modificata
            workbook.Save("GeometryDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


