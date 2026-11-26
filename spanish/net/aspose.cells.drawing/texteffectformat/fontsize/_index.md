---
title: "TextEffectFormat.FontSize"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextEffectFormat. El tamaño en puntos de la fuente utilizada en WordArt"
type: docs
url: /es/net/aspose.cells.drawing/texteffectformat/fontsize/
---
## TextEffectFormat.FontSize property

El tamaño (en puntos) de la fuente utilizada en el WordArt.

```csharp
public int FontSize { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyFontSizeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un cuadro de texto a la hoja de cálculo
            int textboxIndex = worksheet.TextBoxes.Add(5, 5, 200, 100);
            Aspose.Cells.Drawing.TextBox textBox = worksheet.TextBoxes[textboxIndex];
            
            // Establecer texto y formato
            textBox.Text = "Sample Text Effect";
            
            // Obtener el formato de efecto de texto
            Shape shape = textBox;
            TextEffectFormat effectFormat = shape.TextEffect;
            
            // Establecer propiedades de fuente incluyendo FontSize
            effectFormat.FontName = "Arial";
            effectFormat.FontBold = true;
            effectFormat.FontItalic = false;
            effectFormat.FontSize = 18; // Demonstrating FontSize property
            
            // Guarda el libro de trabajo
            workbook.Save("TextEffectFontSizeDemo.xlsx");
            
            Console.WriteLine("Text effect with font size 18 created successfully.");
        }
    }
}
```

### Ver también

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


