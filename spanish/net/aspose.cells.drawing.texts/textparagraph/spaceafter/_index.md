---
title: "TextParagraph.SpaceAfter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextParagraph. Obtiene y establece la cantidad de espacio vertical que habrá después de un párrafo"
type: docs
url: /es/net/aspose.cells.drawing.texts/textparagraph/spaceafter/
---
## TextParagraph.SpaceAfter property

Obtiene y establece la cantidad de espacio en blanco vertical que estará presente después de un párrafo.

```csharp
public double SpaceAfter { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextParagraphPropertySpaceAfterDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregue un cuadro de texto y establezca el texto
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            shape.Text = "First paragraph\nSecond paragraph";
            
            // Obtenga los párrafos
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            
            // Configure el espaciado del segundo párrafo
            TextParagraph p = paragraphs[1];
            p.LineSpaceSizeType = LineSpaceSizeType.Points;
            p.LineSpace = 2;
            p.SpaceAfter = 3; // Demonstrate SpaceAfter property
            p.SpaceBefore = 4;
            
            // Guardar y verificar
            workbook.Save("TextParagraphPropertySpaceAfterDemo.xlsx");
            
            // Recarga para verificar la configuración
            Workbook loadedWorkbook = new Workbook("TextParagraphPropertySpaceAfterDemo.xlsx");
            TextParagraph loadedPara = loadedWorkbook.Worksheets[0].Shapes[0].TextBody.TextParagraphs[1];
            
            Console.WriteLine("SpaceAfter: " + loadedPara.SpaceAfter);
            Console.WriteLine("SpaceBefore: " + loadedPara.SpaceBefore);
            Console.WriteLine("LineSpace: " + loadedPara.LineSpace);
        }
    }
}
```

### Ver también

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


