---
title: "ReflectionEffect.Distance"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ReflectionEffect property. Ottiene e imposta la distanza dell'ombra in unità di punti"
type: docs
url: /it/net/aspose.cells.drawing/reflectioneffect/distance/
---
## ReflectionEffect.Distance property

Ottiene e imposta la distanza dell'ombra, in unità di punti.

```csharp
public double Distance { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ReflectionEffectPropertyDistanceDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma per testare la riflessione - parametri fissi per corrispondere alla firma del metodo
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Imposta le proprietà di riflessione
            ReflectionEffect reflection = shape.Reflection;
            reflection.Type = ReflectionEffectType.HalfReflection4PtOffset;
            reflection.Transparency = 0.5;
            reflection.Size = 55.5;
            reflection.Blur = 0.5;
            reflection.Distance = 4; // Demonstrating Distance property

            // Salva e ricarica per verificare la persistenza
            string outputPath = "ReflectionEffectDemo.xlsx";
            workbook.Save(outputPath);

            // Ricarica per verificare
            Workbook loadedWorkbook = new Workbook(outputPath);
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            ReflectionEffect loadedReflection = loadedShape.Reflection;

            Console.WriteLine("Original Distance: " + reflection.Distance);
            Console.WriteLine("Loaded Distance: " + loadedReflection.Distance);
        }
    }
}
```

### Vedi anche

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


