---
title: "ShapePath.ShapePath"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore ShapePath. Inizializza una nuova istanza della classe ShapePath"
type: docs
url: /it/net/aspose.cells.drawing/shapepath/shapepath/
---
## ShapePath constructor

Inizializza una nuova istanza della classe [`ShapePath`](../).

```csharp
public ShapePath()
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodCtorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crea un nuovo percorso di forma usando il metodo #ctor
                ShapePath shapePath = new ShapePath();

                // Aggiungi segmenti di percorso per creare una forma semplice
                shapePath.MoveTo(100, 100);
                shapePath.LineTo(200, 100);
                shapePath.LineTo(200, 200);
                shapePath.LineTo(100, 200);
                shapePath.Close();

                //aggiungi forma libera
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 200, 200, new ShapePath[] { shapePath });

                Console.WriteLine("ShapePath created and added to worksheet successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ShapePath constructor: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("ShapePathMethodCtorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


