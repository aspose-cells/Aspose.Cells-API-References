---
title: "ReflectionEffect.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ReflectionEffect-Eigenschaft. Gibt den voreingestellten Reflexionseffekt zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing/reflectioneffect/type/
---
## ReflectionEffect.Type property

Ermittelt und setzt den voreingestellten Reflexionseffekt.

```csharp
public ReflectionEffectType Type { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Rechteckform hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            
            // Reflexionseffekt abrufen
            ReflectionEffect reflection = shape.Reflection;
            
            // Type-Eigenschaft demonstrieren
            Console.WriteLine("Initial reflection type: " + reflection.Type);
            
            // Reflexionstyp ändern
            reflection.Type = ReflectionEffectType.HalfReflectionTouching;
            Console.WriteLine("Updated reflection type: " + reflection.Type);
            
            // Weitere Reflexionseigenschaften festlegen
            reflection.Transparency = 0.5;
            reflection.Size = 55;
            reflection.Blur = 0.5;
            reflection.Distance = 0;
            
            // Speichere die Arbeitsmappe
            workbook.Save("ReflectionEffectDemo.xlsx");
            
            Console.WriteLine("Demo completed successfully.");
        }
    }
}
```

### Siehe auch

* enum [ReflectionEffectType](../../reflectioneffecttype/)
* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


