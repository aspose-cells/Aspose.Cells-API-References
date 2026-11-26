---
title: "TextParagraph.LineSpaceSizeType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextParagraph. Obtiene y establece la cantidad de espacio vertical en blanco que se usará dentro de un párrafo"
type: docs
url: /es/net/aspose.cells.drawing.texts/textparagraph/linespacesizetype/
---
## TextParagraph.LineSpaceSizeType property

Obtiene y establece la cantidad de espacio blanco vertical que se utilizará dentro de un párrafo.

```csharp
public LineSpaceSizeType LineSpaceSizeType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextParagraphPropertyLineSpaceSizeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Añade un cuadro de texto y establece el texto
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            shape.Text = "First line\nSecond line";
            
            // Obtén el segundo párrafo
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            TextParagraph paragraph = paragraphs[1];
            
            // Establece las propiedades de interlineado
            paragraph.LineSpaceSizeType = LineSpaceSizeType.Points;
            paragraph.LineSpace = 2;
            paragraph.SpaceAfter = 3;
            paragraph.SpaceBefore = 4;
            
            // Guardar y exportar
            workbook.Save("TextParagraphPropertyLineSpaceSizeTypeDemo_output.xlsx");
            
            Console.WriteLine("Demo executed successfully. Output file created.");
        }
    }
}
```

### Ver también

* enum [LineSpaceSizeType](../../linespacesizetype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


