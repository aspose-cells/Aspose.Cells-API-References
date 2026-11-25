---
title: "Classe ShapePath"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.ShapePath. Rappresenta un percorso di creazione costituito da una serie di spostamenti, linee e curve che, combinati, formeranno una forma geometrica"
type: docs
url: /it/net/aspose.cells.drawing/shapepath/
---
## ShapePath class

Rappresenta un percorso di creazione costituito da una serie di spostamenti, linee e curve che, combinati, formeranno una forma geometrica.

```csharp
public class ShapePath
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ShapePath](shapepath/)() | Inizializza una nuova istanza della classe `ShapePath`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [HeightPixel](../../aspose.cells.drawing/shapepath/heightpixel/) { get; set; } | Restituisce l'altezza di questo percorso in unità di pixel. |
| [PathSegementList](../../aspose.cells.drawing/shapepath/pathsegementlist/) { get; } | (**Obsoleto.**) Restituisce l'elenco [`ShapeSegmentPathCollection`](../shapesegmentpathcollection/) |
| [PathSegments](../../aspose.cells.drawing/shapepath/pathsegments/) { get; } | Restituisce l'elenco [`ShapeSegmentPathCollection`](../shapesegmentpathcollection/) |
| [WidthPixel](../../aspose.cells.drawing/shapepath/widthpixel/) { get; set; } | Restituisce la larghezza di questo percorso in unità di pixel. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [ArcTo](../../aspose.cells.drawing/shapepath/arcto/)(float, float, float, float) | Aggiunge un arco ellittico alla figura corrente. Il punto di partenza è il punto finale della figura corrente. |
| [Close](../../aspose.cells.drawing/shapepath/close/)() | Chiude la figura corrente e avvia una nuova figura. Se la figura corrente contiene una sequenza di linee e curve collegate, il metodo chiude il ciclo collegando una linea dal punto finale al punto di partenza. |
| [CubicBezierTo](../../aspose.cells.drawing/shapepath/cubicbezierto/)(float, float, float, float, float, float) | Aggiunge una curva Bézier cubica alla figura corrente. Il punto di partenza è il punto finale della figura corrente. Unità: Pixel. |
| [LineTo](../../aspose.cells.drawing/shapepath/lineto/)(float, float) | Aggiunge un segmento di linea alla figura corrente. Il punto di partenza è il punto finale della figura corrente. Unità: Pixel. |
| [MoveTo](../../aspose.cells.drawing/shapepath/moveto/)(float, float) | Avvia una nuova figura dal punto specificato senza chiudere la figura corrente. Tutti i punti successivi aggiunti al percorso vengono aggiati a questa nuova figura. Unità: Pixel. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShapePathDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma personalizzata con tutti i parametri richiesti
            Shape customShape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 10, 10, 200, 100, 0, 0);
            
            // Accedi alla ShapePathCollection
            ShapePathCollection shapePaths = customShape.Paths;

            // Aggiungi un nuovo percorso e accedilo
            int pathIndex = shapePaths.Add();
            ShapePath newPath = shapePaths[pathIndex];

            // Visualizza il numero di percorsi
            Console.WriteLine("Number of paths in the ShapePathCollection: " + shapePaths.Count.ToString());

            // Salva la cartella di lavoro
            workbook.Save("ShapePathDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


