---
title: "Classe ReflectionEffect"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.ReflectionEffect. Questa classe specifica un effetto di riflessione"
type: docs
url: /it/net/aspose.cells.drawing/reflectioneffect/
---
## ReflectionEffect class

Questa classe specifica un effetto di riflessione.

```csharp
public class ReflectionEffect
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Blur](../../aspose.cells.drawing/reflectioneffect/blur/) { get; set; } | Ottiene e imposta il raggio di sfocatura, in unità di punti. |
| [Direction](../../aspose.cells.drawing/reflectioneffect/direction/) { get; set; } | Ottiene e imposta la direzione della rampa del gradiente alfa rispetto alla forma stessa. |
| [Distance](../../aspose.cells.drawing/reflectioneffect/distance/) { get; set; } | Ottiene e imposta la distanza dell'ombra, in unità di punti. |
| [FadeDirection](../../aspose.cells.drawing/reflectioneffect/fadedirection/) { get; set; } | Ottiene e imposta la direzione per spostare la riflessione. |
| [RotWithShape](../../aspose.cells.drawing/reflectioneffect/rotwithshape/) { get; set; } | Ottiene e imposta se la riflessione deve ruotare con la forma. |
| [Size](../../aspose.cells.drawing/reflectioneffect/size/) { get; set; } | Ottiene e imposta la posizione finale (lungo la rampa del gradiente alfa) del valore alfa finale, in unità di percentuale. |
| [Transparency](../../aspose.cells.drawing/reflectioneffect/transparency/) { get; set; } | Ottiene e imposta il grado di trasparenza della riflessione iniziale come valore da 0,0 (opaco) a 1,0 (trasparente). |
| [Type](../../aspose.cells.drawing/reflectioneffect/type/) { get; set; } | Ottiene e imposta l'effetto di riflessione predefinito. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassReflectionEffectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma di esempio
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Imposta le proprietà dell'effetto di riflessione
            ReflectionEffect reflection = shape.Reflection;
            reflection.Size = 90;
            reflection.Blur = 30;
            reflection.Transparency = 0.5;
            reflection.Distance = 10;

            // Visualizza le proprietà della riflessione
            Console.WriteLine("Reflection Size: " + reflection.Size);
            Console.WriteLine("Reflection Blur: " + reflection.Blur);
            Console.WriteLine("Reflection Transparency: " + reflection.Transparency);
            Console.WriteLine("Reflection Distance: " + reflection.Distance);

            // Salva la cartella di lavoro
            workbook.Save("ReflectionEffectDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


