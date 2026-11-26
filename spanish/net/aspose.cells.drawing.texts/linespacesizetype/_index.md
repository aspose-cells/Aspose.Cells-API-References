---
title: "Enum LineSpaceSizeType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.Texts.LineSpaceSizeType enum. Representa el tipo de unidad del tamaño del interlineado"
type: docs
url: /es/net/aspose.cells.drawing.texts/linespacesizetype/
---
## LineSpaceSizeType enumeration

Representa el tipo de unidad del tamaño del interlineado.

```csharp
public enum LineSpaceSizeType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Percentage | `0` | Representa en unidades de un porcentaje del tamaño del texto. |
| Points | `1` | Representa en unidades de puntos. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassLineSpaceSizeTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar una forma de cuadro de texto
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            
            // Establecer contenido de texto
            textBox.Text = "Sample Text\nSecond Line";
            
            // Acceder al primer párrafo del cuadro de texto
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];
            
            // Establecer el tipo de tamaño de espacio posterior a Puntos
            paragraph.SpaceAfterSizeType = LineSpaceSizeType.Points;
            
            // Establecer valor de espacio posterior (12 puntos)
            paragraph.SpaceAfter = 12;
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Text box with line spacing created successfully.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


