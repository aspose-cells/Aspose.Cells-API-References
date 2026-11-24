---
title: "ReflectionEffect.Size"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ReflectionEffect-Eigenschaft. Gibt die Endposition entlang der Alpha‑Verlaufsrampe des End‑Alpha‑Werts zurück und legt sie fest, angegeben in Prozent"
type: docs
url: /de/net/aspose.cells.drawing/reflectioneffect/size/
---
## ReflectionEffect.Size property

Ermittelt und setzt die Endposition (entlang der Alpha-Verlaufsrampe) des End-Alpha-Werts, in Prozent.

```csharp
public double Size { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Form hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            // Setzen Sie Reflexionseigenschaften einschließlich Größe
            ReflectionEffect reflection = shape.Reflection;
            reflection.Type = ReflectionEffectType.HalfReflection4PtOffset;
            reflection.Transparency = 0.5;
            reflection.Size = 55.5;
            reflection.Blur = 0.5;
            reflection.Distance = 4;

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");

            // Überprüfen Sie die gespeicherten Reflexionseigenschaften
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            ReflectionEffect loadedReflection = loadedShape.Reflection;

            Console.WriteLine("Reflection Size: " + loadedReflection.Size);
        }
    }
}
```

### Siehe auch

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


