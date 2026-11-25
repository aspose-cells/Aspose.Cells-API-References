---
title: "Classe ShapeGuide"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.ShapeGuide. Incapsula una guida di forma che specifica la presenza di una guida di forma che verrà utilizzata per governare la geometria della forma specificata"
type: docs
url: /it/net/aspose.cells.drawing/shapeguide/
---
## ShapeGuide class

Incapsula una guida di forma che specifica la presenza di una guida di forma che sarà usata per governare la geometria della forma specificata

```csharp
public class ShapeGuide : BaseShapeGuide
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Value](../../aspose.cells.drawing/shapeguide/value/) { get; set; } | Ottiene o imposta il valore di questa guida |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapeGuideDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                var shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RoundedRectangle, 0, 0, 100, 100, 100, 100);
                
                // Crea e aggiungi una guida di forma con i parametri richiesti
                int guideIndex = shape.Geometry.ShapeAdjustValues.Add("Guide1", 0.2);
                ShapeGuide guide = shape.Geometry.ShapeAdjustValues[guideIndex];
                
                Console.WriteLine($"ShapeGuide created with Value: {guide.Value}");
                
                workbook.Save("DrawingClassShapeGuideDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [BaseShapeGuide](../baseshapeguide/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


