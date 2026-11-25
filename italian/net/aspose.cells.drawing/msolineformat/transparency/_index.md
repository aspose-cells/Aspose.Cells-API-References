---
title: "MsoLineFormat.Transparency"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoLineFormat. Restituisce o imposta il grado di trasparenza del riempimento specificato come valore da 0.0 opaco a 1.0 trasparente"
type: docs
url: /it/net/aspose.cells.drawing/msolineformat/transparency/
---
## MsoLineFormat.Transparency property

Restituisce o imposta il grado di trasparenza del riempimento specificato come valore da 0.0 (opaco) a 1.0 (trasparente).

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
    public class MsoLineFormatPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma ad arco
            ArcShape arc = worksheet.Shapes.AddArc(1, 0, 1, 0, 100, 100);

            // Imposta le proprietà del formato linea includendo la trasparenza
            arc.LineFormat.ForeColor = System.Drawing.Color.Red;
            arc.LineFormat.Transparency = 0.5; // 50% transparent
            arc.LineFormat.Weight = 3;
            arc.LineFormat.DashStyle = MsoLineDashStyle.Solid;

            // Crea un altro arco per confronto
            ArcShape arc2 = worksheet.Shapes.AddArc(1, 2, 1, 2, 100, 100);
            arc2.LineFormat.ForeColor = System.Drawing.Color.Red;
            arc2.LineFormat.Transparency = 0.5; // Same transparency
            arc2.LineFormat.Weight = 3;
            arc2.LineFormat.DashStyle = MsoLineDashStyle.Solid;

            // Verifica la proprietà di trasparenza
            if (Math.Abs(arc.LineFormat.Transparency - arc2.LineFormat.Transparency) < 0.001)
            {
                Console.WriteLine("Transparency properties match: " + arc.LineFormat.Transparency);
            }
            else
            {
                Console.WriteLine("Transparency properties do not match");
            }

            // Salva la cartella di lavoro
            workbook.Save("MsoLineFormatTransparencyDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


