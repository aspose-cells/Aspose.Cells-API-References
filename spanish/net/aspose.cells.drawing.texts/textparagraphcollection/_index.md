---
title: "Clase TextParagraphCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.Texts.TextParagraphCollection. Representa todos los párrafos de texto"
type: docs
url: /es/net/aspose.cells.drawing.texts/textparagraphcollection/
---
## TextParagraphCollection class

Representa todo el párrafo de texto.

```csharp
public class TextParagraphCollection : IEnumerable
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.cells.drawing.texts/textparagraphcollection/count/) { get; } | Obtiene la cantidad de párrafos de texto. |
| [Item](../../aspose.cells.drawing.texts/textparagraphcollection/item/) { get; } | Obtiene el objeto [`TextParagraph`](../textparagraph/) en un índice específico. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetEnumerator](../../aspose.cells.drawing.texts/textparagraphcollection/getenumerator/)() | Obtiene el enumerador de los párrafos. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassTextParagraphCollectionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar un cuadro de texto a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            
            // Establecer texto multilínea
            shape.Text = "First paragraph\nSecond paragraph";
            
            // Obtener la colección de párrafos
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            
            // Acceder y modificar el segundo párrafo
            TextParagraph secondParagraph = paragraphs[1];
            secondParagraph.LineSpaceSizeType = LineSpaceSizeType.Points;
            secondParagraph.LineSpace = 20;
            secondParagraph.SpaceAfter = 30;
            secondParagraph.SpaceBefore = 40;
            
            // Guarda el libro de trabajo
            workbook.Save("TextParagraphCollectionDemo.xlsx");
            
            Console.WriteLine("Text paragraph formatting saved successfully.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


