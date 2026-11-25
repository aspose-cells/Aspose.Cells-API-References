---
title: "ThreeDFormat.TopBevelWidth"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ThreeDFormat. Ottiene e imposta la larghezza del contorno superiore o quanto profondamente viene applicata alla forma. In unità di punti"
type: docs
url: /it/net/aspose.cells.drawing/threedformat/topbevelwidth/
---
## ThreeDFormat.TopBevelWidth property

Ottiene e imposta la larghezza del bordo superiore, o quanto profondamente viene applicato nella forma. In unità di punti.

```csharp
public double TopBevelWidth { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ThreeDFormatPropertyTopBevelWidthDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma al foglio di lavoro con i parametri corretti.
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 200, 200, 0, 0);

            // Ottieni il formato 3D della forma
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Imposta le proprietà 3D includendo TopBevelWidth
            threeDFormat.TopBevelType = BevelType.HardEdge;
            threeDFormat.TopBevelWidth = 30;
            threeDFormat.TopBevelHeight = 30;
            threeDFormat.ContourWidth = 17;
            threeDFormat.ExtrusionHeight = 32;

            // Salva la cartella di lavoro
            workbook.Save("ThreeDFormatDemo.xlsx");

            // Verifica le proprietà salvate
            Workbook loadedWorkbook = new Workbook("ThreeDFormatDemo.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            ThreeDFormat loadedFormat = loadedShape.ThreeDFormat;

            Console.WriteLine("TopBevelWidth: " + loadedFormat.TopBevelWidth);
            Console.WriteLine("TopBevelHeight: " + loadedFormat.TopBevelHeight);
            Console.WriteLine("TopBevelType: " + loadedFormat.TopBevelType);
            Console.WriteLine("ContourWidth: " + loadedFormat.ContourWidth);
            Console.WriteLine("ExtrusionHeight: " + loadedFormat.ExtrusionHeight);
        }
    }
}
```

### Vedi anche

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


