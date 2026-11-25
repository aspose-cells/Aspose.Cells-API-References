---
title: "Classe CustomGeometry"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.CustomGeometry. Rappresenta una forma geometrica personalizzata"
type: docs
url: /it/net/aspose.cells.drawing/customgeometry/
---
## CustomGeometry class

Rappresenta una forma geometrica personalizzata.

```csharp
public class CustomGeometry : Geometry
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Paths](../../aspose.cells.drawing/customgeometry/paths/) { get; } | Ottiene le informazioni della raccolta percorsi quando la forma è un autoshape NotPrimitive |
| [ShapeAdjustValues](../../aspose.cells.drawing/geometry/shapeadjustvalues/) { get; } | Ottiene una raccolta di valori di regolazione della forma (Ereditato da [`Geometry`](../geometry/).) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassCustomGeometryDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un autoshape NotPrimitive con i parametri corretti
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.NotPrimitive, 0, 0, 0, 0, 200, 300);

            // Ottieni l'istanza CustomGeometry dalla forma
            CustomGeometry customGeometry = shape.Geometry as CustomGeometry;

            // Crea un nuovo percorso nella raccolta percorsi della geometria
            int pathIndex = customGeometry.Paths.Add();
            ShapePath path = customGeometry.Paths[pathIndex];

            // Aggiungi segmenti di percorso usando chiamate dirette ai metodi
            path.MoveTo(0, 0);
            path.LineTo(1000, 0);
            path.LineTo(1000, 1000);
            path.LineTo(0, 1000);
            path.Close();

            // Salva la cartella di lavoro
            workbook.Save("CustomGeometryDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Geometry](../geometry/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


