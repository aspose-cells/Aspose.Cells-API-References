---
title: "TextBoxOptions.TopMarginPt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextBoxOptions. Obtiene y establece el margen superior en unidades de puntos"
type: docs
url: /es/net/aspose.cells.drawing.texts/textboxoptions/topmarginpt/
---
## TextBoxOptions.TopMarginPt property

Obtiene y establece el margen superior en unidades de Puntos.

```csharp
public double TopMarginPt { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyTopMarginPtDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar un cuadro de texto a la hoja de cálculo
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            
            // Establecer el margen superior en puntos
            textBox.TextBoxOptions.TopMarginPt = 0.2d;
            
            // Guarda el libro de trabajo
            workbook.Save("TextBoxTopMarginDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


