---
title: "TextParagraph.SpaceBeforeSizeType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextParagraph. Obtiene y establece la cantidad de espacio en blanco vertical que estará presente antes de un párrafo"
type: docs
url: /es/net/aspose.cells.drawing.texts/textparagraph/spacebeforesizetype/
---
## TextParagraph.SpaceBeforeSizeType property

Obtiene y establece la cantidad de espacio en blanco vertical que estará presente antes de un párrafo.

```csharp
public LineSpaceSizeType SpaceBeforeSizeType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextParagraphPropertySpaceBeforeSizeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar un cuadro de texto y obtener su forma
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            shape.Text = "First paragraph\nSecond paragraph";
            
            // Acceder al segundo párrafo
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            TextParagraph paragraph = paragraphs[1];
            
            // Establecer propiedades de espaciado de párrafo
            paragraph.LineSpaceSizeType = LineSpaceSizeType.Points;
            paragraph.SpaceBeforeSizeType = LineSpaceSizeType.Points;
            paragraph.SpaceAfterSizeType = LineSpaceSizeType.Points;
            
            paragraph.LineSpace = 12;
            paragraph.SpaceBefore = 8;
            paragraph.SpaceAfter = 10;
            
            // Guarde y vuelva a cargar para demostrar la persistencia
            string outputPath = "TextParagraphSpacingDemo.xlsx";
            workbook.Save(outputPath);
            
            // Recargar para verificar propiedades
            Workbook loadedWorkbook = new Workbook(outputPath);
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            TextParagraph loadedParagraph = loadedShape.TextBody.TextParagraphs[1];
            
            Console.WriteLine("SpaceBeforeSizeType: " + loadedParagraph.SpaceBeforeSizeType);
            Console.WriteLine("SpaceBefore: " + loadedParagraph.SpaceBefore);
            Console.WriteLine("SpaceAfterSizeType: " + loadedParagraph.SpaceAfterSizeType);
            Console.WriteLine("SpaceAfter: " + loadedParagraph.SpaceAfter);
            Console.WriteLine("LineSpaceSizeType: " + loadedParagraph.LineSpaceSizeType);
            Console.WriteLine("LineSpace: " + loadedParagraph.LineSpace);
        }
    }
}
```

### Ver también

* enum [LineSpaceSizeType](../../linespacesizetype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


