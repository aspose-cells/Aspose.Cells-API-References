---
title: "TextParagraph.SpaceAfterSizeType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextParagraph. Obtiene y establece la cantidad de espacio vertical que habrá después de un párrafo"
type: docs
url: /es/net/aspose.cells.drawing.texts/textparagraph/spaceaftersizetype/
---
## TextParagraph.SpaceAfterSizeType property

Obtiene y establece la cantidad de espacio en blanco vertical que estará presente después de un párrafo.

```csharp
public LineSpaceSizeType SpaceAfterSizeType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextParagraphPropertySpaceAfterSizeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar un cuadro de texto y establecer texto con varios párrafos
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            shape.Text = "First paragraph\nSecond paragraph";
            
            // Obtén el segundo párrafo
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            TextParagraph paragraph = paragraphs[1];
            
            // Establecer propiedades de espacio con tipo de tamaño
            paragraph.SpaceAfterSizeType = LineSpaceSizeType.Points;
            paragraph.SpaceAfter = 10; // 10 points space after
            
            // Guarde y recargue para verificar
            string filePath = "TextParagraphPropertySpaceAfterSizeTypeDemo_Output.xlsx";
            workbook.Save(filePath);
            
            Workbook loadedWorkbook = new Workbook(filePath);
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            TextParagraph loadedParagraph = loadedShape.TextBody.TextParagraphs[1];
            
            Console.WriteLine("SpaceAfterSizeType: " + loadedParagraph.SpaceAfterSizeType);
            Console.WriteLine("SpaceAfter: " + loadedParagraph.SpaceAfter);
        }
    }
}
```

### Ver también

* enum [LineSpaceSizeType](../../linespacesizetype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


