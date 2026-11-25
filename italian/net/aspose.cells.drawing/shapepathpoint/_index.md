---
title: "Classe ShapePathPoint"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.ShapePathPoint. Specifica le coordinate di posizione o i marcatori di angolo. Le coordinate di posizione rappresentano le coordinate di un percorso in uno spazio di coordinate, ad es. X/Y. I marcatori di angolo indicano le variazioni angolari in un percorso, ad es. gli angoli di inizio e di swing di un arco."
type: docs
url: /it/net/aspose.cells.drawing/shapepathpoint/
---
## ShapePathPoint class

Specifica coordinate di posizione o marcatori di angolo. Le coordinate di posizione rappresentano le coordinate di un percorso in uno spazio di coordinate (ad es. X/Y). I marcatori di angolo indicano variazioni angolari in un percorso (ad es. gli angoli di inizio e di swing di un arco).

```csharp
public class ShapePathPoint
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Type](../../aspose.cells.drawing/shapepathpoint/type/) { get; } | Specifica il tipo di valore dell'oggetto corrente. |
| [X](../../aspose.cells.drawing/shapepathpoint/x/) { get; set; } | (**Obsolete.**) Ottiene e imposta la coordinata x per questa coordinata di posizione. Unità EMU. |
| [XAngle](../../aspose.cells.drawing/shapepathpoint/xangle/) { get; set; } | Quando l'oggetto è un marcatore di angolo, ottieni o imposta il primo angolo in gradi. |
| [XPixel](../../aspose.cells.drawing/shapepathpoint/xpixel/) { get; set; } | Quando l'oggetto è una coordinata di posizione, ottieni o imposta la coordinata x in pixel. |
| [Y](../../aspose.cells.drawing/shapepathpoint/y/) { get; set; } | (**Obsolete.**) Ottiene la coordinata y per questa coordinata di posizione. Unità EMU. |
| [YAngle](../../aspose.cells.drawing/shapepathpoint/yangle/) { get; set; } | Quando l'oggetto è un marcatore di angolo, ottieni o imposta il secondo angolo in gradi. |
| [YPixel](../../aspose.cells.drawing/shapepathpoint/ypixel/) { get; set; } | Quando l'oggetto è una coordinata di posizione, ottieni o imposta la coordinata y in pixel. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapePathPointDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Aggiungi una forma che conterrà i punti del percorso con tutti i parametri richiesti
                Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 10, 10, 200, 200);
                
                // Ottieni i punti del percorso geometrico
                CustomGeometry geometry = shape.Geometry as CustomGeometry;
                if (geometry != null && geometry.Paths.Count > 0)
                {
                    ShapePath path = geometry.Paths[0];
                    
                    // Accedi a un punto del percorso esistente (se disponibile)
                    if (path.PathSegementList.Count > 0)
                    {
                        // Ottieni il primo punto (l'implementazione reale può variare in base al tipo di segmento)
                        ShapePathPoint point = path.PathSegementList[0].Points[0];
                        
                        // Visualizza le coordinate del punto
                        Console.WriteLine($"ShapePathPoint at X: {point.X}, Y: {point.Y}");
                    }
                }
                
                // Salva la cartella di lavoro
                workbook.Save("ShapePathPointDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ShapePathPoint: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


