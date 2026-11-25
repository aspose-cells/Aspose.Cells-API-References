---
title: "ReflectionEffect.RotWithShape"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ReflectionEffect property. Ottiene e imposta se la riflessione deve ruotare con la forma"
type: docs
url: /it/net/aspose.cells.drawing/reflectioneffect/rotwithshape/
---
## ReflectionEffect.RotWithShape property

Ottiene e imposta se la riflessione deve ruotare con la forma.

```csharp
public bool RotWithShape { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ReflectionEffectPropertyRotWithShapeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma al foglio di lavoro
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Crea e applica l'effetto di riflessione
            ReflectionEffect reflection = shape.Reflection;
            reflection.Type = ReflectionEffectType.FullReflection4PtOffset;
            reflection.Blur = 5;
            reflection.Distance = 10;
            reflection.Transparency = 0.3;

            // Visualizza il valore corrente di RotWithShape
            Console.WriteLine("Current RotWithShape value: " + reflection.RotWithShape);

            // Imposta RotWithShape su true
            reflection.RotWithShape = true;
            Console.WriteLine("RotWithShape set to: " + reflection.RotWithShape);

            // Ruota la forma per dimostrare l'effetto
            shape.RotationAngle = 45;

            // Salva la cartella di lavoro
            workbook.Save("ReflectionEffectRotWithShapeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


