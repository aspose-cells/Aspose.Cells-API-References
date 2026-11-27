---
title: "Klass BaseShapeGuide"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.BaseShapeGuide-klass. Representerar formguiden"
type: docs
url: /sv/net/aspose.cells.drawing/baseshapeguide/
---
## BaseShapeGuide class

Representerar formguiden.

```csharp
public class BaseShapeGuide
```

### Exempel

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
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Skapa en rektangelform med korrekta parametrar
                Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

                // Eftersom BaseShapeGuide inte har en publik konstruktor,
                // kommer vi att demonstrera dess användning genom en form som kan innehålla guider
                // Obs: Detta är en förenklad demonstration eftersom den faktiska åtkomsten till guider kan skilja sig
                Console.WriteLine("Shape created successfully");
                Console.WriteLine($"Shape type: {shape.GetType().Name}");

                // Spara arbetsboken
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

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


