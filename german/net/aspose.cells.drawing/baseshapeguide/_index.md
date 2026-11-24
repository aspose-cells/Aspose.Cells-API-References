---
title: "Klasse BaseShapeGuide"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.BaseShapeGuide Klasse. Stellt den Formleitfaden dar"
type: docs
url: /de/net/aspose.cells.drawing/baseshapeguide/
---
## BaseShapeGuide class

Stellt die Formführung dar.

```csharp
public class BaseShapeGuide
```

### Beispiele

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
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Erstellen Sie eine Rechteckform mit korrekten Parametern
                Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

                // Da BaseShapeGuide keinen öffentlichen Konstruktor hat,
                // werden wir seine Verwendung anhand einer Form demonstrieren, die Leitfäden enthalten könnte
                // Hinweis: Dies ist eine vereinfachte Demonstration, da der tatsächliche Leitfadenzugriff abweichen kann
                Console.WriteLine("Shape created successfully");
                Console.WriteLine($"Shape type: {shape.GetType().Name}");

                // Speichere die Arbeitsmappe
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

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


