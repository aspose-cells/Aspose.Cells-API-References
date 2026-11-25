---
title: "ReflectionEffect.FadeDirection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ReflectionEffect. Restituisce e imposta la direzione per spostare la riflessione"
type: docs
url: /it/net/aspose.cells.drawing/reflectioneffect/fadedirection/
---
## ReflectionEffect.FadeDirection property

Ottiene e imposta la direzione per spostare la riflessione.

```csharp
public double FadeDirection { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ReflectionEffectPropertyFadeDirectionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma per applicare l'effetto di riflessione
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            // Ottieni l'effetto di riflessione della forma
            ReflectionEffect reflection = shape.Reflection;

            // Visualizza il valore corrente di FadeDirection
            Console.WriteLine("Current FadeDirection value: " + reflection.FadeDirection);

            // Imposta un nuovo valore FadeDirection (90 gradi)
            reflection.FadeDirection = 90;
            Console.WriteLine("New FadeDirection value: " + reflection.FadeDirection);

            // Configura altre proprietà di riflessione per una migliore visibilità
            reflection.Type = ReflectionEffectType.TightReflectionTouching;
            reflection.Transparency = 0.5;
            reflection.Size = 50;
            reflection.Blur = 5;
            reflection.Distance = 10;

            // Salva la cartella di lavoro per vedere l'effetto
            workbook.Save("ReflectionEffectFadeDirectionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


