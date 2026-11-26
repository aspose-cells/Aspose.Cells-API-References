---
title: "ShapeTextAlignment.TextShapeType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShapeTextAlignment. Obtiene y establece el tipo de transformación del texto"
type: docs
url: /es/net/aspose.cells.drawing.texts/shapetextalignment/textshapetype/
---
## ShapeTextAlignment.TextShapeType property

Obtiene y establece el tipo de transformación del texto.

```csharp
public AutoShapeType TextShapeType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyTextShapeTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de cuadro de texto
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);

            // Obtener la alineación del texto de la forma
            ShapeTextAlignment shapeTextAlignment = textBox.TextBody.TextAlignment;

            // Establecer la propiedad TextShapeType
            shapeTextAlignment.TextShapeType = AutoShapeType.TextBox;

            // Guarda el libro de trabajo
            workbook.Save("TextShapeTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [AutoShapeType](../../../aspose.cells.drawing/autoshapetype/)
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


