---
title: "ReflectionEffect.Size"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ReflectionEffect property. Ottiene e imposta la posizione finale lungo la rampa del gradiente alfa del valore alfa finale in unità di percentuale"
type: docs
url: /it/net/aspose.cells.drawing/reflectioneffect/size/
---
## ReflectionEffect.Size property

Ottiene e imposta la posizione finale (lungo la rampa del gradiente alfa) del valore alfa finale, in unità di percentuale.

```csharp
public double Size { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ReflectionEffectPropertySizeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            // Imposta le proprietà di riflessione includendo Size
            ReflectionEffect reflection = shape.Reflection;
            reflection.Type = ReflectionEffectType.HalfReflection4PtOffset;
            reflection.Transparency = 0.5;
            reflection.Size = 55.5;
            reflection.Blur = 0.5;
            reflection.Distance = 4;

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");

            // Verifica le proprietà di riflessione salvate
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            ReflectionEffect loadedReflection = loadedShape.Reflection;

            Console.WriteLine("Reflection Size: " + loadedReflection.Size);
        }
    }
}
```

### Vedi anche

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


