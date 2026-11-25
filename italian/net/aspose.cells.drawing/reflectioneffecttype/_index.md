---
title: "Enum ReflectionEffectType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.ReflectionEffectType enum. Rappresenta il tipo di effetto di riflessione"
type: docs
url: /it/net/aspose.cells.drawing/reflectioneffecttype/
---
## ReflectionEffectType enumeration

Rappresenta il tipo di effetto di riflessione.

```csharp
public enum ReflectionEffectType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Nessun effetto di riflessione. |
| Custom | `1` | Effetto di riflessione personalizzato. |
| TightReflectionTouching | `2` | Riflessione stretta, a contatto. |
| HalfReflectionTouching | `3` | Riflessione a metà, a contatto. |
| FullReflectionTouching | `4` | Riflessione completa, a contatto. |
| TightReflection4PtOffset | `5` | Riflessione stretta, offset di 4 pt. |
| HalfReflection4PtOffset | `6` | Riflessione a metà, offset di 4 pt. |
| FullReflection4PtOffset | `7` | Riflessione completa, offset di 4 pt. |
| TightReflection8PtOffset | `8` | Riflessione stretta, offset di 8 pt. |
| HalfReflection8PtOffset | `9` | Riflessione a metà, offset di 8 pt. |
| FullReflection8PtOffset | `10` | Riflessione completa, offset di 8 pt. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassReflectionEffectTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi una forma rettangolare
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            
            // Ottieni l'effetto di riflessione
            ReflectionEffect reflection = rectangle.Reflection;
            
            // Imposta le proprietà di riflessione
            reflection.Type = ReflectionEffectType.HalfReflectionTouching;
            reflection.Transparency = 0.5;
            reflection.Size = 55;
            reflection.Blur = 0.5;
            reflection.Distance = 0;
            
            // Salva la cartella di lavoro
            workbook.Save("DrawingClassReflectionEffectTypeDemo.xlsx");
            
            Console.WriteLine("Reflection effect demo completed successfully.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


