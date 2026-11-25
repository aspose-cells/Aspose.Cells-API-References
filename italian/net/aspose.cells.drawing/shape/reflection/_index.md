---
title: "Shape.Reflection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Rappresenta un oggetto ReflectionEffect che specifica l'effetto di riflessione per l'elemento del grafico o la forma."
type: docs
url: /it/net/aspose.cells.drawing/shape/reflection/
---
## Shape.Reflection property

Rappresenta un oggetto [`ReflectionEffect`](../../reflectioneffect/) che specifica l'effetto di riflessione per l'elemento del grafico o la forma.

```csharp
public ReflectionEffect Reflection { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyReflectionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Imposta le proprietà di riflessione
            ReflectionEffect reflection = shape.Reflection;
            reflection.Blur = 5;
            reflection.Distance = 10;
            reflection.Direction = 90;
            reflection.FadeDirection = 90;
            reflection.Size = 50;
            reflection.Transparency = 0.5;
            reflection.Type = ReflectionEffectType.None;

            // Salva la cartella di lavoro
            workbook.Save("ShapeReflectionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ReflectionEffect](../../reflectioneffect/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


