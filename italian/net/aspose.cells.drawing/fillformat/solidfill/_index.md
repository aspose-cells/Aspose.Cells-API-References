---
title: "FillFormat.SolidFill"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FillFormat. Ottiene l'oggetto SolidFill"
type: docs
url: /it/net/aspose.cells.drawing/fillformat/solidfill/
---
## FillFormat.SolidFill property

Ottiene l'oggetto `SolidFill`.

```csharp
public SolidFill SolidFill { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertySolidFillDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi una forma rettangolare
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            
            // Imposta il colore di riempimento solido per la forma
            shape.Fill.SolidFill.Color = System.Drawing.Color.FromArgb(135, 222, 255);
            
            // Ottieni e visualizza il colore di riempimento solido
            System.Drawing.Color fillColor = shape.Fill.SolidFill.Color;
            Console.WriteLine("Solid Fill Color - R:{0}, G:{1}, B:{2}", 
                fillColor.R, fillColor.G, fillColor.B);
            
            // Salva la cartella di lavoro
            workbook.Save("SolidFillDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SolidFill](../../solidfill/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


