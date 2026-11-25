---
title: "ReflectionEffect.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ReflectionEffect property. Ottiene e imposta l'effetto di riflessione predefinito"
type: docs
url: /it/net/aspose.cells.drawing/reflectioneffect/type/
---
## ReflectionEffect.Type property

Ottiene e imposta l'effetto di riflessione predefinito.

```csharp
public ReflectionEffectType Type { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ReflectionEffectPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi una forma rettangolare
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            
            // Ottieni l'effetto di riflessione
            ReflectionEffect reflection = shape.Reflection;
            
            // Dimostra la proprietà Type
            Console.WriteLine("Initial reflection type: " + reflection.Type);
            
            // Cambia il tipo di riflessione
            reflection.Type = ReflectionEffectType.HalfReflectionTouching;
            Console.WriteLine("Updated reflection type: " + reflection.Type);
            
            // Imposta altre proprietà di riflessione
            reflection.Transparency = 0.5;
            reflection.Size = 55;
            reflection.Blur = 0.5;
            reflection.Distance = 0;
            
            // Salva la cartella di lavoro
            workbook.Save("ReflectionEffectDemo.xlsx");
            
            Console.WriteLine("Demo completed successfully.");
        }
    }
}
```

### Vedi anche

* enum [ReflectionEffectType](../../reflectioneffecttype/)
* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


