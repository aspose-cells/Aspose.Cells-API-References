---
title: "FontSettingCollection.TextAlignment"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FontSettingCollection. Representa la configuración de alineación del cuerpo del texto"
type: docs
url: /es/net/aspose.cells.drawing.texts/fontsettingcollection/textalignment/
---
## FontSettingCollection.TextAlignment property

Representa la configuración de alineación del cuerpo del texto.

```csharp
public ShapeTextAlignment TextAlignment { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FontSettingCollectionPropertyTextAlignmentDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            shape.Text = "Sample Text";

            // Acceder y modificar las propiedades TextAlignment
            var textAlignment = shape.TextBody.TextAlignment;
            
            Console.WriteLine("Default Margins (Points):");
            Console.WriteLine($"AutoMargin: {textAlignment.IsAutoMargin}");
            Console.WriteLine($"Top: {textAlignment.TopMarginPt}");
            Console.WriteLine($"Bottom: {textAlignment.BottomMarginPt}");
            Console.WriteLine($"Left: {textAlignment.LeftMarginPt}");
            Console.WriteLine($"Right: {textAlignment.RightMarginPt}");

            // Modificar los márgenes
            textAlignment.TopMarginPt = 36;
            textAlignment.BottomMarginPt = 36;
            textAlignment.LeftMarginPt = 18;
            textAlignment.RightMarginPt = 18;

            // Guarda el libro de trabajo
            workbook.Save("TextAlignmentDemo.xlsx");

            Console.WriteLine("\nModified Margins (Points):");
            Console.WriteLine($"Top: {textAlignment.TopMarginPt}");
            Console.WriteLine($"Bottom: {textAlignment.BottomMarginPt}");
            Console.WriteLine($"Left: {textAlignment.LeftMarginPt}");
            Console.WriteLine($"Right: {textAlignment.RightMarginPt}");
        }
    }
}
```

### Ver también

* class [ShapeTextAlignment](../../shapetextalignment/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


