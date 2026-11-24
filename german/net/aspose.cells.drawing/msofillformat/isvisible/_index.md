---
title: "MsoFillFormat.IsVisible"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoFillFormat-Eigenschaft. Gibt an, ob eine Füllung vorhanden ist"
type: docs
url: /de/net/aspose.cells.drawing/msofillformat/isvisible/
---
## MsoFillFormat.IsVisible property

Gibt an, ob eine Füllung vorhanden ist.

```csharp
public bool IsVisible { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFillFormatPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Beispielform
            Shape shape1 = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            Shape shape2 = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 100, 150);

            // Setze die Füllsichtbarkeit für shape1 (sichtbar)
            shape1.FillFormat.IsVisible = true;
            shape1.FillFormat.ForeColor = System.Drawing.Color.Red;
            
            // Setze die Füllsichtbarkeit für shape2 (unsichtbar)
            shape2.FillFormat.IsVisible = false;

            // Demonstriere die Verwendung der IsVisible-Eigenschaft
            Console.WriteLine("Shape1 Fill Visible: " + shape1.FillFormat.IsVisible);
            Console.WriteLine("Shape2 Fill Visible: " + shape2.FillFormat.IsVisible);

            // Vergleiche die Füllsichtbarkeit zwischen den Formen
            if (shape1.FillFormat.IsVisible && shape2.FillFormat.IsVisible)
            {
                Console.WriteLine("Both shapes have visible fills");
            }
            else
            {
                Console.WriteLine("At least one shape has invisible fill");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("MsoFillFormatIsVisibleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


