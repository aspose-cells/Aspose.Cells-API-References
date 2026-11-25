---
title: "ReflectionEffect.Transparency"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ReflectionEffect. Restituisce e imposta il grado di trasparenza della riflessione iniziale come valore da 0.0 opaco a 1.0 trasparente"
type: docs
url: /it/net/aspose.cells.drawing/reflectioneffect/transparency/
---
## ReflectionEffect.Transparency property

Ottiene e imposta il grado di trasparenza della riflessione iniziale come valore da 0,0 (opaco) a 1,0 (trasparente).

```csharp
public double Transparency { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ReflectionEffectPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi una forma rettangolare al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            Aspose.Cells.Drawing.Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 200, 150);
            
            // Ottieni l'effetto di riflessione e imposta le sue proprietà
            Aspose.Cells.Drawing.ReflectionEffect reflection = rectangle.Reflection;
            reflection.Type = Aspose.Cells.Drawing.ReflectionEffectType.HalfReflectionTouching;
            reflection.Transparency = 0.5; // Demonstrate transparency property
            reflection.Size = 55;
            reflection.Blur = 0.5;
            reflection.Distance = 0;
            
            // Salva la cartella di lavoro
            workbook.Save("ReflectionEffectDemo.xlsx");
            
            // Verifica le proprietà salvate
            Workbook loadedWorkbook = new Workbook("ReflectionEffectDemo.xlsx");
            Aspose.Cells.Drawing.ReflectionEffect loadedReflection = loadedWorkbook.Worksheets[0].Shapes[0].Reflection;
            
            Console.WriteLine("Reflection Type: " + loadedReflection.Type);
            Console.WriteLine("Transparency: " + loadedReflection.Transparency);
            Console.WriteLine("Size: " + loadedReflection.Size);
            Console.WriteLine("Blur: " + loadedReflection.Blur);
            Console.WriteLine("Distance: " + loadedReflection.Distance);
        }
    }
}
```

### Vedi anche

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


