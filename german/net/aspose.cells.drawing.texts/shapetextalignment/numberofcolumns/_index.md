---
title: "ShapeTextAlignment.NumberOfColumns"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeTextAlignment-Eigenschaft. Ruft die Anzahl der Textspalten im Begrenzungsrechteck ab und legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing.texts/shapetextalignment/numberofcolumns/
---
## ShapeTextAlignment.NumberOfColumns property

Liest und setzt die Anzahl der Textspalten im Begrenzungsrechteck.

```csharp
public int NumberOfColumns { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyNumberOfColumnsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt eine Form hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);
            
            // Setzen Sie den Text für das Shape
            shape.Text = "This is sample text\nin multiple columns";
            
            // Zugriff auf die Textausrichtung und Festlegen der Spaltenanzahl
            shape.TextBody.TextAlignment.NumberOfColumns = 2;
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
            
            // Überprüfen Sie die Eigenschaft
            Console.WriteLine("Number of columns: " + 
                worksheet.Shapes[0].TextBody.TextAlignment.NumberOfColumns);
        }
    }
}
```

### Siehe auch

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


