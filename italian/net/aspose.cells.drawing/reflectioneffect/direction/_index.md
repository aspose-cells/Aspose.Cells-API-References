---
title: "ReflectionEffect.Direction"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ReflectionEffect. Restituisce e imposta la direzione della rampa di gradiente alfa rispetto alla forma stessa"
type: docs
url: /it/net/aspose.cells.drawing/reflectioneffect/direction/
---
## ReflectionEffect.Direction property

Ottiene e imposta la direzione della rampa del gradiente alfa rispetto alla forma stessa.

```csharp
public double Direction { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ReflectionEffectPropertyDirectionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma per applicare l'effetto di riflessione
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            
            // Ottieni l'effetto di riflessione della forma
            ReflectionEffect reflection = shape.Reflection;
            
            // Visualizza il valore corrente di Direction
            Console.WriteLine("Current Direction value: " + reflection.Direction);
            
            // Imposta un nuovo valore Direction (90 gradi)
            reflection.Direction = 90;
            Console.WriteLine("New Direction value: " + reflection.Direction);
            
            // Configura altre proprietà di riflessione per una migliore visibilità
            reflection.Type = ReflectionEffectType.TightReflectionTouching;
            reflection.Transparency = 0.5;
            reflection.Size = 50;
            reflection.Blur = 5;
            
            // Salva la cartella di lavoro per vedere l'effetto di riflessione
            workbook.Save("ReflectionEffectDirectionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


