---
title: "ShapePath.Close"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ShapePath metodo. Chiude la figura corrente e avvia una nuova figura. Se la figura corrente contiene una sequenza di linee e curve collegate, il metodo chiude il ciclo collegando una linea dal punto finale al punto di partenza."
type: docs
url: /it/net/aspose.cells.drawing/shapepath/close/
---
## ShapePath.Close method

Chiude la figura corrente e avvia una nuova figura. Se la figura corrente contiene una sequenza di linee e curve collegate, il metodo chiude il ciclo collegando una linea dal punto finale al punto di partenza.

```csharp
public void Close()
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodCloseDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                //Crea un nuovo percorso di forma
                ShapePath shapePath = new ShapePath();
                shapePath.MoveTo(60, 45);
                shapePath.ArcTo(25, 25, 0, 270);

                // Chiudi il percorso 
                shapePath.Close();

                shapePath.MoveTo(60, 20);
                shapePath.LineTo(110, 70);
                shapePath.LineTo(125, 155.5f);
                shapePath.ArcTo(35.5f, 35.5f, 0, 270);

                // Chiudi il percorso 
                shapePath.Close();

                //aggiungi forma libera
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

                Console.WriteLine("Close method called successfully to complete the shape path");
                
                // Salva la cartella di lavoro
                workbook.Save("ShapePathMethodCloseDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling Close method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


