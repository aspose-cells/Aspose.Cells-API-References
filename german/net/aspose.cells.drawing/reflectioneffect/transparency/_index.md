---
title: "ReflectionEffect.Transparency"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ReflectionEffect-Eigenschaft. Gibt den Grad der Anfangsreflexions-Transparenz als Wert von 0,0 (undurchsichtig) bis 1,0 (klar) zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing/reflectioneffect/transparency/
---
## ReflectionEffect.Transparency property

Ermittelt und setzt den Grad der Anfangs-Reflexions-Transparenz als Wert von 0,0 (undurchsichtig) bis 1,0 (klar).

```csharp
public double Transparency { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Fügt dem ersten Arbeitsblatt ein Rechteck-Shape hinzu.
            Worksheet worksheet = workbook.Worksheets[0];
            Aspose.Cells.Drawing.Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 200, 150);
            
            // Abrufen Sie den Reflexionseffekt und setzen Sie seine Eigenschaften
            Aspose.Cells.Drawing.ReflectionEffect reflection = rectangle.Reflection;
            reflection.Type = Aspose.Cells.Drawing.ReflectionEffectType.HalfReflectionTouching;
            reflection.Transparency = 0.5; // Demonstrate transparency property
            reflection.Size = 55;
            reflection.Blur = 0.5;
            reflection.Distance = 0;
            
            // Speichere die Arbeitsmappe
            workbook.Save("ReflectionEffectDemo.xlsx");
            
            // Überprüfe die gespeicherten Eigenschaften
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

### Siehe auch

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


