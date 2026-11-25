---
title: "ReflectionEffect.Blur"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ReflectionEffect property. Ottiene e imposta il raggio di sfocatura in unità di punti"
type: docs
url: /it/net/aspose.cells.drawing/reflectioneffect/blur/
---
## ReflectionEffect.Blur property

Ottiene e imposta il raggio di sfocatura, in unità di punti.

```csharp
public double Blur { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ReflectionEffectPropertyBlurDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi una forma rettangolare
            Aspose.Cells.Drawing.Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            
            // Accedi all'effetto di riflessione
            Aspose.Cells.Drawing.ReflectionEffect reflection = rectangle.Reflection;
            
            // Imposta il tipo di riflessione e le proprietà
            reflection.Type = Aspose.Cells.Drawing.ReflectionEffectType.HalfReflectionTouching;
            reflection.Blur = 0.5; // Demonstrate Blur property
            reflection.Transparency = 0.5;
            reflection.Size = 55;
            reflection.Distance = 0;
            
            // Salva la cartella di lavoro
            workbook.Save("ReflectionEffectDemo.xlsx");
            
            // Visualizza il valore di sfocatura
            Console.WriteLine("Reflection Blur: " + reflection.Blur);
        }
    }
}
```

### Vedi anche

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


