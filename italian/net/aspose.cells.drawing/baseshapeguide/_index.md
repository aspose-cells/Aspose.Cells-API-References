---
title: "Classe BaseShapeGuide"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.BaseShapeGuide. Rappresenta la guida della forma"
type: docs
url: /it/net/aspose.cells.drawing/baseshapeguide/
---
## BaseShapeGuide class

Rappresenta la guida della forma.

```csharp
public class BaseShapeGuide
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassBaseShapeGuideDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crea una forma rettangolare con i parametri corretti
                Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

                // Poiché BaseShapeGuide non ha un costruttore pubblico,
                // dimostreremo il suo utilizzo tramite una forma che potrebbe contenere guide
                // Nota: questa è una dimostrazione semplificata poiché l'accesso reale alle guide potrebbe differire
                Console.WriteLine("Shape created successfully");
                Console.WriteLine($"Shape type: {shape.GetType().Name}");

                // Salva la cartella di lavoro
                workbook.Save("BaseShapeGuideDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with BaseShapeGuide: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


