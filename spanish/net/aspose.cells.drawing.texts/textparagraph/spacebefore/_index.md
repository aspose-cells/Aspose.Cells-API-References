---
title: "TextParagraph.SpaceBefore"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextParagraph. Obtiene y establece la cantidad de espacio en blanco vertical que estará presente antes de un párrafo"
type: docs
url: /es/net/aspose.cells.drawing.texts/textparagraph/spacebefore/
---
## TextParagraph.SpaceBefore property

Obtiene y establece la cantidad de espacio en blanco vertical que estará presente antes de un párrafo.

```csharp
public double SpaceBefore { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextParagraphPropertySpaceBeforeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregue un cuadro de texto y establezca el texto
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            shape.Text = "First paragraph\nSecond paragraph";
            
            // Obtenga los párrafos
            Aspose.Cells.Drawing.Texts.TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            
            // Configure el espaciado del segundo párrafo
            Aspose.Cells.Drawing.Texts.TextParagraph p = paragraphs[1];
            p.LineSpaceSizeType = Aspose.Cells.Drawing.Texts.LineSpaceSizeType.Points;
            p.LineSpace = 2;
            p.SpaceAfter = 3;
            p.SpaceBefore = 4; // Demonstrate SpaceBefore property
            
            // Guardar y verificar
            string outputPath = "output_SpaceBeforeDemo.xlsx";
            workbook.Save(outputPath);
            
            Console.WriteLine("Demo completed. File saved: " + outputPath);
        }
    }
}
```

### Ver también

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


