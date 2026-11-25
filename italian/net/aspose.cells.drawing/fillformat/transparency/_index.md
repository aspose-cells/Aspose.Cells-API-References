---
title: "FillFormat.Transparency"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FillFormat. Restituisce o imposta il grado di trasparenza dell'area come valore da 0.0 opaco a 1.0 trasparente"
type: docs
url: /it/net/aspose.cells.drawing/fillformat/transparency/
---
## FillFormat.Transparency property

Restituisce o imposta il grado di trasparenza dell'area come valore da 0,0 (opaco) a 1,0 (trasparente).

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
    public class FillFormatPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma per dimostrare la trasparenza
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 200, 100, 50, 50);

            // Imposta le proprietà di riempimento con trasparenza
            shape.Fill.FillType = FillType.Solid;
            shape.Fill.SolidFill.Color = System.Drawing.Color.Blue;
            shape.Fill.Transparency = 0.3; // 30% transparent

            // Salva la cartella di lavoro
            workbook.Save("FillFormatTransparencyDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


